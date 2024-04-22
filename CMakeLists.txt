cmake_minimum_required(VERSION 3.10)

project(MyQtApp)

# Найдем пакет Qt5
find_package(Qt5 COMPONENTS Widgets REQUIRED)

# Добавим исполняемый файл
add_executable(MyQtApp main.cpp)

# Свяжем библиотеки Qt с нашим приложением
target_link_libraries(MyQtApp Qt5::Widgets)
