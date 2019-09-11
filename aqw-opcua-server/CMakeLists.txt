set(headers
  "CountryData.h"
  "LocationData.h"
  "Settings.h"
  "WeatherData.h"
  "WebService.h"
)

set(sources
  "Application.cpp"
  "CountryData.cpp"
  "LocationData.cpp"
  "Settings.cpp"
  "WeatherData.cpp"
  "WebService.cpp"
)

source_group("Headers" ${headers})
source_group("Sources" ${sources})

add_executable(aqw-opcua-server ${headers} ${sources})

target_link_libraries(aqw-opcua-server PRIVATE
  CONAN_PKG::open62541
  CONAN_PKG::cpprestsdk)
