add_swift_library(swiftIRGen STATIC
  AllocStackHoisting.cpp
  DebugTypeInfo.cpp
  EnumPayload.cpp
  ExtraInhabitants.cpp
  Fulfillment.cpp
  GenArchetype.cpp
  GenBuiltin.cpp
  GenCall.cpp
  GenCast.cpp
  GenClangDecl.cpp
  GenClangType.cpp
  GenClass.cpp
  GenConstant.cpp
  GenControl.cpp
  GenCoverage.cpp
  GenDecl.cpp
  GenEnum.cpp
  GenExistential.cpp
  GenFunc.cpp
  GenHeap.cpp
  GenInit.cpp
  GenMeta.cpp
  GenObjC.cpp
  GenOpaque.cpp
  GenPoly.cpp
  GenProto.cpp
  GenReflection.cpp
  GenStruct.cpp
  GenTuple.cpp
  GenType.cpp
  GenValueWitness.cpp
  IRGen.cpp
  IRGenDebugInfo.cpp
  IRGenFunction.cpp
  IRGenMangler.cpp
  IRGenModule.cpp
  IRGenSIL.cpp
  Linking.cpp
  LocalTypeData.cpp
  StructLayout.cpp
  SwiftTargetInfo.cpp
  TypeLayoutVerifier.cpp
  LINK_LIBRARIES
    swiftAST
    swiftLLVMPasses
    swiftSIL
    swiftSILGen
    swiftSILOptimizer

    # Clang dependencies.
    # FIXME: Clang should really export these in some reasonable manner.
    clangCodeGen
    clangAST
)
