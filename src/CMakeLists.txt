project(TESS)

add_library(${PROJECT_NAME} STATIC)

aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR} PROJECT_SOURCES)

target_sources(${PROJECT_NAME}
	PRIVATE ${PROJECT_SOURCES}
)

install(TARGETS ${PROJECT_NAME}
	ARCHIVE DESTINATION "${CMAKE_INSTALL_PREFIX}/lib"
)