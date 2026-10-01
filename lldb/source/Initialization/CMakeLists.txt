add_lldb_library(lldbInitialization NO_PLUGIN_DEPENDENCIES
  SystemInitializerCommon.cpp
  SystemInitializer.cpp
  SystemLifetimeManager.cpp

  ADDITIONAL_HEADER_DIRS
    ${LLDB_INCLUDE_DIR}/lldb/Initialization
  LINK_COMPONENTS
    Support
  LINK_LIBS
    lldbCore
    lldbHost
    lldbUtility
    ${LLDB_SYSTEM_LIBS}
  )
