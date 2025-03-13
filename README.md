# my_pwd:
## steps of implementation:
### searched for a file that contains my working directory, which was a link i found in /proc/self/cwd
### i tried opening with open() and read() but read() couldn't access it and returned -1, since read() works with normal files not links
### instead, i searched with other alternatives for read() and i found readdir() and readlink()
### readlink() was much easier to use than readdir(), since there is no complicated implementation like using structures and custom data types like DIR
### i read also that it is not neseccary to open() it first, so i did,'t try to do it
