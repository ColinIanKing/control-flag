add_library(tree-sitter STATIC
  tree-sitter/lib/src/lib.c
)

target_include_directories(tree-sitter
  PRIVATE
  tree-sitter/lib/src
  tree-sitter/lib/include
)

add_library(tree-sitter-c STATIC
  tree-sitter-c/src/parser.c
)

target_include_directories(tree-sitter-c
  PRIVATE
  tree-sitter-c/src
)

add_library(tree-sitter-verilog STATIC
  tree-sitter-verilog/src/parser.c
)

target_include_directories(tree-sitter-verilog
  PRIVATE
  tree-sitter-verilog/src
)
