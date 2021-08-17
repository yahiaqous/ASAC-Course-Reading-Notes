# Automation

## Regular Expressions

Regular Expressions, often shortened as regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not. In Python, regular expressions are supported by the re module.

- **Basic Patterns**: Ordinary Characters - Ordinary characters are the simplest regular expressions.

- **Wild Card Characters**: Special Characters - characters that do not match themselves as seen but have a special meaning when used in a regular expression.

## Shutil

The shutil module includes high-level file operations such as copying and archiving.

- **Copying Files** - **_copyfile()_** copies the contents of the source to the destination.

- **Copying File Metadata** - By default when a new file is created under Unix, it receives permissions based on the umask of the current user.

- **Working With Directory Trees** - shutil includes three functions for working with directory trees.

- **Finding Files** - The **_which()_** function scans a search path looking for a named file.

- **Archives** - Python’s standard library includes many modules for managing archive files such as tarfile and zipfile.

- **File System Space** - **_disk_usage()_** returns a tuple with the total space, the amount currently being used, and the amount remaining free.
