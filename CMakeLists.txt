cmake_minimum_required(VERSION 3.13.4)

project(ALIIOS)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/ALIIOS")
set(EXTENSION_CATEGORY "Landmarks")
set(EXTENSION_CONTRIBUTORS "John Doe (AnyWare Corp.)")
set(EXTENSION_DESCRIPTION "Extension for automatic landmarks identification on intra oral scans ")
set(EXTENSION_ICONURL "http://www.example.com/Slicer/Extensions/ALIIOS.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/ALIIOS/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(ALIIOS)
add_subdirectory(ALIIOS_CLI)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
