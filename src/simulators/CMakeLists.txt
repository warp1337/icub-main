# Copyright: (C) 2009,2010 RobotCub Consortium
# Authors: Lorenzo Natale
# CopyPolicy: Released under the terms of the GNU GPL v2.0.

add_subdirectory(simCartesianControl)

if(ICUB_USE_ODE AND ICUB_USE_SDL)
	add_subdirectory(iCubSimulation)
	add_subdirectory(simFaceExpressions)
else(ICUB_USE_ODE AND ICUB_USE_SDL)
	message(STATUS "ODE or SDL not found/selected, skipping iCubSimulation and simFaceExpressions")
endif(ICUB_USE_ODE AND ICUB_USE_SDL)


