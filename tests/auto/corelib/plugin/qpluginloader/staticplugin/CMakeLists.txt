# Generated from staticplugin.pro.

#####################################################################
## staticplugin Generic Library:
#####################################################################

add_cmake_library(staticplugin
    STATIC
    SOURCES
        main.cpp
    PUBLIC_LIBRARIES
        Qt::Core
    MOC_OPTIONS
        "-M"
        "ExtraMetaData=StaticPlugin"
        "-M"
        "ExtraMetaData=foo"
)

#### Keys ignored in scope 1:.:.:staticplugin.pro:<TRUE>:
# TEMPLATE = "lib"

qt_autogen_tools_initial_setup(staticplugin)

target_compile_definitions(staticplugin PRIVATE QT_STATICPLUGIN)
