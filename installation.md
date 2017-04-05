# INSTALLATION INSTRUCTIONS

## [Installation of PIPS-NLP and Julia/StructJuMP](structjump.md)

## Building PIPS-S only can be achieved via 
1. cmake -DBUILD_ALL=OFF -DBUILD_PIPS_S=ON <path_to_CMakeLists.txt>
or 
2. including "set(BUILD_ALL OFF); set(BUILD_PIPS_S ON)" in a toolchain file, then 
invoking
cmake -DCMAKE_TOOLCHAIN_FILE=<path_to_toolchain_file> <path_to_CMakeLists.txt>

Same applies to PIPS-IPM and PIPS-NLP (option names BUILD_PIPS_IPM and BUILD_PIPS_NLP, 
respectively).

## General installation instructions
1. Install package wget, cmake, mpich2, and boost.
You can get them via the following command (xxx stands for the name of the package):
In Linux(Ubuntu): apt-get install xxxx

2. Go to the following folders and run the script wgetXXX.sh
ThirdPartyLibs/ASL  
ThirdPartyLibs/CBC 
ThirdPartyLibs/ConicBundle   
ThirdPartyLibs/METIS
For an example, use command "sh wgetASL.sh" in the folder ThirdPartyLibs/ASL  

3. Download MA27 and MA57 from HSL and put the source code in the correct folder. 
(See ThirdPartyLibs/MA27/README.txt and ThirdPartyLibs/MA57/README.txt for more details.)

4. Assuming we are trying to install PIPS in the folder PIPSMAINPATH/build_pips, where 
PIPSMAINPATH is the root installation folder, use the following commands in the PIPSMAINPATH
folder to configure and install PIPS:
mkdir build_pips
cd build_pips
cmake ..
make

5. The build system will install executables from three sources: PIPS-IPM, PIPS-S and PIPS-NLP. 
