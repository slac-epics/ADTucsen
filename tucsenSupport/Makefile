TOP=..
include $(TOP)/configure/CONFIG
#----------------------------------------
#  ADD MACRO DEFINITIONS AFTER THIS LINE
#=============================

# Note, the files in this directory were manually copied from the Andor SDK3 directories 
# for Linux and Windows.  The soft links for Linux were manually created.

INC += TUCamApi.h TUDefine.h

ifeq (windows-x64, $(findstring windows-x64, $(T_A)))
ifneq ($(TUCAM_EXTERNAL),YES)
LIB_INSTALLS_WIN32    += ../os/windows-x64/TUCam.lib
BIN_INSTALLS_WIN32    += ../os/windows-x64/TUCam.dll
endif
endif

ifeq (x86_64, $(findstring x86_64, $(T_A)))
ifneq ($(TUCAM_EXTERNAL),YES)
LIB_INSTALLS_Linux += ../os/linux-x86_64/libTUCam.so
LIB_INSTALLS_Linux += ../os/linux-x86_64/libTUCam.so.1
LIB_INSTALLS_Linux += ../os/linux-x86_64/libTUCam.so.1.0
LIB_INSTALLS_Linux += ../os/linux-x86_64/libTUCam.so.1.0.0
LIB_INSTALLS_Linux += ../os/linux-x86_64/coaxlink.cti
LIB_INSTALLS_Linux += ../os/linux-x86_64/libGCBase_gcc421_v3_0.so
LIB_INSTALLS_Linux += ../os/linux-x86_64/libGenApi_gcc421_v3_0.so
LIB_INSTALLS_Linux += ../os/linux-x86_64/libKYFGLibGenTL.cti
LIB_INSTALLS_Linux += ../os/linux-x86_64/liblog4cpp_gcc421_v3_0.so
LIB_INSTALLS_Linux += ../os/linux-x86_64/libLog_gcc421_v3_0.so
LIB_INSTALLS_Linux += ../os/linux-x86_64/libMathParser_gcc421_v3_0.so
LIB_INSTALLS_Linux += ../os/linux-x86_64/libNodeMapData_gcc421_v3_0.so
LIB_INSTALLS_Linux += ../os/linux-x86_64/libXmlParser_gcc421_v3_0.so
endif
endif

#=============================

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE

