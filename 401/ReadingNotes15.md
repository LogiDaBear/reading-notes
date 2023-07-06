# AUTOMATION

- [Python RegEx](https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial)
- [shutil](https://pymotw.com/3/shutil/)
- [os](https://pymotw.com/3/os/)

## How can you use regular expressions in Python to search for specific patterns in a string, and what is the primary module to work with them?

primary module is `re`
You can easily tackle many basic patterns in Python using ordinary characters. Ordinary characters are the simplest regular expressions. They match themselves exactly and do not have a special meaning in their regular expression syntax.

Examples are 'A', 'a', 'X', '5'.

## What is the purpose of the shutil module in Python, and provide an example of a common use case for file or directory management with this module?

the purpose is to provide a high-level file operation such as copying and archiving

below is an example of a common use case from the documentation:

### Working With Directory Trees
shutil includes three functions for working with directory trees. To copy a directory from one place to another, use copytree(). It recurses through the source directory tree, copying files to the destination. The destination directory must not exist in advance.

shutil_copytree.py
import glob
import pprint
import shutil

print('BEFORE:')
pprint.pprint(glob.glob('/tmp/example/*'))

shutil.copytree('../shutil', '/tmp/example')

print('\nAFTER:')
pprint.pprint(glob.glob('/tmp/example/*'))
The symlinks argument controls whether symbolic links are copied as links or as files. The default is to copy the contents to new files. If the option is true, new symlinks are created within the destination tree.

$ python3 shutil_copytree.py

BEFORE:
[]

AFTER:
['/tmp/example/example',
 '/tmp/example/example.out',
 '/tmp/example/file_to_change.txt',
 '/tmp/example/index.rst',
 '/tmp/example/shutil_copy.py',
 '/tmp/example/shutil_copy2.py',
 '/tmp/example/shutil_copyfile.py',
 '/tmp/example/shutil_copyfile.py.copy',
 '/tmp/example/shutil_copyfileobj.py',
 '/tmp/example/shutil_copymode.py',
 '/tmp/example/shutil_copystat.py',
 '/tmp/example/shutil_copytree.py',
 '/tmp/example/shutil_copytree_verbose.py',
 '/tmp/example/shutil_disk_usage.py',
 '/tmp/example/shutil_get_archive_formats.py',
 '/tmp/example/shutil_get_unpack_formats.py',
 '/tmp/example/shutil_make_archive.py',
 '/tmp/example/shutil_move.py',
 '/tmp/example/shutil_rmtree.py',
 '/tmp/example/shutil_unpack_archive.py',
 '/tmp/example/shutil_which.py',
 '/tmp/example/shutil_which_regular_file.py']
copytree() accepts two callable arguments to control its behavior. The ignore argument is called with the name of each directory or subdirectory being copied along with a list of the contents of the directory. It should return a list of items that should be copied. The copy_function argument is called to actually copy the file.

shutil_copytree_verbose.py
import glob
import pprint
import shutil


def verbose_copy(src, dst):
    print('copying\n {!r}\n to {!r}'.format(src, dst))
    return shutil.copy2(src, dst)


print('BEFORE:')
pprint.pprint(glob.glob('/tmp/example/*'))
print()

shutil.copytree(
    '../shutil', '/tmp/example',
    copy_function=verbose_copy,
    ignore=shutil.ignore_patterns('*.py'),
)

print('\nAFTER:')
pprint.pprint(glob.glob('/tmp/example/*'))
In the example, ignore_patterns() is used to create an ignore function to skip copying Python source files. verbose_copy() prints the names of files as they are copied then uses copy2(), the default copy function, to make the copies.

$ python3 shutil_copytree_verbose.py

BEFORE:
[]

copying
 '../shutil/example.out'
 to '/tmp/example/example.out'
copying
 '../shutil/file_to_change.txt'
 to '/tmp/example/file_to_change.txt'
copying
 '../shutil/index.rst'
 to '/tmp/example/index.rst'

AFTER:
['/tmp/example/example',
 '/tmp/example/example.out',
 '/tmp/example/file_to_change.txt',
 '/tmp/example/index.rst']
To remove a directory and its contents, use rmtree().

shutil_rmtree.py
import glob
import pprint
import shutil

print('BEFORE:')
pprint.pprint(glob.glob('/tmp/example/*'))

shutil.rmtree('/tmp/example')

print('\nAFTER:')
pprint.pprint(glob.glob('/tmp/example/*'))
Errors are raised as exceptions by default, but can be ignored if the second argument is true, and a special error handler function can be provided in the third argument.

$ python3 shutil_rmtree.py

BEFORE:
['/tmp/example/example',
 '/tmp/example/example.out',
 '/tmp/example/file_to_change.txt',
 '/tmp/example/index.rst']

AFTER:
[]
To move a file or directory from one place to another, use move().

shutil_move.py
import glob
import shutil

with open('example.txt', 'wt') as f:
    f.write('contents')

print('BEFORE: ', glob.glob('example*'))

shutil.move('example.txt', 'example.out')

print('AFTER : ', glob.glob('example*'))
The semantics are similar to those of the Unix command mv. If the source and destination are within the same file system, the source is renamed. Otherwise the source is copied to the destination and then the source is removed.

$ python3 shutil_move.py

BEFORE:  ['example.txt']
AFTER :  ['example.out']

## Compare and contrast the os and shutil modules. When would you choose to use one over the other?

you would choose to use the os module when you need fine-grained control over file system operations or when you want to perform tasks beyond file manipulation, such as process management. On the other hand, you would opt for the shutil module when you need high-level file operations, especially for tasks like copying, moving, and deleting files and directories, as it provides a simpler and more convenient API.

## Things I want to know mo aboot
how the heck does it work