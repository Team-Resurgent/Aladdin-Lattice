# Aladdin XT CPLD mods

This package contains HDL projects to program the Aladdin XT PLUS2 clone devices.

You will require Lattice ISPLever Classic software suite (version 2.0 at the time of writing) to generate programming files.
Constraint files included in each projects interface the Aladdin XT PLUS2 PCB exclusively.
All designs require the use of internal pullups of the LC4032V CPLD to operate properly.

Projects:

**1MB_LPCmod_OSSupport**
    
    Support 1MB SST49LF080A device and gives support to XBlast OS to manage user flash banks. Split in 1 * 512KB and 1 * 256KB user banks. 
    Last 256KB bank is reserved for XBlast OS. Uses L1 + D0 for LFrame and D0 respectivly.
    
**1MB_LPCmod_OSSupport_MosfetD0**
    
    Support 1MB SST49LF080A device and gives support to XBlast OS to manage user flash banks. Split in 1 * 512KB and 1 * 256KB user banks. 
    Last 256KB bank is reserved for XBlast OS. Uses D0 for either LFrame or D0.

**2MB_LPCmod_OSSupport**
    
    Support 2MB SST49LF160C device and gives support to PrometheOS to manage user flash banks. Split in 4 * 256KB or 2 * 512KB or 1 * 1024KB user banks. 
    Last 1024KB is divided into 4 * 256KB banks and is reserved for PrometheOS. Uses L1 + D0 for LFrame and D0 respectivly.
    
**2MB_LPCmod_OSSupport_MosfetD0**
    
    Support 2MB SST49LF160C device and gives support to PrometheOS to manage user flash banks. Split in 4 * 256KB or 2 * 512KB or 1 * 1024KB user banks. 
    Last 1024KB is divided into 4 * 256KB banks and is reserved for PrometheOS. Uses D0 for either LFrame or D0.

Other files include images of JTAG interface on board and a table of pin mappings between the LC4032V CPLD, Flash chip and LPC interface.

Have fun.