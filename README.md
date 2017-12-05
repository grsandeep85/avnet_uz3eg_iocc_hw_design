Vivado Design
=============

BOARD:em.avnet.com:ultrazed_eg_iocc_production:part0:1.0
IP NAME: ultrazed_eg_iocc_production_1 IP: (em.avnet.com:ultrazed_eg_iocc_production:part0:1.0)

Prerequisites
=============
1. Download and Install Vivado tools from https://www.xilinx.com/support/download.html
2. Make sure you have applied license to install tools.

Steps to Build Vivado Design Project
====================================
1. Clone this git repo with release version branch which matches your vivado version.
2. Launch the Vivado tools
3. On the Tcl Console window run below command to set the Ultrazed board files
   set_param board.repoPaths <git_repo_avnet_uz3eg_iocc_hw_design>/board_files/ultrazed_3eg_iocc/1.0
4. Source the project tcl files, This will create a IOCC DP(display port) design and generate 
   the bitstream.
   source ./<git_repo_avnet_uz3eg_iocc_hw_design>/avnet_uz3eg_iocc_dp.tcl
5. Once the bitstream generation is complete you can export the hdf
   File ---> Export ---> Export Hardware ---> [*] Include bitstream
