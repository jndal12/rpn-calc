CPP = g++
CPPFLAGS = -std=c++0x -g
CXX = g++ -std=c++11
DEBUG = -g
CXXFLAGS = $(shell fltk-config --cxxflags ) -std=c++11 -I.
LDFLAGS = $(shell fltk-config --ldflags )
LDSTATIC = $(shell fltk-config --ldstaticflags )
LINK = g++-4.8
OBJS = stack.o display2.o


.o:	$@.cpp $@.h
	$(CXX) $(CXXFLAGS) -c $@.cpp


RPNCalc:	RPNCalc.cpp $(OBJS)
	$(CXX) $(CXXFLAGS) RPNCalc.cpp $(OBJS) $(LDFLAGS) -o RPNCal