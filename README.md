# Todo: Terminal-based Todo List Manager

**Author:** Tyler Petresky

**Description:** The purpose of this project is to provide an extremely easy to use, yet versatile interface for managing simple to-do lists within your terminal. As long as this file in your `PATH`, you can execute an array of commands to easily manage multiple lists to keep track of what you need to get done.

## Commands:
**Create a List**
  - `init <list>`: Initialize a new list with a given identifier
  - `i`: Alias for `init`
  

**Delete a List or Delete a Task**
  - `remove <list>`: Delete an entire todo list
  - `remove <list> <item #>`: Remove a single task from a given todo list
  - `rm`: Alias for `remove`

**Add a Task to a List**
  - `add <list> "<task to add>"`: Add a single task to a given todo list
  - `add "<task to add>"`: Add a single task to the currently active todo list (see `activate` and `deactivate`)
  - `a`: Alias for `add`

**Show all Lists/Items**
  - `list`: List all currently initialized lists
  - `list <list>`: List all tasks within a given list
  - `ls`: Alias for `list`

**Do/Undo Tasks**
  - `do <list> <item #>`: Mark a task within a given list as "completed"
  - `d`: Alias for `do`
  - `undo <list> <item #>`: Mark a task within a given list as "incomplete"
  - `u`: Alias for `undo`
  
**Clear a List**
  - `clear <list>`: Clear a list and reinitialize it
  - `cls <list>`: Alias for `clear`

**Activate/Deactive List**

The concept of an "active" list exists to allow you to skip typing the name of a list when you want to add a lot of tasks to a particular todo list. Rather than typing `todo add <list> "<task to add>"` everytime. You can simply activate a list (`todo activate <list>`) and then just enter `todo add "<task to add>"`, or with the built-in alias, `todo a "<task to add>"`. This will add all following insertions to the same list.
  - `activate <list>`: Set a given list as the "active" list
  - `deactivate`: Set the currently "active" list as "inactive"
 
**For Extra Ease of Use**

For added ease and quicker typing add these two aliases to your terminal:<br />
<code>alias do="todo add"</code><br />
<code>alias did="todo do"</code>
 
This will allow you to type something like the following:

<code>do "Task to do"</code>: Will add to the active list

<code>do list "Task to do"</code>: Will add to the list entitled 'list'

<code>did list 2</code>: Mark item 2 on the list entitled 'list' as completed
