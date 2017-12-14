# stlFaceFinder
small program which attempts to split .STL files into separate "solids" by identifying triangles which share common faces. 

Objective:

Create a simple command line tool which automatically identifies faces in a .stl file and splits the solid into individual components. 

Secondary objective, pre-process .STL file prior to use by snappyHexMesh to check for common quality issues, grid alignment with surfaces, water-tightness, etc.

How to:

Download stlFaceFinder.exe
(currently windows only but will port to linux when initial features completed)

Use windows command promt to run from command line.

stlFaceFinder.exe [inputFile] [outputFile]

[inputFile] = either local file or complete file path (validation of file not done)
[outputFile] = either local file or complete file path (will overwrite files without warning)

Example:

Download pipe.STL (from this repo) and place it in the directory of stlFaceFinder.exe.
Open windows command promt or power shell.
change directory to where stlFaceFinder.exe and pipe.stl are located.

Run the program using 
> stlFaceFinder.exe pipe.STL output.STL

The output should be,

> C:\path\to\files> ./stlFaceFinder.exe wier.STL release.stl
> Importing C:\Users\Noram\Desktop\stlFaceFinder\Debug\wier.STL...  Done.
> 6162 facets in file.
> Generating edge list ... Sorting edges ... Done. (1.50148)
> Matching facets ... Done.
> Successfully matched 18486 of 18486 facet edges.
> Doing setup ... Done.
> Searching for surfaces ... Done.
> Assigning new surfaces to STL solids ... Done.
> Writing to C:\Users\Noram\Desktop\stlFaceFinder\Debug\release.stl... Done.

Source code:

Source will be made avaible in a week or so when I have cleaned it.... 
I understand anyone who doesn't trust pre-builts sorry.

https://xkcd.com/1513/
https://xkcd.com/1695/
