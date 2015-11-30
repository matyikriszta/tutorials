---
layout: page
title: More command line
---

In the previous command line tutorial we have learned how to:

- print out the current directory you are in (pwd),
- list the contents of a directory (ls),
- navigate the directory structure of your computer (cd),
- create new directories (mkdir),
- create new files (touch)

In this tutorial we will learn more advanced commands that will allow us to delete, copy and move things around.

## Example 1: deleting files and directories

We have learned how to create files and directories, now it's time to learn how to delete them. We have two commands that let's us do just that. Let's start by creating a `temp` folder in the home directory of your machine. Navigate inside this directory and create three new .txt files.

### `rm` or removing files

Inside the temp folder type:

```bash
$ rm name-of-your-file
```

Now check out the contents of the directory by typing `ls`. As you can see the name-of-your-file file has been deleted.

We can delete more than one files. Type:

```bash
$ rm name-of-your-file.txt name-of-your-other-file.txt
```

Now check the contents of your directory. It's empty! 

### `rmdir` or removing directories

Still in the temp folder, let's create an empty folder and a folder with a file in it.

```bash
$ rmdir the-empty-folder
```

> What happened? Check the content of your directory

```bash
$ rmdir the-folder-with-stuff
```

What happened there? The machine wouldn't allow you to delete a non empty folder. To delete a folder with files in it, you have to first remove all the files and then delete the folder. Type:

```bash
$ rm -rf the-folder-with-stuff
```
> What happened now?

## Example 2: copying and renaming files

### `cp` or copying files

Still in the `temp` folder, type:

```bash
$ cp one-file.txt other-file.txt
```

```bash
$ cp other-file.txt folder
```

```bash
$ cp -r folder new-folder
```

### `mv` or renaming files

- mv

## Example 3: viewing a file in the terminal

Sometimes you might want to preview a file in your terminal. You can do that in two ways, by using either `less` or `cat`. Type:

```bash
$ less file.txt
```

`less` will give you a preview of your file that you can page through by hitting enter. You can get out of this preview by typing `q` after the `:`.

Another way of printing a file to the terminal is by using `cat`. Type: 

```bash
$ less file.txt
```

> What happened there? How does `cat` differ from `less`?


