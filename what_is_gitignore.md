#What is .gitignore?

A `.gitignore` file tells git to ignore files and directories before making a commit.

##Why?

Not all files are written by us, but are *generated* by our code, and therefore shouldn't be added to a repo. Examples include `.class` files in Java or `.pyc` files in Python.

Some files may contain sensitive data, like passwords.



##How do you use it?

In Terminal:

```
$ touch .gitignore
$ subl .gitignore
```
And add to the file:

```
# comment like this
###################
*.class               # ignore all files of type 'class'
*.pyc                 # ignore all files of type 'pyc'
Documentation/*.html  # ignore all 'html' files in /Documentation/
```
File structure is relative to the directory `.gitignore` is stored in.

##Sources

* https://git-scm.com/docs/gitignore
* http://stackoverflow.com/questions/13675216/why-should-i-use-gitignore
* https://www.quora.com/Whats-the-purpose-of-a-gitignore-file
* http://gitready.com/beginner/2009/01/19/ignoring-files.html