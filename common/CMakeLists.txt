set(
  SOURCES
    "src/window.cpp"
    "include/window.hpp"
)

add_library(mimic_common ${SOURCES})
target_include_directories(mimic_common PUBLIC "include")
target_compile_features(mimic_common PUBLIC "cxx_std_14")

install(
  TARGETS mimic_common
  ARCHIVE DESTINATION lib
  LIBRARY DESTINATION lib
  RUNTIME DESTINATION bin
)