# IC.Standalone
This API will not depend other *.js, so it can run independently.
The API also supports multiple platforms as compatible as possible.
Mocha also covers functions in the API.

## diskSpace({onDone: });

This function gets information about disk spaces, used spaces, and free spaces.

### Input

onDone: function (result) {}
Just put a callback function named onDone to receive returned results.


### Output

{err: , disk}

The returned results will be an object with two items, err and disk.

If (err === null) indicates that no error occurs, otherwise err returns error messages.
Your can use disk information if no error occurs.


## whichPartition({path: , onDone: });

This function returns

## is enoughDiskSpace();




