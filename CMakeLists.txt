cmake_minimum_required(VERSION 3.0)

Project(tuxedo-dgpu-run)

configure_file(share/kservices5/ServiceMenus/runApplicationWithDedicatedGPU.desktop.in share/kservices5/ServiceMenus/runApplicationWithDedicatedGPU.desktop)

install(DIRECTORY libexec share ${CMAKE_CURRENT_BINARY_DIR}/share DESTINATION . PATTERN "*.in" EXCLUDE)
