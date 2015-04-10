# IC.Standalone

Implementation of this API do not depend on other *.js files as well as external packages, so this API can be run independently.
This API depends only Node.js APIs or packages in bare Node.js.
The API also supports multiple platforms as compatible as possible.
Mocha also covers functions in the API.

## result = cleanArray(arr);

This function gets rid of empty elements in the given array, and returns an array.

### input

an array

### output

return array;


## result = compare2arrays(array1, array2);

This function returns that the given two arrays are identical or not.
note: This function currently supports only simple arrays with only simple elements, such as numbers, integers, and boolean.
Objects and arrays cannot be included.



## diskSpace({onDone: });

This function gets information about disk spaces, used spaces, and free spaces.

### Input

onDone: function (result) {}
Just put a callback function named onDone to receive returned results.


### Output

{err: , disk: }

The returned result will be an object with two items, err and disk.

If (err === null) indicates that no error occurs, otherwise err returns error messages.
Your can use disk information if no error occurs.


## whichPartition({path: , onDone: });

When give an existing path, this function returns corresponding partition by onDone callback function.

### Input

path: The path is a string. If given path exists, onDone callback function will return corresponding partition. If given path does not exist, return an error message.

onDone: callback function

### output

err, {resolvedPath: , mount: }



{err: , resolvedPath: , mount: }



## is enoughDiskSpace();




