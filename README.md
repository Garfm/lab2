# CS190 Lab 2 - What Does the _____ Say? #

The purpose of this lab is to teach the basics of using the Terminal. After you finish this lab, you will be able to manipulate files within your CS account (or any UNIX machine) with ease.

Before starting the lab, please navigate to the [Lecture 1 Cheat Sheet](https://github.com/purduecs190/syllabus/blob/master/lecture01-basic-terminal-commands.md) to review all the common commands.

## The Lab ##

Throughout this lab we will give you specific environment parameters and you will have to give the appropriate command to fulfill the action we ask of you. All answers should only contain one primary command (mv, cp, rm, etc.). We will ask you to complete tasks based on a fresh `~/cs190lab2` folder, so it may be wise to be run the "Magic Command" before working on each task.


### The Magic Command ###
    cd; curl -sL https://raw.githubusercontent.com/PurdueCS190/lab2/master/lab2init | /bin/bash

The command above, when run in a terminal, will create a folder structure (shown below) located within your home directory. Throughout this lab, you will be moving these files around, deleting some, and duplicating others. If at any time you want to reset to the default solder structure, you can run the "Magic Command" again. It will delete the old one and give you a new one to work with.


### Folder Structure ###
Below is the folder structure that is generated from running the "Magic Command". It is incorrect (ie. dog sounds in the cat/sounds folder). Throughout this lab, you will write terminal commands that fix some of the mistakes.

        cs190lab2/
        ├── cat/
        │   ├── famous cats/
        │   │   ├── Garfield
        │   │   ├── Grumpy Cat
        │   │   └── Tom
        │   ├── sounds/
        │   │   ├── cat_hiss
        │   │   ├── dog_bark
        │   │   ├── dog_howl
        │   │   └── dog_woof
        │   ├── cat_meow
        │   └── cat_purr
        │
        ├── dog/
        │   ├── famous cows/
        │   │   ├── Air Bud
        │   │   ├── Blue
        │   │   └── Clifford
        │   └── sounds/
        │
        ├── fox/
        │   ├── famous foxes/
        │   │   ├── Fox McCloud
        │   │   ├── Pablo the Little Red Fox
        │   │   └── Swiper
        │   └── sounds/
        │       ├── ding
        │       ├── ding ding
        │       └── ding ding ding
        │
        └── human/
            ├── famous humans/
            │   ├── Albert Einstein
            │   ├── Michael Jordan
            │   └── Kirby Kohlmorgen
            └── sounds/
                ├── human_cry
                ├── human_laugh
                └── human_whistle


## Rules and Example Task ##
There are 6 tasks, and you will write 6 **one line** terminal commands that fulfill that task. Each command may only contain **ONE BASE COMMAND** (mv, ls, cp, rm, etc). You may not combine different base commands (cd, mv) into one response, and you may not combine two of the same base commands (mv, mv) into one response. Examples of this are below in the *Task 0 Example*.

All commands should be recorded in answers.txt. To download the answer sheet below, right-click on the file and click "Save File As" and save it to your **Downloads** folder.

[answers.txt Download Link](https://raw.githubusercontent.com/PurdueCS190/lab2/master/answers.txt)

> NOTE: Do not save this file within `~/cs190lab2` because that folder and all of its contents will be erased each time you run the "Magic Script"


#### Example: Task 0 ####

    Working Directory:  ~/cs190lab2/

    Desired Action:     print out only the names of the normal folders and files in the cat/ folder and the dog/ folder

    Write the answer under the Task 0 block. Make sure not to put '#' before your answer.

#### Example: Task 0 Sample Answer ####
    # -----------------
    # Task 0 Answer
    # -----------------
    ls cat dog

This above answer is allowed because it is on one line and only contains one base command, which in this case, is a single `ls`. Example invalid responses are shown below.

    # Not allowed response because it is two lines and contains two "ls" commands.
    ls cat
    ls dog

    # Not allowed response because it contains two "ls" commands.
    ls cat; ls dog

    # Not allowed because it is four lines and contains more than one base command.
    cd cat
    ls
    cd ../dog
    ls


## Assigned Tasks ##

#### Task 1 ####

    Working Directory:  ~/cs190lab2/

    Desired Action:     remove the human/ folder from the working directory

    Write the answer under the Task 1 block. Make sure not to put '#' before your answer.

#### Task 2 ####

    Working Directory:  ~/cs190lab2/

    Desired Action:     create a folder named mouse/ with the subfolders [sounds] and [famous mice]  
                        (may not use MORE THAN TWO path arguments)
                        (mkdir one/ two/ three/  # this has three path arguments)

    Write the answer under the Task 2 block. Make sure not to put '#' before your answer.

#### Task 3 ####

    Working Directory:  ~/cs190lab2/

    Desired Action:     move the dog sounds from the cat/sounds/ folder to dog/sounds/ folder
                        (may not explicitly list files in command)

    Write the answer under the Task 3 block. Make sure not to put '#' before your answer.

#### Task 4 ####

    Working Directory:  ~/cs190lab2/dog

    Desired Action:     rename the folder [famous cows] to [famous dogs]

    Write the answer under the Task 4 block. Make sure not to put '#' before your answer.

#### Task 5 ####

    Working Directory:  ~/cs190lab2/fox/sounds

    Desired Action:     copy [ding ding ding] to a new file named [ding ding ding ding]

    Write the answer under the Task 5 block. Make sure not to put '#' before your answer.

#### Task 6 ####

    Working Directory:  ~/cs190lab2/cat/sounds

    Desired Action:     move files that are cat sounds from parent directory (~/cs190lab2/cat)
                        to the current working directory
                        (may not use definite paths such as ~/cs190lab2/cat)

    Write the answer under the Task 6 block. Make sure not to put '#' before your answer.


#### End of Lab ####
That is the last of the tasks. You can raise your hand and get checked off, but please do the `Extra\ Fun*` sections before you leave.


## Extra Fun ##
Did you realize that you made a shell script that is actually runnable? As you saw in the default folder structure, files were all over the place and things were not in the correct locations, nor did they have the correct names. If you have the correct answers, you are able to run your answers.txt file as a script and it will result in a folder structure that makes sense.

If you want to run your answers.txt as a script, run the following command in the terminal:

    bash answers.txt

Now look at the entire folder structure of your `~/cs190lab2` folder by running the following command:

    ls -al ~/cs190lab2/*/*


## More Extra Fun ##
View the [source](https://github.com/PurdueCS190/lab2/blob/master/lab2init) of the Magic script. You know almost everything that is going on in this script!

## Quiz 2 (optional) ##

If you want to get a head start on Quiz 2 do it during lab!
** Due Sunday, September 20 at 11:59p **

1. Go to [Blackboard](https://mycourses.purdue.edu).

2. Login with your career account.

3. Go to Fall-2014-CS-19000-TLE under "My Courses."

4. Click Quizzes, Quiz 2 - Basic Terminal Commands, Begin.
<br>

----

*If you find any bugs within the code or misspellings in the write-up, please tell the TA. Thanks!*
