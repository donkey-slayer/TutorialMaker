cmake_minimum_required(VERSION 3.16.3...3.19.7 FATAL_ERROR)

project(Tutorial Maker)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/TutorialMaker")
set(EXTENSION_CATEGORY "Utilities")
set(EXTENSION_CONTRIBUTORS "John Doe (AnyWare Corp.)")
set(EXTENSION_DESCRIPTION "Vamo fazer tutorial")
set(EXTENSION_ICONURL "https://www.example.com/Slicer/Extensions/TutorialMaker.png")
set(EXTENSION_SCREENSHOTURLS "https://www.example.com/Slicer/Extensions/TutorialMaker/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(TutorialMaker)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
