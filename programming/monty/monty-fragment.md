<div id="intro">

<div class="lead">

<pic eager add-class="float-start border me-2 mt-2 p1 bg-white" src="https://upload.wikimedia.org/wikipedia/en/c/cb/Flyingcircus_2.jpg" width="200">

<small><small>The **Monty Python** Comedy Group,<br> [[credit: Wikipedia](https://en.wikipedia.org/wiki/Monty_Python)]</small></small>
</pic>

**The _Monty Project_ is an educational software project designed to take you through the steps of building a small software _incrementally_**, while applying as many Python and SE techniques as possible along the way.
</div>

**The project aims to build a product named _Monty_, a Personal Assistant Chatbot that helps a person to keep track of various things.** %%The name _Monty_ was chosen as a placeholder name, in honor of the [Monty Python comedy group](https://en.wikipedia.org/wiki/Monty_Python) whose work inspired the name of the Python language.%% **You may give it any other name and personality you wish.**

Here is a sample interaction with Monty:
```
*******************************************************************************************
*  __          __  _                            _          __  __             _           *
*  \ \        / / | |                          | |        |  \/  |           | |          *
*   \ \  /\  / /__| | ___ ___  _ __ ___   ___  | |_ ___   | \  / | ___  _ __ | |_ _   _   *
*    \ \/  \/ / _ \ |/ __/ _ \| '_ ' _ \ / _ \ | __/ _ \  | |\/| |/ _ \| '_ \| __| | | |  *
*     \  /\  /  __/ | (_| (_) | | | | | |  __/ | || (_) | | |  | | (_) | | | | |_| |_| |  *
*      \/  \/ \___|_|\___\___/|_| |_| |_|\___|  \__\___/  |_|  |_|\___/|_| |_|\__|\__, |  *
*                                                                                  __/ |  *
*                                                                                 |___/   *
*******************************************************************************************

>>> What can I do for you?

help
>>> I'm glad you asked. Here it is:
==================================================
Monty can understand the following commands:

  add DESCRIPTION
    Adds a task with the DESCRIPTION to the list
    Example: add read book
  done INDEX
    Marks the task at INDEX as 'done'
    Example: done 1
  exit
    Exits the application
  help
    Shows the help information
  list
    Lists the tasks in the list
--------------------------------------------------

>>> What can I do for you?

add read book
>>> Task added to the list
>>> What can I do for you?

add return book
>>> Task added to the list
>>> What can I do for you?

done 1
>>> Congrats on completing a task! :-)
>>> What can I do for you?

list
>>> Here is the list of tasks:
==================================================
STATUS | INDEX | DESCRIPTION
--------------------------------------------------
  X    |   1   | read book
  -    |   2   | return book
--------------------------------------------------
>>> What can I do for you?
```
</div>

<div id="increments_summary">

The project consists of the following _increments_:
* **Levels**: A series of features, meant to be added to Monty in the given order, although some can be skipped. These have been named `Level 1` to `Level 14` to indicate how each makes the product progressively "level up".
* **Extensions:**
  * ++<span class="badge rounded-pill bg-primary">Category B</span>++ These are enhancements related to task tracking.
  * ++<span class="badge rounded-pill bg-success">Category C</span>++ These are enhancements, not specifically related to task tracking.
  * ++<span class="badge rounded-pill bg-danger">Category D</span>++ Each of these adds the ability to track another type of entities.
</div>

## Levels

<div id="monty1">

### <span class="badge bg-info">Level 1</span> <span class="text-info">Echo Once</span>

Write a Python program to read in one user command and repeat it back to the user. An example output is given below.

```
>>> Hello, my name is Monty
>>> What can I do for you?
foo
>>> Your command is: foo
>>> Bye!
```

<panel header=":fas-battery-quarter: Partial solution" minimized>

```python
print('>>> Hello, my name is Monty')
# ADD MORE CODE HERE
```
</panel>
</div>
{{ line_double }}
<div id="monty2">

### <span class="badge bg-info">Level 2</span> <span class="text-info">Recognize Known Commands</span>

Extend [Monty 1 code]({{ baseUrl }}/programming/chapters/monty.html#monty1) to work as follows:
* It recognizes the `list` command and responds with a fixed message.
* It recognizes the `exit` command and exits the program if user confirms.
* For all other inputs, it responds with a fixed error message.

A sample session is given below.

<box type="warning">

You are highly encouraged to give the software a **different name** (i.e., not Monty), define your own **command formats** (e.g., `show` instead of `list`), and even a different **personality** (e.g., you can make its questions/responses sound similar to a popular video game character). Differentiating your software in those ways will reduce the risk of plagiarism concerns.
</box>

```
>>> Hello, my name is Monty
>>> What can I do for you?

list
>>> Nothing to list
>>> What can I do for you?

foo
>>> OOPS! Unknown command
>>> What can I do for you?

exit
>>> Are you sure? y/n
n
>>> What can I do for you?

exit
>>> Are you sure? y/n
y
>>> Bye!
```

<panel header=":fas-battery-quarter: Partial solution" minimized>

```python
print('>>> Hello, my name is Monty')
while True:
    print('>>> What can I do for you?')
    # ADD MORE CODE HERE
print('>>> Bye!')
```
</panel>

</div>
{{ line_double }}
<div id="monty3">

### <span class="badge bg-info">Level 3</span> <span class="text-info">Use Functions</span>

Restructure the [Monty Level 2 code]({{ baseUrl }}/programming/chapters/monty.html#monty2) to fit the following structure, while keeping the behavior same as before.

```python
import sys


# ADD MISSING FUNCTIONS


def main():
    print_greeting()
    while True:
        command = read_command()
        execute_command(command)


main()
```

<panel header=":fas-battery-quarter: Partial solution" minimized>

```python
import sys

def is_exit_confirmed():
    print('>>> Are you sure? y/n')
    response = input()
    return response == 'y'


def execute_command(command):
    if command == '':
        return
    elif command == 'exit':
        if is_exit_confirmed():
            print('>>> Bye!')
            sys.exit()
    # ...


def main():
    print_greeting()
    while True:
        command = read_command()
        execute_command(command)


main()
```
</panel>

</div>
{{ line_double }}
<div id="monty4">

### <span class="badge bg-info">Level 4</span> <span class="text-info">Collect Tasks in Memory</span>

Enhance the [Monty Level 3 code]({{ baseUrl }}/programming/chapters/monty.html#monty3) to improve the functionality as per the sample output given below.

```
>>> Hello, my name is Monty
>>> What can I do for you?

list
>>> Nothing to list
>>> What can I do for you?

add read book
>>> What can I do for you?

list
>>> List of items:
     1. read book
>>> What can I do for you?

add return book
>>> What can I do for you?

list
>>> List of items:
     1. read book
     2. return book
>>> What can I do for you?

exit
>>> Are you sure? y/n
y
>>> Bye!
```

<box>

{{ icon_tip }} You can use the list slicing syntax to extract a portion of a  string.<br>

<include src="inputOutput.md" boilerplate>
<span id="input">

```python

s = 'abcdefgh'
print(s[2:])
print(s[:5])
```
</span>
<span id="output">

```
cdefgh
abcde
```

</span>
</include>

The above technique can be used to extract the item description from an `add` command.
</box>


<panel header=":fas-battery-quarter: Partial solution" minimized>

```python
import sys

items = []


def print_items():
    if len(items) == 0:
        print('>>> Nothing to list')
    else:
        for i, item in enumerate(items):
            # ...


def add_item(user_input):
    # ...


def terminate():
    # ...

# ...

def execute_command(command):
    if command == '':
        return
    elif command == 'exit':
        terminate()
    elif command == 'list':
        print_items()
    elif command.startswith('add '):
        add_item(command)
    else:
        print('>>> OOPS! Unknown command')


def main():
    print_greeting()
    while True:
        command = read_command()
        execute_command(command)


main()
```
</panel>

</div>
{{ line_double }}

<div id="monty5">

### <span class="badge bg-info">Level 5</span> <span class="text-info">Mark Tasks as Done</span>

Enhance the [Monty Level 4 code]({{ baseUrl }}/programming/chapters/monty.html#monty4) in the following ways:
* Add a `done` command so that the user can mark a task as done. e.g., `done 2` marks the task at index 2 as _done_.
* Show appropriate error messages if the user gives an invalid index for the `done` command
* Optionally, implement an `undone` (or `unmark`) command to change the status of a task back to _not done_.

A sample output is given below.

```
>>> Hello, my name is Monty
>>> What can I do for you?

add borrow book
>>> What can I do for you?

add read book
>>> What can I do for you?

add return book
>>> What can I do for you?

list
>>> List of items:
     [ ] 1. borrow book
     [ ] 2. read book
     [ ] 3. return book
>>> What can I do for you?

done 1
>>> What can I do for you?

list
>>> List of items:
     [X] 1. borrow book
     [ ] 2. read book
     [ ] 3. return book
>>> What can I do for you?

done abc
>>> SORRY, I could not perform that command. Problem: abc is not a number
>>> What can I do for you?

done 5
>>> SORRY, I could not perform that command. Problem: No item at index 5
>>> What can I do for you?

done 0
>>> SORRY, I could not perform that command. Problem: Index must be greater than 0
>>> What can I do for you?

garbage
>>> SORRY, I could not perform that command. Problem: Command not recognized
>>> What can I do for you?

exit
>>> Are you sure? y/n
y
>>> Bye!
```

<box>

{{ icon_tip }} Each task has two data values: the description and the 'done' status. You can use a list to hold these two data items. That means your list of tasks will be a list containing lists. Example:
```python
tasks = []
tasks.append(['read book', False])
print('Description of the first task:', tasks[0][0])

if tasks[0][1]:
    print('X')
else:
    print('-')
```

{{ icon_tip }} You can use exceptions to identify and handle errors in the command.
```python
def main():
    print_greeting()
    while True:
        try:
            command = read_command()
            execute_command(command)
        except Exception as e:
            print('>>> SORRY, I could not perform that command. Problem:', e)
```
</box>


<panel header=":fas-battery-quarter: Partial solution" minimized>

```python

items = []

# ...

def get_item_for_index(index_as_string):
    try:
        index = int(index_as_string.strip())
    except Exception:
        raise ValueError(index_as_string + ' is not a number ')

    if index < 1:
        raise ValueError('Index must be greater than 0 ')

    try:
        return items[index - 1]
    except IndexError:
        raise ValueError('No item at index ' + index_as_string)


def mark_item_as_done(user_input):
    index_as_string = user_input[5:]
    get_item_for_index(index_as_string)[1] = True


def execute_command(command):
    if command == '':
        return
    elif command == 'exit':
        terminate()
    elif command == 'list':
        print_items()
    elif command.startswith('add '):
        add_item(command)
    elif command.startswith('done '):
        mark_item_as_done(command)
    else:
        raise Exception('Command not recognized')


def main():
    print_greeting()
    while True:
        try:
            command = read_command()
            execute_command(command)
        except Exception as e:
            print('>>> SORRY, I could not perform that command. Problem:', e)


main()
```
</panel>

</div>
{{ line_double }}

<div id="monty6">

### <span class="badge bg-info">Level 6</span> <span class="text-info">Give Help</span>

Enhance the [Monty Level 5 code]({{ baseUrl }}/programming/chapters/monty.html#monty5) in the following ways:
* Add a `help` command so that the user can view how to use the app.
* Improve the formatting of the text displayed to the user to make the user experience nicer.

A sample output is given below.

```
*******************************************************************************************
*  __          __  _                            _          __  __             _           *
*  \ \        / / | |                          | |        |  \/  |           | |          *
*   \ \  /\  / /__| | ___ ___  _ __ ___   ___  | |_ ___   | \  / | ___  _ __ | |_ _   _   *
*    \ \/  \/ / _ \ |/ __/ _ \| '_ ' _ \ / _ \ | __/ _ \  | |\/| |/ _ \| '_ \| __| | | |  *
*     \  /\  /  __/ | (_| (_) | | | | | |  __/ | || (_) | | |  | | (_) | | | | |_| |_| |  *
*      \/  \/ \___|_|\___\___/|_| |_| |_|\___|  \__\___/  |_|  |_|\___/|_| |_|\__|\__, |  *
*                                                                                  __/ |  *
*                                                                                 |___/   *
*******************************************************************************************

>>> What can I do for you?

help
>>> I'm glad you asked. Here it is:
==================================================
Monty can understand the following commands:

  add DESCRIPTION
    Adds a task to the list
    Example: add read book
  done INDEX
    Marks the task at INDEX as 'done'
    Example: done 1
  exit
    Exits the application
  help
    Shows the help information
  list
    Lists the tasks in the list
--------------------------------------------------

>>> What can I do for you?

add read book
>>> Task added to the list
>>> What can I do for you?

add return book
>>> Task added to the list
>>> What can I do for you?

done 1
>>> Congrats on completing a task! :-)
>>> What can I do for you?

list
>>> Here is the list of tasks:
==================================================
STATUS | INDEX | DESCRIPTION
--------------------------------------------------
  X    |   1   | read book
  -    |   2   | return book
--------------------------------------------------
>>> What can I do for you?
```

<box>

{{ icon_tip }} You can use triple quotes to define a long string such as the help text.
```python
help_text ='''
long text
more text
'''
```

{{ icon_tip }} You can generate ASCII art using online resources such as http://patorjk.com/software/taag
</box>


<panel header=":fas-battery-quarter: Partial solution" minimized>

```python
def print_greeting():
    banner = '''
*******************************************************************************************
*  __          __  _                            _          __  __             _           *
*  \ \        / / | |                          | |        |  \/  |           | |          *
*   \ \  /\  / /__| | ___ ___  _ __ ___   ___  | |_ ___   | \  / | ___  _ __ | |_ _   _   *
*    \ \/  \/ / _ \ |/ __/ _ \| '_ ' _ \ / _ \ | __/ _ \  | |\/| |/ _ \| '_ \| __| | | |  *
*     \  /\  /  __/ | (_| (_) | | | | | |  __/ | || (_) | | |  | | (_) | | | | |_| |_| |  *
*      \/  \/ \___|_|\___\___/|_| |_| |_|\___|  \__\___/  |_|  |_|\___/|_| |_|\__|\__, |  *
*                                                                                  __/ |  *
*                                                                                 |___/   *
*******************************************************************************************
'''
    print(banner.strip(), '\n')
```
</panel>

</div>
{{ line_double }}
<div id="monty7">

### <span class="badge bg-info">Level 7</span> <span class="text-info">Save Tasks to Disk</span>

Enhance the [Monty Level 6 code]({{ baseUrl }}/programming/chapters/monty.html#monty6) in the following ways:
* Monty **saves tasks into a csv file**, and **loads data from the same file at the start**.
* **Add a `delete` command** that can delete a task at a specific index.

A sample output is given below. Note the following:
* Monty is able to show at the very start the three tasks loaded from the file.
* When item 2 is deleted, the item previously at index 3 moves to position 2.

```
*******************************************************************************************
*  __          __  _                            _          __  __             _           *
*  \ \        / / | |                          | |        |  \/  |           | |          *
*   \ \  /\  / /__| | ___ ___  _ __ ___   ___  | |_ ___   | \  / | ___  _ __ | |_ _   _   *
*    \ \/  \/ / _ \ |/ __/ _ \| '_ ' _ \ / _ \ | __/ _ \  | |\/| |/ _ \| '_ \| __| | | |  *
*     \  /\  /  __/ | (_| (_) | | | | | |  __/ | || (_) | | |  | | (_) | | | | |_| |_| |  *
*      \/  \/ \___|_|\___\___/|_| |_| |_|\___|  \__\___/  |_|  |_|\___/|_| |_|\__|\__, |  *
*                                                                                  __/ |  *
*                                                                                 |___/   *
*******************************************************************************************

>>> What can I do for you?

list
>>> Here is the list of tasks:
==================================================
STATUS | INDEX | DESCRIPTION
--------------------------------------------------
  X    |   1   | borrow book
  -    |   2   | read book
  -    |   3   | return book
--------------------------------------------------
>>> What can I do for you?

delete 2
>>> Task deleted from the list
>>> What can I do for you?

list
>>> Here is the list of tasks:
==================================================
STATUS | INDEX | DESCRIPTION
--------------------------------------------------
  X    |   1   | borrow book
  -    |   2   | return book
--------------------------------------------------
```

<box>

{{ icon_tip }} here are some tips:

* The filename can be specified in the code. e.g.,
  ```python
  DATA_FILE = 'monty7.csv'
  ```

* The following statement will create an empty `data.csv` file if the file doesn't exist, but will keep the file as it is if it already exists %%(it simply opens the file in append mode -- which creates the file it if it doesn't exist -- and close it right after)%%.
  ```python
  open('data.csv', 'a').close()
  ```
* The format of the file is up to you. Here is an example:
  ```
  borrow book,done
  read book,pending
  return book,pending
  ```
* The program can load the tasks from the file at the beginning. It can save the data after each command. For example, as follows:
  ```python
   items = []
   DATA_FILE = 'monty7.csv'


   def main():
       create_file_if_missing(DATA_FILE)
       load_data(DATA_FILE) # load task data from the file
       print_greeting()
       while True:
           try:
               command = read_command()
               execute_command(command)
               save_data(DATA_FILE, items) # save all tasks in the file
           except Exception as e:
               print('>>> SORRY, I could not perform that command. Problem:', e)


   main()
  ```
</box>

<panel header=":fas-battery-quarter: Partial solution" minimized>

Here is the code for loading data from the file.
```python
def load_data(filename):
    data_file = open(filename)
    deliveries_reader = csv.reader(data_file)
    for row in deliveries_reader:
        if not row:
            continue
        add_item_from_csv_line(row)
    data_file.close()


def add_item_from_csv_line(values):
    status = True if values[1] == 'done' else False
    items.append([values[0], status])  # items is a global variable
```

Note that `status = True if values[1] == 'done' else False`{.python} is a shortcut syntax. It is equivalent to the code below:
```
if values[1] == 'done':
    status = True
else:
    status = False
```
</panel>
<p/>

Given below are some more features you can consider adding at this point (it is ==optional to add them to Monty 7==):
* **Remove the need for the user to confirm before exiting Monty.** As data are saved to a file, such a confirmation is no longer necessary because an accidental exit will not cause any permanent damage.
  ```
  >>> What can I do for you?

  exit
  >>> Bye!
  ```
* **Add a `pending` command** (other possible names: `undone` or `unmark`) that can mark a task as not-done-yet (i.e., the opposite of the `done` command), if you haven't done that already.
  ```
   >>> What can I do for you?

   list
   >>> Here is the list of tasks:
   ==================================================
   STATUS | INDEX | DESCRIPTION
   --------------------------------------------------
     X    |   1   | borrow book
     -    |   2   | read book
     -    |   3   | return book
   --------------------------------------------------
   >>> What can I do for you?

   pending 1
   >>> OK, I have marked that item as pending
   >>> What can I do for you?

   list
   >>> Here is the list of tasks:
   ==================================================
   STATUS | INDEX | DESCRIPTION
   --------------------------------------------------
     -    |   1   | borrow book
     -    |   2   | read book
     -    |   3   | return book
   --------------------------------------------------
   >>> What can I do for you?
  ```
* **Make commands case-insensitive and immune to extra leading/trailing spaces**. For example, all these commands should work the same way.
  ```
  add read book
  ADD read book
  Add read book
  add    read book
      add read book
  ```

</div>

{{ line_double }}

<div id="monty8">

### <span class="badge bg-info">Level 8</span> <span class="text-info">Support Deadlines</span>

Enhance the [Monty Level 7 code]({{ baseUrl }}/programming/chapters/monty.html#monty7) to add support for keeping track of deadlines as well as regular todo tasks

Previous behavior:
* `add buy book`: adds a task `buy book`

Proposed change - replace the above command with the following two:
* `todo read book`: adds a todo task `read book`
* `deadline return book by: May 3rd` adds a deadline `return book` which is to be done by `May 3d`.<br>
  Note: `by:` is a keyword. Anything that comes after it is considered a description of the deadline.

A sample output is given below.

```
>>> What can I do for you?

list
>>> Here is the list of tasks:
============================================================
STATUS | INDEX | DESCRIPTION                 | DEADLINE
------------------------------------------------------------
  X    |   1   | borrow book                 | -
  -    |   2   | read book                   | -
  -    |   3   | return book                 | Monday
------------------------------------------------------------
>>> What can I do for you?

todo watch movie
>>> What can I do for you?

deadline submit assignment by: end of May
>>> What can I do for you?

list
>>> Here is the list of tasks:
============================================================
STATUS | INDEX | DESCRIPTION                 | DEADLINE
------------------------------------------------------------
  X    |   1   | borrow book                 | -
  -    |   2   | read book                   | -
  -    |   3   | return book                 | Monday
  -    |   4   | watch movie                 | -
  -    |   5   | submit assignment           | end of May
------------------------------------------------------------
>>> What can I do for you?
```

<box>

{{ icon_tip }} here are some tips:

* One option is to use a list of dictionary objects to store the tasks/deadlines. Given below is an example of such a data structure. In that data structure, `T` and `D` is used to indicate todo items and deadline items, respectively.
  ```python{.no-line-numbers}
  [
   {'type': 'T', 'description': 'borrow book', 'is_done': True},
   {'type': 'T', 'description': 'read book', 'is_done': False},
   {'type': 'D', 'description': 'return book', 'is_done': False, 'by': 'Monday'}
  ]

  ```
* The format of the csv file needs to be updated to store extra values too. Here is an example:
  ```{.no-line-numbers}
  T,borrow book,done
  T,read book,pending
  D,return book,pending,Monday
  ```
</box>

<panel header=":fas-battery-quarter: Partial solution" minimized>

Here is the code for adding a todo item:
```python

command_parts = command.strip().split(' ', 1) # split the command into two: first word and the remainder
if action == 'todo':
    items.append({'type': 'T', 'description': command_parts[1], 'is_done': False})
elif  ...
```

</panel>
<p/>

</div>

{{ line_double }}

<div id="monty9">

### <span class="badge bg-info">Level 9</span> <span class="text-info">Use Classes</span>

Enhance the [Monty Level 8 code]({{ baseUrl }}/programming/chapters/monty.html#monty8) to use classes `ToDo` and `Deadline` (i.e., you need to define these two classes) to represent todo tasks and deadlines, respectively.<br>
{{ icon_info }} This means you no longer needs to use `dict` objects to represent todo/deadline tasks. That is, your tasks can be kept as a `list` of `ToDo` and `Deadline` objects, instead of a `list` of `dict`objects.

<box header=":fas-lightbulb: A shorthand for `if-else`">
Consider the following code:

```python
def get_as_word(status):
    if status == 1:
        return 'Yes'
    else:
        return 'No'
```

The same can be written using the following shorthand for `if-else`:
```python
def get_as_word(status):
    return 'Yes' if status == 1 else 'No'
```
A few more examples:
```python
status_as_word = 'Yes' if status == 1 else 'No'
print('Yes') if status == 1 else print('No')
print('Yes' if status == 1 else 'No')
```

Note that this shorthand requires both the `if` part and the `else` part.

</box>


<panel header=":fas-battery-quarter: Partial solution" minimized>

Here is the code for an example `ToDo` class:
```python
class ToDo:

    def __init__(self, description, status):
        self.description = description
        self.is_done = status

    def mark_as_done(self):
        self.is_done = True

    def mark_as_pending(self):
        self.is_done = False

    def as_string(self):
        """ Return the details of todo object as a string"""
        status = 'X' if self.is_done else '-'
        return status.center(6) + ' ' + '   -'.ljust(13) + self.description

    def as_csv(self):
        """ Return the details of todo object as a list,
        suitable to be stored in a csv file.
        """
        return ['T', self.description, 'done' if self.is_done else 'pending']
```

Here are some sample functions that work with `ToDo` objects:
```python
def load_data(filename):
    data_file = open(filename)
    deliveries_reader = csv.reader(data_file)
    for row in deliveries_reader:
        if row[0] == 'T':
            items.append(ToDo(row[1], True if row[2] == 'done' else False))
        elif row[0] == 'D':
            items.append(Deadline(row[1], True if row[2] == 'done' else False, row[3]))
    data_file.close()


def save_data(filename, items_to_save):
    output_file = open(filename, 'w', newline='')
    output_writer = csv.writer(output_file)
    for item in items_to_save:
        output_writer.writerow(item.as_csv())
    output_file.close()
```

</panel>
<p/>

</div>

{{ line_double }}

<div id="monty10">

### <span class="badge bg-info">Level 10</span> <span class="text-info">Use More Classes</span>

Enhance the [Monty Level 9 code]({{ baseUrl }}/programming/chapters/monty.html#monty9) to extract the following classes:

* `UserInterface`: an object of this class can be used to handle reading input from the user and showing output back to the user.
* `StorageManager`: an object of this class can be used to read data from the data file and write data back to the data file.
* `TaskManager`: an object of this class will hold the list of `Task`/`Deadline` objects and will execute commands.



<panel header=":fas-battery-quarter: Partial solution" minimized>

Here's the main part of the code that illustrates how these objects can work together:
```python
def main():
    # create a UserInterface object and show the greeting
    ui = UserInterface()
    ui.show_greeting()

    # create a StorageManager object
    storage = StorageManager('data.csv')

    # create a TaskManager object and load data
    task_manager = TaskManager(storage)
    task_manager.load_data()

    while True:
        try:
            command = ui.read_command()
            execute_command(command, task_manager, ui)
            task_manager.save_data()
        except Exception as e:
            ui.display('SORRY, I could not perform that command. Problem:' + str(e))


main()
```

Here's a partial `execute_command` function:

```python
def execute_command(command_parts, task_manager, ui):
    if action == 'exit':
        ui.display('Bye!')
        sys.exit()
    elif action == 'list':
        message = task_manager.get_items_as_table()
        ui.display(message)
    elif action == 'todo':
        message = task_manager.add_item(ToDo(command_parts[1], False))
        ui.display(message)
    ...
```

</panel>
<p/>

**Optional feature to consider:** add a `progress` command that shows how many tasks/deadlines were marked as _done_ during a session so far. Here is an example output:
```
>>> What can I do for you?

list
>>> Here is the list of tasks:
    ============================================================
    STATUS | INDEX | DESCRIPTION                 | DEADLINE
    ------------------------------------------------------------
      X    |   1   | borrow book                 | -
      -    |   2   | read book                   | -
      -    |   3   | return book                 | Monday
    ------------------------------------------------------------
>>> What can I do for you?

progress
>>> Progress for this session: todos 0 deadlines 0
>>> What can I do for you?

done 2
>>> Congrats on completing a task! :-)
>>> What can I do for you?

progress
>>> Progress for this session: todos 1 deadlines 0
>>> What can I do for you?

done 3
>>> Congrats on completing a task! :-)
>>> What can I do for you?

progress
>>> Progress for this session: todos 1 deadlines 1
>>> What can I do for you?

pending 2
>>> OK, I have marked that item as pending
>>> What can I do for you?

progress
>>> Progress for this session: todos 0 deadlines 1
>>> What can I do for you?

list
>>> Here is the list of tasks:
    ============================================================
    STATUS | INDEX | DESCRIPTION                 | DEADLINE
    ------------------------------------------------------------
      X    |   1   | borrow book                 | -
      -    |   2   | read book                   | -
      X    |   3   | return book                 | Monday
    ------------------------------------------------------------
>>> What can I do for you?
```


<panel header=":fas-battery-quarter: Partial solution" minimized>

A class-level variable in the `ToDo` class can be used to track the number of todo tasks marked as _done_ in a session.

```python
class ToDo:

    progress = 0  # class-level variable

    def __init__(self, description, status):
        self.description = description
        self.is_done = status

    def mark_as_done(self):
        if not self.is_done: # increment progress if needed
            ToDo.progress = ToDo.progress + 1
        self.is_done = True
```

</panel>
<p/>

</div>

{{ line_double }}

<div id="monty11">

### <span class="badge bg-info">Level 11</span> <span class="text-info">Use Multiple Code Files</span>

Enhance the [Monty Level 10 code]({{ baseUrl }}/programming/chapters/monty.html#monty10) to divide the source code into multiple files (e.g., `todo.py`, `deadline.py`, etc.).

</div>

{{ line_double }}

<div id="monty12">

### <span class="badge bg-info">Level 12</span> <span class="text-info">Use Inheritance</span>

Enhance the [Monty Level 11 code]({{ baseUrl }}/programming/chapters/monty.html#monty11) to make the `Deadline` class inherit from the `ToDo` class:



<panel header=":fas-battery-quarter: Partial solution" minimized>


```python
class ToDo:

    TYPE_KEY = 'T'

    def __init__(self, description, status):
        self.description = description
        self.is_done = status

    def mark_as_done(self):
        self.is_done = True

    def mark_as_pending(self):
        self.is_done = False

    def __status_as_icon(self):
        return 'X' if self.is_done else '-'

    def __str__(self):
        return '(' + self.__status_as_icon() + ') ' + self.description

    # more code ...


class Deadline (ToDo):

    TYPE_KEY = 'D'

    def __init__(self, description, status, by):
        super().__init__(description, status)
        self.by = by

    def __str__(self):
        return super().__str__() + ' [by: ' + self.by + ']'

```

Note:
* There no need for the `Deadline` class to implement methods such as `mark_as_done` because it inherits those methods from the parent class.
* Note how the `Deadline` class overrides some methods (e.g., `__init__`) but uses the parent class method inside the overridden method (e.g., `__init__` method of the `Deadline` class calls the `super().__init__()` method.

</panel>

</div>

{{ line_double }}

<div id="monty13">

### <span class="badge bg-info">Level 13</span> <span class="text-info">Add Unit Tests</span>

Add some unit tests to [Monty Level 12 code]({{ baseUrl }}/programming/chapters/monty.html#monty12).

Minimum requirement: 2 unit tests, testing two functions/methods

</div>

{{ line_double }}

<div id="monty14">

### <span class="badge bg-info">Level 14</span> <span class="text-info">Add a GUI</span>

Enhance the [Monty Level 13 code]({{ baseUrl }}/programming/chapters/monty.html#monty13) to integrate it with the skeletal GUI given below.

Notes about the given version of the GUI:
* The GUI shows the list of tasks all the time.
* It initializes with some dummy data.
* It only supports an `add` command and a `help` command.

Here are some screenshots of the GUI:<br>
<pic eager src="images/gui-start.png"></pic><p/>
<pic eager src="images/gui-later.png"></pic>

<panel type="seamless" header="Skeletal GUI code">

```python
import datetime
from tkinter import *

import sys


class GUI:

    def __init__(self, task_manager):
        self.task_manager = task_manager
        self.window = Tk()
        self.window.geometry('800x700')  # set Window size
        self.window.title('Monty')  # set Window title

        self.input_box = Entry(self.window)  # create an input box
        self.input_box.pack(padx=5, pady=5, fill='x')  # make the input box fill the width of the Window
        self.input_box.bind('<Return>', self.command_entered)  # bind the command_entered function to the Enter key
        self.input_box.focus()  # set focus to the input box

        # add a text area to show the chat history
        self.history_area = Text(self.window, width="50")
        self.history_area.pack(padx=5, pady=5, side=LEFT, fill="y")
        self.output_font = ('Courier New', 12)
        self.history_area.tag_configure('error_format', foreground='red', font=self.output_font)
        self.history_area.tag_configure('success_format', foreground='green', font=self.output_font)
        self.history_area.tag_configure('normal_format', font=self.output_font)

        # add a text area to show the list of tasks
        self.list_area = Text(self.window)
        self.list_area.pack(padx=5, pady=5, side=RIGHT, fill="both")
        self.list_area.tag_configure('normal_format',  font=self.output_font)
        self.list_area.tag_configure('pending_format', foreground='red', font=self.output_font)
        self.list_area.tag_configure('done_format', foreground='green', font=self.output_font)

        # show the welcome message and the list of tasks
        self.update_chat_history('start', 'Welcome to Monty!', 'success_format')
        self.update_task_list(self.task_manager.items)

    def update_chat_history(self, command, response, status_format):
        """
        status_format: indicates which color to use for the status message
          can be 'error_format', 'success_format', or 'normal_format'
        """
        current_time = datetime.datetime.now().strftime("%H:%M:%S")
        self.history_area.insert(1.0, '-' * 40 + '\n', 'normal_format')
        self.history_area.insert(1.0, '>>> ' + response + '\n', status_format)
        self.history_area.insert(1.0, 'You said: ' + command + '\n', 'normal_format')
        self.history_area.insert(1.0, current_time + '\n', 'normal_format')

    def update_task_list(self, tasks):
        self.list_area.delete('1.0', END)  # clear the list area
        for i, task in enumerate(tasks):
            if task[1]:
                icon = 'X'
                output_format = 'done_format'
            else:
                icon = '-'
                output_format = 'pending_format'
            self.list_area.insert(END, icon + ' ' + str(i+1) + ' ' + task[0] + '\n', output_format)

    def clear_input_box(self):
        self.input_box.delete(0, END)

    def command_entered(self, event):
        command = None
        try:
            command = self.input_box.get()
            if command.strip().lower() == 'exit':
                sys.exit()
            output = self.task_manager.execute_command(command)
            self.update_chat_history(command, output, 'success_format')
            self.update_task_list(self.task_manager.items)
            self.clear_input_box()
        except Exception as e:
            self.update_chat_history(command, str(e) + '\n' + self.task_manager.get_help(), 'error_format')

    def start(self):
        self.window.mainloop()


class TaskManager:
    def __init__(self):
        self.items = [
            ['task 1', True],
            ['task 2', False],
            ['task 3', True]
        ]

    def get_help(self):
        return 'help:\n...'

    def execute_command(self, command):
        if command == 'help':
            return self.get_help()
        elif command.startswith('add '):
            self.items.append([command[4:], False])
            return 'task added'
        else:
            raise Exception('Command not recognized')


GUI(TaskManager()).start()
```
</panel>
</div>

<include src="extensions-fragment.md" />
</div>
