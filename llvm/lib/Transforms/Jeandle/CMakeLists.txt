add_llvm_component_library(LLVMJeandleTransforms
  InsertGCBarriers.cpp
  JavaOperationLower.cpp
  JeandleGCNarrowOopAnnotation.cpp
  NarrowOopOpt.cpp
  TLSPointerRewrite.cpp
  TypeCheckElimination.cpp

  ADDITIONAL_HEADER_DIRS
  ${LLVM_MAIN_INCLUDE_DIR}/llvm/Transforms/Jeandle

  LINK_COMPONENTS
  Analysis
  Core
  )
