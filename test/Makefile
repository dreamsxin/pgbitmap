# Makefile
#
#      Makefile for test directory of pgbitmap
#
#      Copyright (c) 2020 Marc Munro
#      Author:  Marc Munro
#      License: BSD
#
# Do not attempt to use this makefile explicitly: its targets are available
# and should be built from the main GNUmakefile in the parent directory.
# The GNUmakefile in this directory will build using the parent GNUmakefile
# so using make <target> in this directory will work as long as you don't
# try to specify this makefile.  It even works with emacs compile and 
# next-error functions though the number of makefiles involved seems a 
# little alarming at first.
# The whole strangeness of this makefile hierarchy derives from a, 
# possibly misguided, attempt to avoid recursive make (see the article
# "Recursive make considered harmful" for a rationale).

.PHONY: unit check test

# You can run this using several target names.
unit check test:
	psql -f test/test_bitmap.sql
