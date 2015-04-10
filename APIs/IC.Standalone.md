# IC.Standalone

Implementation of this API do not depend on other *.js files as well as external packages, so this API can be run independently.
This API depends only Node.js APIs or packages in bare Node.js.
The API also supports multiple platforms as compatible as possible.
Mocha also covers functions in the API.

## diskSpace({onDone: });

This function gets information about disk spaces, used spaces, and free spaces.

### Input

onDone: function (result) {}
Just put a callback function named onDone to receive returned results.


### Output

{err: , disk: }

The returned results will be an object with two items, err and disk.

If (err === null) indicates that no error occurs, otherwise err returns error messages.
Your can use disk information if no error occurs.


## whichPartition({path: , onDone: });

When give a existing path, this function returns corresponding partition by onDone callback function.

### Input

path: 

### output

## is enoughDiskSpace();




