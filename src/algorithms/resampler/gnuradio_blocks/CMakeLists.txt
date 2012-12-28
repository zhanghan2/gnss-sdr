# Copyright (C) 2012-2013  (see AUTHORS file for a list of contributors)
#
# This file is part of GNSS-SDR.
#
# GNSS-SDR is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# at your option) any later version.
#
# GNSS-SDR is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with GNSS-SDR. If not, see <http://www.gnu.org/licenses/>.
#


set(RESAMPLER_GR_BLOCKS_SOURCES 
     direct_resampler_conditioner_cc.cc
#    direct_resampler_conditioner_ss.cc
)

include_directories(
     $(CMAKE_CURRENT_SOURCE_DIR)
     ${GNURADIO_CORE_INCLUDE_DIRS}
     ${GNURADIO_GRUEL_INCLUDE_DIRS}
)

add_library(resampler_gr_blocks ${RESAMPLER_GR_BLOCKS_SOURCES})