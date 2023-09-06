## Bash Practice 

1. Create a new directory called `ds219` under the /tmp directory.

2. Look up the touch program. The man program is your friend.

3. Use touch to create a new file called `myscript` in `/tmp/ds219`.

4. Write the following into that file, one line at a time:

```bash
#!/bin/sh
curl --head --silent  https://github.com/DS219/resources/blob/main/LICENSE
```

5. Try to execute the file, i.e. type the path to the script (/tmp/ds219/myscript) into your shell and press enter. Understand why it doesn’t work by consulting the output of ls (hint: look at the permission bits of the file).

6. Look up the chmod program (use `man chmod`).

7. Use chmod to make it possible to run the command `/tmp/ds219/myscript` How does your shell know that the file is supposed to be interpreted using sh? Hint: Run a google search for "what is the bash shebang line" for more information.

8. Use | and > to write today's date into a file called `today.txt` in your home directory.

9. Write a command that _appends_ a list of all files in your home directory to `./today.txt`

10. Use `top` or `ps` commands to list of all processes owned by you (not root) running on your machine sorted by CPU usage. To exit from the `top` cmd, enter `Ctrl-c`


When finished, you can remove `today.txt` practice file (you want to clean up clutter on your system!)

```
rm today.txt
```

*This is heavily borrowed from https://missing.csail.mit.edu/2020/course-shell/*
