# Copyright (c) 2014-2018 LG Electronics, Inc.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
# SPDX-License-Identifier: Apache-2.0

set(moduleName ${NYX_CMD_MODULE_PREFIX}Charger)
add_library(${moduleName} SHARED nyx_cmd_charger.cpp nyx_cmd_charger_query.cpp nyx_cmd_charger_register.cpp)
target_link_libraries(${moduleName} ${NYXLIB_LDFLAGS})
nyx_cmd_install_library(${moduleName})
