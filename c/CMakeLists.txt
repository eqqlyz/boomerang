SET(boomerang_DSLs_sources
    ansi-c-parser.cpp
    ansi-c-scanner.cpp
ansi-c-parser.h
ansi-c-scanner.h
)
ADD_LIBRARY(boomerang_DSLs STATIC ${boomerang_DSLs_sources} )
qt5_use_modules(boomerang_DSLs Core)

IF(BUILD_TESTING)
ADD_SUBDIRECTORY(unit_testing)
ENDIF()
