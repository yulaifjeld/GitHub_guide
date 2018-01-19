# GitHub_guide

This is a personal guide for using git and GitHub. 

## Creating a new repository

Create a **new directory** by executing the **init** command in the terminal: 

```
git init
```

This creates the new repository. 

## Checking out a repository

To create a **copy** of an already existing repository, run the following command in the terminal: 

```
git clone /path/to/repository
```

If you are using a remote server, use the following command: 

```
git clone username@host:/path/to/repository
```

## About the repository

The repository consists of three **trees** (or structures). 
	* Working Directory --> wherein the actual files are kept
	* Index --> a staging area.
	* HEAD --> a pointer to the last commit made. 

## **add** and **commit**

These commands are useful for proposing changes by adding them to your **Index**. 

```
git add <filename>
```

Adds a specific file to the Index. 

```
git add . 
```

Adds all proposed changes to the Index. 

If you are happy wiht the changes, use the command **commit**: 

```
git commit -m "Commit message"
```

The -m option allows you to include a message with the commit. 

The file(s) are now commited to the **HEAD**, but are still not in your remote repository. 

## **push**

In order to actually reflect the changes in your repository, you need to use the **push** command. 

Up to this point, the changes only exist in the **HEAD**. Use the following command to send the changes to your repository: 

```
git push origin master
```

There are many options for **push** in git. 