Hello!

We wanted to put together a quick document to help you make sure you’ve set up your environment correctly. First we’ll make sure you have python installed so you can run the files you create in this class, then we’ll recommend a code editor for you.

# Python Install

We’re going to point you to the Treehouse videos that were linked in the syllabus to get python set up. Pick the select the type of computer you have and make your way through the course.

[**Setting up a Local Python Environment (Windows)**](https://teamtreehouse.com/library/setting-up-a-local-python-environment-windows)

[**Setting up a Local Python Environment (Mac)**](https://teamtreehouse.com/library/setting-up-a-local-python-environment-mac)


# VS Code

Next we’re going to have you install Visual Studio Code. We’re recommending this code editor for the course, but you’ll find a lot of people also write python using [Pycharm](https://www.jetbrains.com/pycharm/) and several other options.

To get started, please follow the steps for your computer type:

[Visual Studio Code on macOS](https://code.visualstudio.com/docs/setup/mac)

[Visual Studio Code on Windows](https://code.visualstudio.com/docs/setup/windows)


Before we get any further, let’s decide where we want to keep your code for Code Louisville. I personally like having a folder called Code that keeps all my projects in one place.

Once you decide, create a new folder in that place called `test_setup`. Next navigate to within that folder in command prompt (windows) or terminal (mac) and run the command to create a virtual environment:

```
    python3 -m venv my-first-venv
```

Now we can write some code! If you open up VS Code, you should see something like this:

![welcome page](https://code.visualstudio.com/assets/docs/getstarted/tips-and-tricks/welcome_page.png)


Click Open Folder, and then find the test_setup folder we just created. Now you should see a file explorer pop up on the left for our folder. Next we’ll create our file.

Go ahead and click new file and then paste in this code:

```
    from datetime import date
    for i in range(1, 4):
        print(i)
    today = date.today()
    print("Today is " + str(today) + " and it's a great day to code!")
```

Save the file by pressing ctrl+s (cmd+s on mac) or by clicking File > Save. Save it within our test_setup folder as `first_script.py`.

Once you save it, you should see two things happen. First, VS Code now highlights parts of the code to make it easier to read. Second, a pop-up should have shown up in the bottom right asking you to install the Python extension for VS Code.

If you didn’t see the pop up to install python for VS Code, you can install it by clicking on the extensions icon on the left side and searching for python. It should be the top result, and you can click and install it.

![](https://paper-attachments.dropbox.com/s_48AD6C49DA2FB6C9B83F9DC9DDBA49906D278A6F52FEE65CCCF102D0A2F55044_1589035333914_Screenshot+from+2020-05-09+10-36-10.jpg)


There are thousands of different extensions for VS Code that make it really power. This is how you’ll install them later.

If we try to run the script now, you’ll see a pop up in the bottom right that you need to select a Python interpreter. You can do that by clicking the part of the bottom status bar that says “Select Python Interpreter”.

![](https://paper-attachments.dropbox.com/s_48AD6C49DA2FB6C9B83F9DC9DDBA49906D278A6F52FEE65CCCF102D0A2F55044_1589037841845_Screenshot+from+2020-05-09+11-22-57.png)


Once you click it you should see a list appear with 2 or 3 options. One of the options should include `('my-first-venv': venv)` in the title. Select that one so VS Code knows what to run our code with and what packages we have installed.

When you click it, you might see a few more pop-ups about things you don’t have installed (pylint, pycodestyle, pytest). These are all useful python packages that VS Code can use to help you write your code. You can go ahead and install this one at a time.

Now you can run your code! Click Run on the top bar and select “Run without Debugging” and you should see the program get run, and then the follow output appear:
```
    1
    2
    3
    Today is 2020-05-09 and it's a great day to code!
```
