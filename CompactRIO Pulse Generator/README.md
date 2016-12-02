# CompactRIO pulse generator
This project implements a pulse generator, sometimes called a delay generator, using a National Instruments CompactRIO 9075 and an NI 9401 DIO module.

## Installation
This example is implemented in LabVIEW 2013, though it should work in later versions without modification. To get this example to work you will need to install the following National Instruments software:
 *	LabVIEW 2013 SP1
 *	LabVIEW Real-Time 2013 SP1
 *	LabVIEW FPGA 2013 SP1
 *	CompactRIO driver 2014 r1
 * 	Xilinx Toolchain 14.4

## Deployment checklist
a.	Insert the NI 9401 DIO module into slot 1.
b.	Physically connect the CompactRIO to the host PC using a crossover Ethernet cable.
c.	In Windows Device Manager set the host PC IP address to 192.168.0.1 on the Ethernet interface.
d.	Connect the power to the CompactRIO and power it up
e.	In NI Measurement and Automation Explorer setup the CompactRIO to use static IP address 192.168.0.2, subnet mask 255.255.255.0, Gateway and DNS server 0.0.0.0 and save the settings. 
f.	Install CompactRIO Support 13.0 and NI-RIO 13.0 onto the device.
g.	Power down the CompactRIO and physically connect the hardware that will receive the pulses to the NI 9401 DIO module. The NI 9924 Terminal Block provides a convenient way to break out the connections.
h.	Verify that the device is present in Measurement and Automation Explorer.
i.	Compile the FPGA VI and run it.

## Disclaimer
Delay generators are often used to provide timing signals for expensive scientific equipment. It is up to you to read and understand this code before deploying it to ensure that it is compatible with your requirements. 

Or, to put it in legalese:

THIS SOFTWARE IS PROVIDED "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

## License
All code is made available under the Creative Commons Attribution (CC-BY) license v4.0.
[https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/ "View license")
