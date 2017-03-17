##################################################################################
#        License                                                                 #
##################################################################################
#        This file is a part of the CineFX project.                              #
#        Copyright (C) 2017 Florian DUFOUR                                       #
#                                                                                #
#        This program is free software; you can redistribute it and/or modify    #
#        it under the terms of the GNU General Public License as published by    #
#        the Free Software Foundation; either version 3 of the License, or       #
#        (at your option) any later version.                                     #
#                                                                                #
#        This program is distributed in the hope that it will be useful,         #
#        but WITHOUT ANY WARRANTY; without even the implied warranty of          #
#        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the           #
#        GNU General Public License for more details.                            #
#                                                                                #
#        You should have received a copy of the GNU General Public License       #
#        along with this program; if not, write to the Free Software Foundation, #
#        Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA       #
#                                                                                #
##################################################################################

cmake_minimum_required(VERSION 3.6)

##################################################################################
# setup
##################################################################################

project(cinefx-framework)

set (PROJECT_VER_MAJOR 0)
set (PROJECT_VER_MAJOR 1)
set (PROJET_VER_PATCH 0 )

set (PROJECT_VER
  "${PROJECT_VER_MAJOR}.${PROJECT_VER_MINOR}.${PROJECT_VER_PATCH}")
set (PROJECT_APIVER
  "${PROJECT_VER_MAJOR}.${PROJECT_VER_MINOR}")

OPTION (BUILD_RENDER_EXTERNAL "Build the render for external use" ON)
OPTION (BUILD_CINEFX "Build the CineFX software" ON)
OPTION (BUILD_ADDONS_CINEFX "Build Addons for CineFX" ON)
OPTION (BUILD_ADDONS_EXTERNAL "Build addons for other programme" OFF)

##################################################################################
# CMake
##################################################################################

add_subdirectory(src)
