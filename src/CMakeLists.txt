#SET(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)
#在这里add_executable在这里set path
#现在我有install，可以不生成到bin，install会生成
#SET(LIBRARY_OUTPUT_PATH ${PROJECT_BINARY_DIR}/lib)
ADD_EXECUTABLE(myskills main.c)
INSTALL (TARGETS myskills DESTINATION installbin) 
