set(mapnik_sources
    box2d.cpp
    cairo_io.cpp
    color.cpp
    color_factory.cpp
    config_error.cpp
    conversions.cpp
    css_color_grammar.cpp
    dasharray_parser.cpp
    datasource_cache.cpp
    datasource_cache_static.cpp
    debug.cpp
    expression.cpp
    expression_grammar.cpp
    expression_node.cpp
    expression_string.cpp
    feature_kv_iterator.cpp
    feature_style_processor.cpp
    feature_type_style.cpp
    font_engine_freetype.cpp
    font_set.cpp
    fs.cpp
    function_call.cpp
    geometry_envelope.cpp
    geometry_reprojection.cpp
    glibc_workaround.cpp
    gradient.cpp
    image.cpp
    image_any.cpp
    image_compositing.cpp
    image_copy.cpp
    image_filter_grammar.cpp
    image_filter_types.cpp
    image_options.cpp
    image_reader.cpp
    image_scaling.cpp
    image_util.cpp
    image_util_jpeg.cpp
    image_util_png.cpp
    image_util_tiff.cpp
    image_util_webp.cpp
    image_view.cpp
    image_view_any.cpp
    jpeg_reader.cpp
    layer.cpp
    load_map.cpp
    map.cpp
    mapped_memory_cache.cpp
    marker_cache.cpp
    marker_helpers.cpp
    math.cpp
    memory_datasource.cpp
    palette.cpp
    params.cpp
    parse_path.cpp
    parse_transform.cpp
    plugin.cpp
    png_reader.cpp
    proj_transform.cpp
    projection.cpp
    raster_colorizer.cpp
    renderer_common.cpp
    request.cpp
    rule.cpp
    save_map.cpp
    scale_denominator.cpp
    simplify.cpp
    symbolizer.cpp
    symbolizer_enumerations.cpp
    symbolizer_keys.cpp
    tiff_reader.cpp
    transform_expression.cpp
    transform_expression_grammar.cpp
    twkb.cpp
    unicode.cpp
    value.cpp
    vertex_adapters.cpp
    vertex_cache.cpp
    warp.cpp
    webp_reader.cpp
    well_known_srs.cpp
    wkb.cpp
    xml_tree.cpp

    geometry/interior.cpp

    util/utf_conv_win.cpp

    # JSON
    json/generic_json.cpp
    json/mapnik_geometry_to_geojson.cpp
    json/mapnik_json_feature_collection_grammar.cpp
    json/mapnik_json_feature_grammar.cpp
    json/mapnik_json_generator_grammar.cpp
    json/mapnik_json_geometry_grammar.cpp
    json/mapnik_json_geometry_parser.cpp
    json/mapnik_json_positions_grammar.cpp
    json/mapnik_topojson_grammar.cpp
    
    # Text placements
    text/face.cpp
    text/font_feature_settings.cpp
    text/font_library.cpp
    text/glyph_positions.cpp
    text/itemizer.cpp
    text/placement_finder.cpp
    text/properties_util.cpp
    text/renderer.cpp
    text/scrptrun.cpp
    text/symbolizer_helpers.cpp
    text/text_layout.cpp
    text/text_line.cpp
    text/text_properties.cpp

    text/placements/base.cpp
    text/placements/dummy.cpp
    text/placements/list.cpp
    text/placements/registry.cpp
    text/placements/simple.cpp
    

    text/formatting/base.cpp
    text/formatting/format.cpp
    text/formatting/layout.cpp
    text/formatting/list.cpp
    text/formatting/registry.cpp
    text/formatting/text.cpp
    
    # WKT
    wkt/mapnik_wkt_generator_grammar.cpp
    wkt/mapnik_wkt_grammar.cpp
    
    # AGG
    agg/agg_renderer.cpp
    agg/process_building_symbolizer.cpp
    agg/process_debug_symbolizer.cpp
    agg/process_dot_symbolizer.cpp
    agg/process_group_symbolizer.cpp
    agg/process_line_pattern_symbolizer.cpp
    agg/process_line_symbolizer.cpp
    agg/process_markers_symbolizer.cpp
    agg/process_point_symbolizer.cpp
    agg/process_polygon_pattern_symbolizer.cpp
    agg/process_polygon_symbolizer.cpp
    agg/process_raster_symbolizer.cpp
    agg/process_shield_symbolizer.cpp
    agg/process_text_symbolizer.cpp
    ..//deps//agg//src//agg_arc.cpp
    ..//deps//agg//src//agg_arrowhead.cpp
    ..//deps//agg//src//agg_bezier_arc.cpp
    ..//deps//agg//src//agg_bspline.cpp
    ..//deps//agg//src//agg_curves.cpp
    ..//deps//agg//src//agg_embedded_raster_fonts.cpp
    ..//deps//agg//src//agg_gsv_text.cpp
    ..//deps//agg//src//agg_image_filters.cpp
    ..//deps//agg//src//agg_line_aa_basics.cpp
    ..//deps//agg//src//agg_line_profile_aa.cpp
    ..//deps//agg//src//agg_pixfmt_rgba.cpp
    ..//deps//agg//src//agg_rounded_rect.cpp
    ..//deps//agg//src//agg_sqrt_tables.cpp
    ..//deps//agg//src//agg_trans_affine.cpp
    ..//deps//agg//src//agg_trans_double_path.cpp
    ..//deps//agg//src//agg_trans_single_path.cpp
    ..//deps//agg//src//agg_trans_warp_magnifier.cpp
    ..//deps//agg//src//agg_vcgen_bspline.cpp
    ..//deps//agg//src//agg_vcgen_contour.cpp
    ..//deps//agg//src//agg_vcgen_dash.cpp
    ..//deps//agg//src//agg_vcgen_markers_term.cpp
    ..//deps//agg//src//agg_vcgen_smooth_poly1.cpp
    ..//deps//agg//src//agg_vcgen_stroke.cpp
    ..//deps//agg//src//agg_vpgen_clip_polygon.cpp
    ..//deps//agg//src//agg_vpgen_clip_polyline.cpp
    ..//deps//agg//src//agg_vpgen_segmentator.cpp

    # # clipper
    # ../deps/clipper/src/clipper.cpp
    
    # grid
    grid/grid.cpp
    grid/grid_renderer.cpp
    grid/process_building_symbolizer.cpp
    grid/process_group_symbolizer.cpp
    grid/process_line_pattern_symbolizer.cpp
    grid/process_line_symbolizer.cpp
    grid/process_markers_symbolizer.cpp
    grid/process_point_symbolizer.cpp
    grid/process_polygon_pattern_symbolizer.cpp
    grid/process_polygon_symbolizer.cpp
    grid/process_raster_symbolizer.cpp
    grid/process_shield_symbolizer.cpp
    grid/process_text_symbolizer.cpp

    renderer_common/pattern_alignment.cpp
    renderer_common/render_group_symbolizer.cpp
    renderer_common/render_markers_symbolizer.cpp
    renderer_common/render_pattern.cpp
    renderer_common/render_thunk_extractor.cpp


    group/group_layout_manager.cpp
    group/group_rule.cpp
    group/group_symbolizer_helper.cpp
    
    # (mandatory) SVG
    svg/svg_parser.cpp
    svg/svg_path_parser.cpp
    svg/svg_points_parser.cpp
    svg/svg_transform_parser.cpp
)

set(binary_directories ${MAPNIK_BINARY_DIRECTORIES})

# boost
set(Boost_USE_STATIC_LIBS OFF)
set(Boost_USE_STATIC_RUNTIME OFF)
find_package(Boost REQUIRED COMPONENTS chrono date_time filesystem regex system thread)
set_package_properties(Boost PROPERTIES
    DESCRIPTION "Portable C++ source libraries"
    URL "http://www.boost.org/"
    TYPE REQUIRED
    PURPOSE "Required for all core operations.")
include_directories(${Boost_INCLUDE_DIRS})
add_definitions(-DBoost_LIB_DIAGNOSTIC_DEFINITIONS -DBOOST_ALL_DYN_LINK -DBOOST_ALL_NO_LIB)
list(APPEND mapnik_libraries ${Boost_LIBRARIES})
get_filename_component(boost_binary_directories ${Boost_INCLUDE_DIRS}/../bin ABSOLUTE)
list(APPEND binary_directories ${boost_binary_directories})

# ICU
set(icu_components uc)

# Check whether the boost libary uses ICU.
include(CheckCXXSourceRuns)

find_package(ICU REQUIRED COMPONENTS uc i18n)

set(CMAKE_REQUIRED_LIBRARIES ${ICU_LIBRARIES})

if (CMAKE_BUILD_TYPE EQUAL "Debug")
    list(APPEND CMAKE_REQUIRED_LIBRARIES ${Boost_REGEX_LIBRARY_DEBUG})
else (CMAKE_BUILD_TYPE EQUAL "Debug")
    list(APPEND CMAKE_REQUIRED_LIBRARIES ${Boost_REGEX_LIBRARY_RELEASE})
endif (CMAKE_BUILD_TYPE EQUAL "Debug")

set(CMAKE_REQUIRED_DEFINITIONS -DBOOST_ALL_DYN_LINK -DBOOST_ALL_NO_LIB)
set(CMAKE_REQUIRED_INCLUDES ${Boost_INCLUDE_DIRS} ${ICU_INCLUDE_DIRS})
file(READ ${CMAKE_MODULE_PATH}/CheckBoostRegexIcu.cpp CheckBoostRegexIcuSource)
CHECK_CXX_SOURCE_RUNS("${CheckBoostRegexIcuSource}" BOOST_REGEX_HAS_ICU)

if (BOOST_REGEX_HAS_ICU)
    list(APPEND icu_components i18n)
endif (BOOST_REGEX_HAS_ICU)

find_package(ICU REQUIRED COMPONENTS ${icu_components})
set_package_properties(ICU PROPERTIES
    DESCRIPTION "Unicode and Globalization support library"
    URL "http://site.icu-project.org/"
    TYPE REQUIRED
    PURPOSE "Required for text conversions.")
include_directories(${ICU_INCLUDE_DIRS})
list(APPEND mapnik_libraries ${ICU_LIBRARIES})
get_filename_component(icu_binary_directories ${ICU_INCLUDE_DIRS}/../bin ABSOLUTE)
list(APPEND binary_directories ${icu_binary_directories})

# iconv
find_package(ICONV REQUIRED)
set_package_properties(ICONV PROPERTIES
    DESCRIPTION "String conversion library"
    URL "http://www.gnu.org/software/libiconv/"
    TYPE REQUIRED
    PURPOSE "Required for text conversions (also dependency for some libraries).")
include_directories(${ICONV_INCLUDE_DIR})
list(APPEND mapnik_libraries ${ICONV_LIBRARY})
get_filename_component(iconv_binary_directories ${ICONV_INCLUDE_DIR}/../bin ABSOLUTE)
list(APPEND binary_directories ${iconv_binary_directories})

# zlib
find_package(ZLIB REQUIRED)
set_package_properties(ZLIB PROPERTIES
    DESCRIPTION "Compression library"
    URL "http://www.zlib.net/"
    TYPE REQUIRED
    PURPOSE "Required for processing compressed material (also dependency for some libraries).")
include_directories(${ZLIB_INCLUDE_DIRS})
list(APPEND mapnik_libraries ${ZLIB_LIBRARIES})
get_filename_component(zlib_binary_directories ${ZLIB_INCLUDE_DIRS}/../bin ABSOLUTE)
list(APPEND binary_directories ${zlib_binary_directories})

# freetype
find_package(Freetype REQUIRED)
set_package_properties(Freetype PROPERTIES
    DESCRIPTION "Font rendering library"
    URL "http://www.freetype.org/"
    TYPE REQUIRED
    PURPOSE "Required for all font rendering.")
include_directories(${FREETYPE_INCLUDE_DIRS})
list(APPEND mapnik_libraries ${FREETYPE_LIBRARIES})
get_filename_component(freetype_binary_directories ${FREETYPE_LIBRARY}/../../bin ABSOLUTE)
list(APPEND binary_directories ${freetype_binary_directories})

# proj.4
find_package(Proj REQUIRED)
set_package_properties(Proj PROPERTIES
    DESCRIPTION "Cartographic Projections library"
    URL "https://trac.osgeo.org/proj/"
    TYPE REQUIRED
    PURPOSE "Required for all projection transformations.")
include_directories(${PROJ_INCLUDE_DIR})
add_definitions(-DMAPNIK_USE_PROJ4)
list(APPEND mapnik_libraries ${PROJ_LIBRARY})
get_filename_component(proj_binary_directories ${PROJ_INCLUDE_DIR}/../bin ABSOLUTE)
list(APPEND binary_directories ${proj_binary_directories})

# JPEG
find_package(JPEG)
set_package_properties(JPEG PROPERTIES
    DESCRIPTION "JPEG library"
    URL "http://www.ijg.org/"
    TYPE RECOMMENDED
    PURPOSE "Enables using JPEG images.")
if (USE_JPEG AND JPEG_FOUND)
    list(APPEND mapnik_sources jpeg_reader.cpp)
    include_directories(${JPEG_INCLUDE_DIR})
    list(APPEND mapnik_libraries ${JPEG_LIBRARIES})
    get_filename_component(jpeg_binary_directories ${JPEG_INCLUDE_DIR}/../bin ABSOLUTE)
    list(APPEND binary_directories ${jpeg_binary_directories})
endif (USE_JPEG AND JPEG_FOUND)

# PNG
find_package(PNG)
set_package_properties(PNG PROPERTIES
    DESCRIPTION "Portable Network Graphics library"
    URL "http://www.libpng.org/"
    TYPE RECOMMENDED
    PURPOSE "Enables using PNG images.")
if (USE_PNG AND PNG_FOUND)
    list(APPEND mapnik_sources png_reader.cpp)
    include_directories(${PNG_INCLUDE_DIRS})
    add_definitions(${PNG_DEFINITIONS})
    list(APPEND mapnik_libraries ${PNG_LIBRARIES})
    get_filename_component(png_binary_directories ${PNG_LIBRARY}/../../bin ABSOLUTE)
    list(APPEND binary_directories ${png_binary_directories})
endif (USE_PNG AND PNG_FOUND)

# TIFF
find_package(TIFF)
set_package_properties(TIFF PROPERTIES
    DESCRIPTION "TIFF library"
    URL "http://www.libtiff.org/"
    TYPE RECOMMENDED
    PURPOSE "Enables using TIFF images.")

if (USE_TIFF AND TIFF_FOUND)
    list(APPEND mapnik_sources tiff_reader.cpp)
    include_directories(${TIFF_INCLUDE_DIR})
    list(APPEND mapnik_libraries ${TIFF_LIBRARIES})
    get_filename_component(tiff_binary_directories ${TIFF_INCLUDE_DIR}/../bin ABSOLUTE)
    list(APPEND binary_directories ${tiff_binary_directories})
endif (USE_TIFF AND TIFF_FOUND)

# SVG
if (USE_SVG)
    list(APPEND mapnik_sources
        svg/output/process_line_symbolizer.cpp
        svg/output/process_polygon_symbolizer.cpp
        svg/output/process_symbolizers.cpp
        svg/output/svg_generator.cpp
        svg/output/svg_output_attributes.cpp
        svg/output/svg_output_grammars.cpp
        svg/output/svg_renderer.cpp)
    add_definitions(-DSVG_RENDERER)
endif (USE_SVG)

# libxml2
find_package(LibXml2)
set_package_properties(LibXml2 PROPERTIES
    DESCRIPTION "XML processing library"
    URL "http://xmlsoft.org/"
    TYPE RECOMMENDED
    PURPOSE "Enables more extensive XML support.")

if (USE_LIBXML2 AND LIBXML2_FOUND)
    list(APPEND mapnik_sources libxml2_loader.cpp)
    include_directories(${LIBXML2_INCLUDE_DIR})
    add_definitions(${LIBXML2_DEFINITIONS} -DHAVE_LIBXML2)
    list(APPEND mapnik_libraries ${LIBXML2_LIBRARIES})
    get_filename_component(xml2_binary_directories ${LIBXML2_LIBRARIES}/../../bin ABSOLUTE)
    list(APPEND binary_directories ${xml2_binary_directories})
else(USE_LIBXML2 AND LIBXML2_FOUND)
    list(APPEND mapnik_sources rapidxml_loader.cpp)
endif (USE_LIBXML2 AND LIBXML2_FOUND)

# cairo
find_package(Cairo)
set_package_properties(Cairo PROPERTIES
    DESCRIPTION "2D graphics library with support for multiple output devices"
    URL "http://www.cairographics.org/"
    TYPE OPTIONAL
    PURPOSE "Enables rendering with the cairo library.")

if (USE_CAIRO AND CAIRO_FOUND)
    # Cairo dependencies
    find_package(FontConfig REQUIRED)
    list(APPEND mapnik_sources
        cairo_context.cpp
        cairo_renderer.cpp)
    include_directories(${CAIRO_INCLUDE_DIRS} ${FONTCONFIG_INCLUDE_DIR})
    add_definitions(-DHAVE_CAIRO)
    list(APPEND mapnik_libraries ${CAIRO_LIBRARIES} ${FONTCONFIG_LIBRARIES})
    get_filename_component(fontconfig_binary_directories ${FONTCONFIG_LIBRARIES}/../../bin ABSOLUTE)
    get_filename_component(cairo_binary_directories ${CAIRO_LIBRARIES}/../../bin ABSOLUTE)
    list(APPEND binary_directories ${fontconfig_binary_directories} ${cairo_binary_directories})
endif (USE_CAIRO AND CAIRO_FOUND)

add_definitions(-DMAPNIK_EXPORTS)

# Create the mapnik library
add_library(mapnik SHARED ${mapnik_sources})

target_link_libraries(mapnik ${mapnik_libraries})

# Create install rules
install(TARGETS mapnik RUNTIME DESTINATION "bin/${CMAKE_BUILD_TYPE}")
install(TARGETS mapnik ARCHIVE DESTINATION "lib/MSVC/${CMAKE_BUILD_TYPE}")
# For windows we need the extension to be same as executables for BundleUtilities
if (WIN32)
    install(
        FILES ${CMAKE_INSTALL_PREFIX}/bin/${CMAKE_BUILD_TYPE}/mapnik${CMAKE_SHARED_LIBRARY_SUFFIX}
        DESTINATION "bin/${CMAKE_BUILD_TYPE}"
        RENAME mapnik${CMAKE_EXECUTABLE_SUFFIX})
endif (WIN32)

# Also add the mapnik.dll as plugin so we get correct dependencies.
set(MAPNIK_PLUGINS ${MAPNIK_PLUGINS} ${CMAKE_INSTALL_PREFIX}/bin/${CMAKE_BUILD_TYPE}/mapnik${CMAKE_SHARED_LIBRARY_SUFFIX} PARENT_SCOPE)
set(MAPNIK_BINARY_DIRECTORIES ${binary_directories} ${CMAKE_CURRENT_BINARY_DIR} PARENT_SCOPE)
