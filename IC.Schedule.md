# IC.Schedule.setTask({id: , callback: , monthday: , weekday: , hour:, minute:, cycle: argument:, action: , suspend: , descritpion: , onDone: });

## input
### id: task ID
If

### callback:
When condition matching, the callback will be executed.

### monthday: 
1 to 31

### weekday:
Monday, Tuesday, Wednesday, Thursday, Friday, and Sunday

### hour:
0 to 23

### minute:
0 to 59

### cycle:
supported: hourly, daily, weekly, monthly

### argument: 
The argument will be the input for callback function 

### action:
The action should be the callback name which is expected to execute. 

### suspend:
Without delete, this task will not be executed when condition is matched.

### description:
You can give some descriptions for this task.

### onDone: callback function

The callback function will be executed when this setTask is finished.

## Output
{scheduleId: , message: }

### scheduleId:



### message:



# deleteTask({id: , onDone: });

# suspendTask({id: , onDone: });

# resumeTask({id: , onDone: });

# patchCallback({id: , action: , callback: });


# getStatus();

# enable();



# disable();

