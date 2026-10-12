With the gcc and llvm backends of GHDL, the tests that elaborate the same design with the same
elaboration flags share one executable, linked once in a run instead of once per test.
The executable is written to ``executables`` in the output path and is no longer found in the output
path of each test. Elaborating with ``ghdl.elab_e`` and the coverage of the llvm backend are unchanged.
