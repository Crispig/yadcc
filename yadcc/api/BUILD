# Copyright (C) 2020 THL A29 Limited, a Tencent company. All rights reserved.
#
# Licensed under the BSD 3-Clause License (the "License"); you may not use this
# file except in compliance with the License. You may obtain a copy of the
# License at
#
# https://opensource.org/licenses/BSD-3-Clause
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
# License for the specific language governing permissions and limitations under
# the License.

load('//flare/tools/build_rules.bld', 'cc_flare_library')

proto_library(
  name = 'env_desc_proto',
  srcs = 'env_desc.proto',
  visibility = 'PUBLIC',
)

proto_library(
  name = 'daemon_proto',
  srcs = 'daemon.proto',
  deps = [
    ':env_desc_proto',
  ],
  visibility = 'PUBLIC',
)

cc_flare_library(
  name = 'daemon_proto_flare',
  srcs = 'daemon.proto',
  deps = [
    ':daemon_proto',
  ],
  visibility = 'PUBLIC',
)

proto_library(
  name = 'scheduler_proto',
  srcs = 'scheduler.proto',
  deps = [
    ':env_desc_proto',
  ],
  visibility = 'PUBLIC',
)

cc_flare_library(
  name = 'scheduler_proto_flare',
  srcs = 'scheduler.proto',
  deps = [
    ':scheduler_proto',
  ],
  visibility = 'PUBLIC',
)

proto_library(
  name = 'cache_proto',
  srcs = 'cache.proto',
  visibility = 'PUBLIC',
)

cc_flare_library(
  name = 'cache_proto_flare',
  srcs = 'cache.proto',
  deps = [
    ':cache_proto',
  ],
  visibility = 'PUBLIC',
)
