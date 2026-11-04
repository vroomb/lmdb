cmake_minimum_required(VERSION 3.19)
project(lmdb VERSION 1.0.2 LANGUAGES C)

add_library(lmdb SHARED
	"mdb.c"
	"midl.c"
	"module.c"
)

target_compile_definitions(lmdb PUBLIC C_STANDARD_REQUIRED)
