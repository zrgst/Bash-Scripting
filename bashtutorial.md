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


```bash
#!/bin/bash
echo "Today is:"
cal
date
exit
```

link to the video:
https://youtu.be/KG97VzMjfMg?si=6nqJUYCVcVi0niBs&t=655


if you creat a bin folder in yout home directory and rebbot the system, it will automatically be added to your $PATH . if this does not work the solution is in the end of the video.


