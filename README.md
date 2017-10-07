# JoesJunk

This is a collection of little utilities. The intention is that the code is simple and mostly self-contained. The code is not a library, but rather a collection of files that can be copied piecemeal into a project.

Some pieces are contained entirely in an X.h file, and other pieces are contained in a pair of Y.h and Y.cpp files. Although most files are independent, some super common utilities like vec.h are used extensively even if not strictly necessary. e.g. If I have an image struct, I am likely to use vector primitives as in:

struct Image
{
	vec2i size;
	vec4f *data;
};
