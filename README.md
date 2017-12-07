# stlFaceFinder
small program which attempts to split .STL files into separate "solids" by identifying triangles which share common faces. 

Objective:

Create a simple command line tool which automatically identifies faces in a .stl file and splits the solid into individual components. 

Secondary objective, pre-process .STL file prior to use by snappyHexMesh to check for common quality issues, grid alignment with surfaces, water-tightness, etc.

How to:

Download stlFaceFinder.exe
(currently windows only but will port to linux when initial features completed)

Use windows command promt to run from command line.

This is SLOW right now for STL files with a few 1000 facets. I am currently working on an impoved data structure to speed this up a lot.

stlFaceFinder.exe [inputFile] [outputFile]

[inputFile] = either local file or complete file path (validation of file not done)
[outputFile] = either local file or complete file path (will overwrite files without warning)

Source code:

Source will be made avaible in a week or so when I have cleaned it.... 
I understand anyone who doesn't trust pre-builts sorry.

https://xkcd.com/1513/
https://xkcd.com/1695/
