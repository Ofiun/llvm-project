set(LLVM_TARGET_DEFINITIONS ShapeOps.td)
mlir_tablegen(ShapeOps.h.inc -gen-op-decls)
mlir_tablegen(ShapeOps.cpp.inc -gen-op-defs)
mlir_tablegen(ShapeOpsDialect.h.inc -gen-dialect-decls)
add_public_tablegen_target(MLIRShapeOpsIncGen)
