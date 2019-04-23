set(mapnik_plugin_geojson_sources
    geojson_datasource.cpp
    geojson_featureset.cpp
    geojson_index_featureset.cpp
    geojson_memory_index_featureset.cpp
    )

# boost
set(Boost_USE_STATIC_LIBS OFF)
set(Boost_USE_STATIC_RUNTIME OFF)
find_package(Boost REQUIRED COMPONENTS system)
include_directories(${Boost_INCLUDE_DIRS})
add_definitions(-DBoost_LIB_DIAGNOSTIC_DEFINITIONS -DBOOST_ALL_DYN_LINK -DBOOST_ALL_NO_LIB)
list(APPEND mapnik_plugin_geojson_libraries ${Boost_LIBRARIES})
get_filename_component(boost_binary_directories ${Boost_INCLUDE_DIRS}/../bin ABSOLUTE)
list(APPEND mapnik_plugin_geojson_binary_directories ${boost_binary_directories})

# ICU
find_package(ICU REQUIRED)
include_directories(${ICU_INCLUDE_DIRS})
list(APPEND mapnik_plugin_geojson_libraries ${ICU_LIBRARIES})
get_filename_component(icu_binary_directories ${ICU_INCLUDE_DIRS}/../bin ABSOLUTE)
list(APPEND mapnik_plugin_geojson_binary_directories ${icu_binary_directories})

include_directories(
    ${mapnik_SOURCE_DIR}/deps/mapbox/geometry/include
    )

add_library(geojson MODULE ${mapnik_plugin_geojson_sources})

set_target_properties(geojson PROPERTIES SUFFIX ".input")

target_link_libraries(geojson ${mapnik_plugin_geojson_libraries} mapnik)

install(TARGETS geojson LIBRARY DESTINATION "bin/${CMAKE_BUILD_TYPE}/mapnik/input")

set(MAPNIK_PLUGINS ${MAPNIK_PLUGINS} ${CMAKE_INSTALL_PREFIX}/bin/${CMAKE_BUILD_TYPE}/mapnik/input/geojson.input PARENT_SCOPE)
set(MAPNIK_BINARY_DIRECTORIES ${MAPNIK_BINARY_DIRECTORIES} ${mapnik_plugin_geojson_binary_directories} ${CMAKE_CURRENT_BINARY_DIR} PARENT_SCOPE)