# FPGA Development

- Back to [Personal Notes](README.md)

## Altera/Intel

- [Intel FPGAs and Programmable Devices](https://www.intel.com/content/www/us/en/products/programmable.html)
  - [Arria V Handbook](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/hb/arria-v/arriav_handbook.pdf)
  - [Stratix V Handbook](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/hb/stratix-v/stratix5_handbook.pdf)
  - [DSP Builder Version History and Software Requirements](https://www.intel.com/content/www/us/en/programmable/support/support-resources/intellectual-property/dsp/dsp-builder/ips-dsp-version.html)

### Legacy Altera URLs

Old Altera URLs (now redirecting to Intel Website):

- [Altera.com](https://www.altera.com)
- [AlteraForum.com](https://www.alteraforum.com/)
- [AlteraWiki.com](https://www.alterawiki.com)

Old Altera Wiki Articles (new links to Intel Website):

- [TimeQuest User Guide](https://forums.intel.com/s/createarticlepage?articleid=a3g0P0000005R9MQAU&action=view&language=en_US)
  - [Paper - TimeQuest User Guide, v1.1, R. Scoville](https://www.intel.com/content/dam/altera-www/global/en_US/uploads/3/3f/TimeQuest_User_Guide.pdf)
- [Source Synchronous Analysis with TimeQuest](https://forums.intel.com/s/createarticlepage?language=en_US&articleid=a3g0P0000005RIKQA2&artTopicId=0TO0P000000MWKBWA4&action=view)
  - [Paper - Source-Synchronous Timing with TimeQuest, v1.2, R. Scoville](https://www.intel.com/content/dam/altera-www/global/en_US/uploads/e/ea/Source_Synchronous_Timing.pdf)
- [Transceiver Toolkit](https://forums.intel.com/s/createarticlepage?articleid=a3g0P0000005RAtQAM&action=view&language=en_US)
- [DDR Timing with TimeQuest](https://forums.intel.com/s/createarticlepage?articleid=a3g0P0000005QzHQAU&action=view&language=en_US)

### Altera Signal Processing

- [AN639: Inferring Stratix V DSP Blocks for FIR Filtering Applications](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/an/an639.pdf)

### Quartus Scripting

- [Command Line Scripting](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/hb/qts/qts_qii52002.pdf)
- [Tcl Scripting](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/hb/qts/qts_qii52003.pdf)
  - [Quartus II Tcl Examples](https://www.intel.com/content/altera-www/global/en_us/index/support/support-resources/design-examples/design-software/tcl.html)
  - [Quartus II Tcl Example: Opening Projects](https://www.intel.com/content/www/us/en/programmable/support/support-resources/design-examples/design-software/tcl/open_project.html)
  - [TCL Commands and Packages](https://www.intel.com/content/www/us/en/programmable/quartushelp/current/index.htm#tafs/tafs/tafs.htm)

### Altera/Intel IP Cores

- [ASMI Parallel Intel® FPGA IP CoreUser Guide](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/ug/ug_altasmi_parallel.pdf)
- [FIFO Intel® FPGA IP User Guide](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/ug/ug_fifo.pdf)
- [Internal Memory (RAM and ROM) User Guide](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/ug/ug_ram.pdf)
- [LVDS SERDES Transmitter / ReceiverIP Cores User Guide](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/ug/ug_altlvds.pdf)
- [Remote Update Intel® FPGA IP User Guide](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/ug/ug_altremote.pdf)
- [Triple-Speed Ethernet Intel® FPGA IP User Guide](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/ug/ug_ethernet.pdf)
- [V-Series Transceiver PHY IP Core User Guide](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/ug/xcvr_user_guide.pdf)

## Xilinx

### Xilinx Signal Processing

- [FIR Compiler](https://www.xilinx.com/support/documentation/ip_documentation/fir_compiler/v7_2/pg149-fir-compiler.pdf)
- [DDS Compiler](https://www.xilinx.com/support/documentation/ip_documentation/dds_compiler/v6_0/pg141-dds-compiler.pdf) (Direct Digital Synthesizer), also know as NCO (Numeric Controlled Oscillator)

## ModelSim

- [Mentor - ModelSim](https://www.mentor.com/products/fv/modelsim/)

Create library folder:

    vlib work

Command to compile VHDL file from command line:

    vcom -work work -2008 -explicit -check_synthesis -lint test.vhd

## Doxygen VHDL support

- [Doxygen - Comment blocks in VHDL](http://www.doxygen.nl/manual/docblocks.html#vhdlblocks)
- [Generate VHDL Doxygen documentation in Sigasi](https://insights.sigasi.com/tech/generate-vhdl-doxygen-documentation-sigasi/)

## Systolic FIR Filters

- H. T. Kung, "[Why Systolic Architecture?](https://www.eecs.harvard.edu/~htk/publication/1982-kung-why-systolic-architecture.pdf)", *IEEE Computers Magazine*, Vol. 15, No 1, pp. 37-46, Jan. 1982.
- [Pipelined Direct Form FIR Versus the Transposed Structure](https://www.allaboutcircuits.com/technical-articles/pipelined-direct-form-fir-versus-the-transposed-structure/)
- [Systolic FIR Filter Based FPGA](https://www.design-reuse.com/articles/19106/systolic-fir-filter-based-fpga.html)

## FPGA Development related Websites

- [Mentor - Verification Academy](https://verificationacademy.com/)
- [EDAPlayground](https://www.edaplayground.com/)

## Verification Frameworks

### Universal Verification Methodology (UVM)

- [Accellera - UVM Community](https://www.accellera.org/community/uvm/)
  - [Download UVM](https://www.accellera.org/downloads/standards/uvm)
- [Mentor - Universal Verification Methodology (UVM)](https://www.mentor.com/products/fv/uvm)
- [Universal Verification Methodology](http://www.learnuvmverification.com/)

### Open Source VHDL Verification Methodology (OSVVM)

- [SynthWorks Blog - OSVVM](http://www.synthworks.com/blog/osvvm/)
- [Github - OSVVM](https://github.com/OSVVM)
  - [Github - Open Source VHDL Verification Methodology (OSVVM) Repository](https://github.com/OSVVM/OSVVM)
- [Doulos - The Open Source VHDL Verification Methodology (OSVVM)](https://www.doulos.com/knowhow/vhdl_designers_guide/OSVVM/)
- [Medium - Shorten FPGA Development Time with Open Source VHDL Verification Methodology](https://medium.com/@einfochips/shorten-fgpa-development-time-with-open-source-vhdl-verification-methodology-ca5254d5132e)

### Universal VHDL Verification Methodology (UVVM)

- [UVVM.org](https://uvvm.org/)
  - [UVVM Forum](https://forum.uvvm.org/)
- [bitvis.no - Universal VHDL Verification Methodology](https://bitvis.no/dev-tools/uvvm/)
- [Github - UVVM](https://github.com/UVVM)
  - [Github - Universal VHDL Verification Methodology (UVVM) Repository](https://github.com/UVVM/UVVM)
