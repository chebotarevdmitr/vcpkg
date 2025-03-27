cmake_minimum_required(VERSION 3.10)

project(CheckersGame)

# Указываем стандарт C++ (используем C++17)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Подключаем SFML
find_package(SFML 3 COMPONENTS graphics window system REQUIRED)

# Добавляем исполняемый файл
add_executable(CheckersProject src/main.cpp)

# Линкуем SFML
target_link_libraries(CheckersProject sfml-graphics sfml-window sfml-system)