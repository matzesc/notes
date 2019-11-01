# FPGA Development

- [Personal Notes](README.md)

## Altera/Intel

- [Arria V Handbook](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/hb/arria-v/arriav_handbook.pdf)
- [Stratix V Handbook](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/hb/stratix-v/stratix5_handbook.pdf)
- [DSP Builder Version History and Software Requirements](https://www.intel.com/content/www/us/en/programmable/support/support-resources/intellectual-property/dsp/dsp-builder/ips-dsp-version.html)

### Altera Signal Processing

- [AN639: Inferring Stratix V DSP Blocks for FIR Filtering Applications](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/an/an639.pdf)

### Quartus Scripting

- [Command Line Scripting](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/hb/qts/qts_qii52002.pdf)
- [Tcl Scripting](https://www.intel.com/content/dam/www/programmable/us/en/pdfs/literature/hb/qts/qts_qii52003.pdf)
  - [Quartus II Tcl Examples](https://www.intel.com/content/altera-www/global/en_us/index/support/support-resources/design-examples/design-software/tcl.html)
  - [Quartus II Tcl Example: Opening Projects](https://www.intel.com/content/www/us/en/programmable/support/support-resources/design-examples/design-software/tcl/open_project.html)
  - [TCL Commands and Packages](https://www.intel.com/content/www/us/en/programmable/quartushelp/current/index.htm#tafs/tafs/tafs.htm)

## Xilinx

### Xilinx Signal Processing

- [FIR Compiler](https://www.xilinx.com/support/documentation/ip_documentation/fir_compiler/v7_2/pg149-fir-compiler.pdf)
- [DDS Compiler](https://www.xilinx.com/support/documentation/ip_documentation/dds_compiler/v6_0/pg141-dds-compiler.pdf) (Direct Digital Synthesizer), also know as NCO (Numeric Controlled Oscillator)

## ModelSim

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
