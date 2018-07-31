# DoxygenMakefile
A includefile for Makefiles creating a dyxygen-configurationsfile for the sourcecode-documentation-tool Doxygen.

In this maner it becomes possible creating a documentation depending on your makefiles project.

Set in your makefile the variables using by Doxygen. E.g.:
```
DOX_PROJECT_NAME = "My very nice Project"
DOX_PROJECT_NUMBER = "4711"
DOX_PROJECT_LOGO = myLogo.png
DOX_EXTRACT_ALL = YES
DOX_EXTRACT_PRIVATE = YES
DOX_CALL_GRAPH = YES
DOX_CALLER_GRAPH = YES
```
Include at the buttom of your makefile:
```
include makefile.dox
```
To creating your documentation just type:
```
make doc
```
To deleting your documentation type:
```
make deldoc
```
