## Boost build for Mobile
Scripts to build boost for different platforms (macOS, iOS, tvOS, watchOS, Linux, Android) and package it as a Maven tarball and/or an Apple Framework.

Libraries are grouped by variant (debug/release) and then by platform architecture beneath the variant. This makes debug/x86, debug/armv7 etc folders.

To build packages use ./boost.sh with appropriate argument -android, -ios, -osx, -linux or -linux-cxx11-abi-disabled. If not specified, it will attempt to build all. 

To find the directories from cmake specify two cmake defines, e.g.:

	cmake -DBOOST_INCLUDEDIR=toplevel/include -DBOOST_LIBRARYDIR=toplevel/lib/release/armv7
	
# iOS, MacOS build
The boost build for iOS and MacOS should be run on MacOS PC only.
I tested it on MacOS 10.14.4 (Mojave)
# Android build
This script support android build on MacOS and Ubuntu.