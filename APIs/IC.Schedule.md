# IC.Schedule.setTask({id: , callback: , monthday: , weekday: , hour:, minute:, cycle: argument:, action: , suspend: , descritpion: , onDone: });

This function adds/sets a task in to database. When conditions are matched, the callback function will be executed.

## input

### id: task ID

If the id does not exist, a new task will be added. 
If the id exists, the function sets a existing task.

### callback:

When condition matching, the callback function will be executed.

### monthday: 

1 to 31

### weekday:

Monday, Tuesday, Wednesday, Thursday, Friday, and Sunday (lower case please)

### hour:

0 to 23

### minute:

0 to 59

### cycle:

supported: hourly, daily, weekly, monthly

### argument: 

The argument will be the input for callback function.

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

* scheduleId: 
* message: 


# deleteTask({id: , onDone: });

The deleted task will be removed from database and will no longer be executed. 

# suspendTask({id: , onDone: });

The suspended task will be not executed when condition is matched without deleting. 

# resumeTask({id: , onDone: });

The function resumeTask resumes a suspended task.

# patchCallback({id: , action: , callback: });

This function, patchCallback, patches/register a callback function for a scheduled task. Scheduled tasks will be stored in database but functions will be not. When project server restarts, tasks will be reloaded but their functions. So, to patch/register back is necessary when project server restarts.

# getStatus();

To get IC.Schedule status

# enable();

To enable IC.Schedule

# disable();

To disable IC.Schedule
