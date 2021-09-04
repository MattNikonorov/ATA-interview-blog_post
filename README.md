# How to edit files in terminal with the 'nano' command

Sometimes, when working with remote files inside an AWS EC2 instance or any other type of virtual machines running in the cloud, 
you'd probably find out that you aren't able to directly edit the files the way you are able to adit files in your trusty code editor like VScode.

**Unbenownst to quite a few people, there is in fact a way to directly edit files inside a virtual machine without using third party applications or addons!**

Using the 'nano' command, you can easily edit and work with remote files inside virtual machines inside your terminal. 

## The file operations with the nano command
Here I'll be showing you how to work with the 'nano' command in terminal, as well as demonstrating and explaning the basic, as well as more advanced operations with the 'nano' command.

### Installation and working with 'nano'
If you don't already have nano installed, you can install it with:

Mac: `brew install nano`

Linux/Debian/Ubuntu: `sudo apt install nano`

CentOS/Fedora: `yum install nano`

***********

**To open a file with nano, you can simply run something like `nano filename.txt` and your terminal will open up and display the file's contents**
![The nano command](https://github.com/MattNikonorov/ATA-interview-blog_post/blob/main/nanodemo.png)


To edit files with the nano command works pretty much the same as any other code editor, except the fact that you cannot select text and can only remove chunks of text or code by spamming the backspace key the way you would in the terminal.
![Editing with nano](https://github.com/MattNikonorov/ATA-interview-blog_post/blob/main/nanoediting.gif)

### Basic operations
**Saving and Discarding new edits**
To save or discard any edits that you've made to a file with nano, first you will have to press "ctrl + x" on your keyboard


### More advanced operations


## Tips and tricks


## Quirks and potential downsides of the 'nano' command

