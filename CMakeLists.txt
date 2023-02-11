cmake_minimum_required(VERSION 3.24)
project(ovgme)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_LIBRARIES "-static-libgcc -static-libstdc++ -lwsock32 -lws2_32 ${CMAKE_CSS_STANDARD_LIBRARIES}")
set (CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -Wl,-Bstatic,--whole-archive -lwinpthread -Wl,--no-whole-archive")
set(CURL_INCLUDE_DIR ${CMAKE_SOURCE_DIR}/include/thirdparty/curl)
include_directories(include ${CURL_INCLUDE_DIR} include/thirdparty/miniz include/thirdparty/pugixml include/thirdparty/xxhash)

add_definitions("-DCURL_STATICLIB")
link_directories("${CMAKE_SOURCE_DIR}/lib")
#add_library(cURL STATIC IMPORTED)
#set_target_properties(cURL PROPERTIES IMPORTED_LOCATION "lib/libcurl.a")

add_executable(ovgme main.cpp resource.rc src/gme.cpp src/gme_conf.cpp src/gme_dlg_about.cpp src/gme_dlg_debug.cpp src/gme_dlg_game.cpp src/gme_dlg_main.cpp src/gme_dlg_mods.cpp src/gme_dlg_prof.cpp src/gme_dlg_repo.cpp src/gme_dlg_snap.cpp src/gme_game.cpp src/gme_logs.cpp src/gme_mods.cpp src/gme_netw.cpp src/gme_prof.cpp src/gme_repo.cpp src/gme_snap.cpp src/gme_tools.cpp src/gme_uins.cpp src/gmenode.cpp src/thirdparty/xxhash/xxhash.c src/thirdparty/pugixml/pugixml.cpp src/thirdparty/miniz/miniz.c)
target_link_libraries(ovgme PRIVATE libcurl.a wsock32 ws2_32 Gdi32 Comctl32 Comdlg32 Shell32 Shlwapi)
#target_link_libraries(ovgme )