# Copyright (c) 2014-present, The osquery authors
#
# This source code is licensed as defined by the LICENSE file found in the
# root directory of this source tree.
#
# SPDX-License-Identifier: (Apache-2.0 OR GPL-2.0-only)

function(rapidjsonMain)
  set(library_root "${CMAKE_CURRENT_SOURCE_DIR}/src")

  add_library(thirdparty_rapidjson INTERFACE)
  target_include_directories(thirdparty_rapidjson SYSTEM INTERFACE
    "${library_root}/include"
  )
endfunction()

rapidjsonMain()
