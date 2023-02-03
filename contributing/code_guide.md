Adapted from RoundWorld Solutions


# Code Guide

The following rules will be enforced on any code written for applications.

## Variable Naming Conventions

1) The name should describe the use or name of the data in question in no more than two words.
2) iOS App / Swift - Variables will be in camel case
3) Robot / Python - Variables will be all lowercase with underscores between words. 

## Headers

Files and Functions should have a commented header as follows:

### Swift

File Header:
```Swift
/*-------------------------------------------------------------------
  File: MYFILE.EXT
  Summary: Give a brief summary of the file contents and purpose
  Exported Data Structures and Functions
-------------------------------------------------------------------*/
```
Function Header:
```Swift
/*-------------------------------------------------------------------
  Function: MyLocalFunction
  Summary: Give a brief summary of what the function is for
  Params: MYTYPE MyFunctionParam1
          Description
          MYTYPE MyFunctionParam2
          Description
  Returns: MYRETURNTYPE
           Description
-------------------------------------------------------------------*/
```

### Python

File Header:
```Python
#-------------------------------------------------------------------
#  File: MYFILE.EXT
#  Summary: Give a brief summary of the file contents and purpose
#  Exported Data Structures and Functions
#-------------------------------------------------------------------
```

Function Header:
```Python
#-------------------------------------------------------------------
#  Function: MyLocalFunction
#  Summary: Give a brief summary of what the function is for
#  Params: my_function_param_1
#          Description
#          my_function_param_2
#          Description
#  Returns: Description
#-------------------------------------------------------------------
```
