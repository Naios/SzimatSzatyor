#   This file is part of SzimatSzatyor.
#
#   SzimatSzatyor is free software: you can redistribute it and/or modify
#   it under the terms of the GNU General Public License as published by
#   the Free Software Foundation, either version 3 of the License, or
#   (at your option) any later version.
#
#   SzimatSzatyor is distributed in the hope that it will be useful,
#   but WITHOUT ANY WARRANTY; without even the implied warranty of
#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
#   GNU General Public License for more details.
#
#   You should have received a copy of the GNU General Public License
#   along with SzimatSzatyor.  If not, see <http://www.gnu.org/licenses/>.

add_executable(szatyor
    main.cpp
)

include_directories(
    ${SZIMAT_SZATYOR_SHARED_HEADERS}
)

target_link_libraries(szatyor
    shared
    Psapi
    shlwapi
    version
)
