############################################################################
#
#   Copyright (c) 2015 ECL Development Team. All rights reserved.
#
# Redistribution and use in source and binary forms, with or without
# modification, are permitted provided that the following conditions
# are met:
#
# 1. Redistributions of source code must retain the above copyright
#    notice, this list of conditions and the following disclaimer.
# 2. Redistributions in binary form must reproduce the above copyright
#    notice, this list of conditions and the following disclaimer in
#    the documentation and/or other materials provided with the
#    distribution.
# 3. Neither the name ECL nor the names of its contributors may be
#    used to endorse or promote products derived from this software
#    without specific prior written permission.
#
# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
# COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
# INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS
# OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED
# AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
# ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
# POSSIBILITY OF SUCH DAMAGE.
#
############################################################################
include_directories(.)
px4_add_library(ecl
	airdata/WindEstimator.cpp
	attitude_fw/ecl_controller.cpp
	attitude_fw/ecl_pitch_controller.cpp
	attitude_fw/ecl_roll_controller.cpp
	attitude_fw/ecl_wheel_controller.cpp
	attitude_fw/ecl_yaw_controller.cpp
	EKF/airspeed_fusion.cpp
	EKF/control.cpp
	EKF/covariance.cpp
	EKF/drag_fusion.cpp
	EKF/ekf.cpp
	EKF/ekf_helper.cpp
	EKF/estimator_interface.cpp
	EKF/gps_checks.cpp
	EKF/mag_fusion.cpp
	EKF/optflow_fusion.cpp
	EKF/sideslip_fusion.cpp
	EKF/terrain_estimator.cpp
	EKF/vel_pos_fusion.cpp
	geo/geo.cpp
	geo_lookup/geo_mag_declination.cpp
	l1/ecl_l1_pos_controller.cpp
	tecs/tecs.cpp
	validation/data_validator.cpp
	validation/data_validator_group.cpp
	)
