# How to edit files in terminal with the 'nano' command

Sometimes, when working with remote files inside an AWS EC2 instance or any other type of virtual machines running in the cloud, 
you'd probably find out that you aren't able to directly edit the files the way you are able to edit files in your trusty code editor like VScode.

**Unbenownst to quite a few people, there is in fact a way to directly edit files inside a virtual machine without using third party applications or addons!**

Using the 'nano' command, you can easily edit and work with remote files inside virtual machines inside your terminal. 

## Prerequisitries
If you don't already have nano installed on your virtual machine, you can install it with:

Mac: `brew install nano`

Linux/Debian/Ubuntu: `sudo apt install nano`

CentOS/Fedora: `yum install nano`

## Working with nano

Here I'll be showing you how to work with the 'nano' command in terminal, as well as demonstrating and explaning the basic, as well as more advanced operations with the 'nano' command.


**Once you've SSHed into your virtual machine running on AWS or Azure, to open a file with nano, you can simply run something like `nano filename.txt` and your terminal will open up and display the file's contents**
![The nano command](https://github.com/MattNikonorov/ATA-interview-blog_post/blob/main/nanodemo.png)


Editing files with the nano command works pretty much the same as any other code editor, except the fact that you cannot select text and can only remove chunks of text or code by spamming the backspace key the way you would in the terminal.
![Editing with nano](https://github.com/MattNikonorov/ATA-interview-blog_post/blob/main/nanoediting.gif)

### Basic operations
**Saving and Discarding new edits**
To save or discard any edits that you've made to a file with nano, first you will have to press "ctrl + x" on your keyboard and then select either 'No' to discard new edits or 'Yes' to save new edits and finally hit enter.
![Exit](https://github.com/MattNikonorov/ATA-interview-blog_post/blob/main/nanodemo2.png)
![Yes or No](https://github.com/MattNikonorov/ATA-interview-blog_post/blob/main/nanodemo3.png)

### More advanced operations
**Here are the more advanced operations you can perform with the nano command**

#### Cut and Uncut
By putting your cursor on the line which you want to cut, and then press "ctrl + k" on your keyboard, you will be able to cut that line out of your file:
![ctrl + k](https://github.com/MattNikonorov/ATA-interview-blog_post/blob/main/ctrlk.png)

![cut out piece of text](https://github.com/MattNikonorov/ATA-interview-blog_post/blob/main/cutout.png)

Then when pasting the cut out piece of text or code, you can paste it back in by putting your cursor on the line that you want to paste the text/code into and press "ctrl + u":
![ctrl + u](https://github.com/MattNikonorov/ATA-interview-blog_post/blob/main/ctrlu.png)

#### Position
To get the current position of your cursor within the file, you can press "ctrl + c" to find your cursor's position:
![ctrl + c](https://github.com/MattNikonorov/ATA-interview-blog_post/blob/main/ctrlc.png)


#### Search
To find a word or piece of text within your file with nano, you can press "ctrl + w". If found, nano will redirect your cursor to the first character of the specified piece of text:
![ctrl + W](https://github.com/MattNikonorov/ATA-interview-blog_post/blob/main/ctrlw.png)

![Position of "Matt"](https://github.com/MattNikonorov/ATA-interview-blog_post/blob/main/Mattpos.png)


## Quirks and potential downsides of the 'nano' command

Even though the nano command is the easiest, fastest and most straight-forward way of editing remote files,

as you might have guessed, editing files inside terminal isn't exactly a hassle-free experience, and comes with a few downsides which are:

1. You can't cut multiple lines of text or code
2. No syntaxing
3. Getting your cursor to a specific position in the file takes slower than a normal code editor because you can't drag your cursor to that position, but have to get there manually.


## Conclusion

In summary, if you are working with remote files inside virtual machines, then the nano command is definetely the easiest, fastest and most straight-forward way of editing those files, creating a much faster way of working with remote code and virtual machines.
