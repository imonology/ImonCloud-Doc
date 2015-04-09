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
The deleted task will no longer be executed.

# suspendTask({id: , onDone: });
The suspended task will be not executed when condition is matched without deleting. 

# resumeTask({id: , onDone: });

# patchCallback({id: , action: , callback: });
This function, patchCallback, patches(register) a callback function for a schedule task. Scheduled tasks will be stored in database but functions will not. When project server restarts, tasks will be reloaded but functions. So, to patch/register back is necessary when project server starts.

# getStatus();
To get IC.Schedule status

# enable();
To enable IC.Schedule

# disable();
To disable IC.Schedule
