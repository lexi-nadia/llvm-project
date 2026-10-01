add_lldb_library(lldbPluginProcessPOSIX
  CrashReason.cpp
  NativeProcessELF.cpp

  LINK_COMPONENTS
    Support
  LINK_LIBS
    lldbPluginProcessUtility
    lldbUtility
  )
