### Use fmm in your own project.

1. Copy the `find_fmm.cmake` file to a folder cmake of your repo.

```
list(APPEND CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")
find_package(FMM REQUIRED)
```

Check the finding result

```
if(NOT FMM_FOUND)
    message(WARNING "FMM not found!\n")
endif()
include_directories(${FMM_INCLUDE_DIRS})
```
