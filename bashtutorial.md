# Tutorial on making scripts in bash

*This tutorial is base on th video from Joe Collins on YouTube, please check out his channel. He has a lot of great Linux content *

To create a script in terminal you can use the "cat" command.
This will allow you to add mulitple lines to the script directly from
the terminal. But with very limited functionality in terms of editing mistakes.
as soon as the line is finished and you continue to the next line, you can not
edit the previous line. Then you would have to open it in a text-editor to fix mistakes.

In your terminal navigate to the folder where you want your script to be stored.
Use the following command to start making your script:

```bash
cat > yourscriptname.sh
```
the line below your command will be your tex editor. so there you will enter your script commands.

If you make a mistake one one of the lines and need to start over, use the shortcut "Ctrl-c" to Return to your terminal,  nothing will be saved and you can run the command again to make your script.

First we need to define the interpreter for the script.

int the first line of you script you will Write the following line:

```bash
#!/bin/bash
```

this tells your computer that this script wil be interpreted by the bash interpreter.

After this you can add the actual script. In the example from the video he makes a calendar script that shows a calendar fo the current month and teh current date and time.

Here is the entire script:

```bash
#!/bin/bash
echo "Today is:"
cal
date
exit
```

If you try to run the script now it wil not run. first you need to change permissions on the file.
This can be done with the "chmod" command:

```bash
chmod 755 today.sh

```
or

```bash
chmod +x today.sh
```

now the script will run. but not by just writing the name in the terminal. The new script is not in your $SOURCES yet.
To run it now you have to use this command:

```
./today.sh
```

Congratulations, you have now made your first script. Later we will explore how to add it to your sources so it can be run woth a single word command like all the other bash commands we use every day!

link to the video:
https://youtu.be/KG97VzMjfMg?si=6nqJUYCVcVi0niBs&t=655


if you creat a bin folder in yout home directory and rebbot the system, it will automatically be added to your $PATH . if this does not work the solution is in the end of the video.


