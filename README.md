# command-prompt-basics
I was told i should write this for future reference. I made the mistake of trying to use certain unix commands (im a bash linux and bsd user) in command prompt. Apparently `touch` is not a thing :(. Also wth why backslashes 😢.
# commands and their properties
Before you begin, open the app called `terminal`. Note that command prompt is not the same as powershell. (they are made with different purposes in mind).
| command name  | name | desc | details |
-----|------------------|-------------------------------------------------------------|--------------------------------------------------|
| cd | change directory | it changes the directory it is looking at to the stated one | sample usage: `cd Downloads\Photos` (goes to Downloads\Photos)<br><br>`cd ..` (goes backwards in the file tree).<br><br>If your file name has spaces you can use strings: `cd "My files"` |
| mkdir | make directory | it creates a directory using flags can help you in other ways | read more [here](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/mkdir) |
| rmdir | removes directory | it deletes a directory using flags can help you in other ways | read more [here](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/rmdir) |
| dir | directory | lists all directories in a folder | `dir` command. The `dir` (directory) command lists directory contents, including files and subdirectories. |

# unix (OSx, linux, bsd and more...)
Note that this was tested in a bash environemnt, so you might have to check if you are using bash, zsh or whatever.          
I love zsh, better floating point support and more, but it breaks POSIX compliance. Which sometimes gets me.
| command name | name | desc | details |
-----|------------------|-------------------------------------------------------------|--------------------------------------------------|
| `~/` | home | shorthand | `cd ~/` goes to the home directory <br> mkdir `~/potato` creates a folder called potato in the home folder |
| cd | change directory | It changes the current working directory to the one that is stated | same as the one above (however you need to use `/` instead of `\`). |
| mkdir | make directory | it creates a directory using flags can help you in other ways | `mkdir documents` creates a file called documents <br> `mkdir -p ~/documents/school` creates a folder called school in documents <br> `mkdir banana potato` creates folders banana and potato |
| rmdir | removes directory | it deletes a directory using flags can help you in other ways, if there are things in the folder it will throw a warning, use rm for that instead | `rmdir documents` removes folders <br> [read more here](https://www.ibm.com/docs/tr/aix/7.2?topic=r-rmdir-command) |
| touch | creates a file | creates a file | `touch grass.txt` creates a file called grass |
| rm | remove | used to remove files and folders | `rm -rf potato` removes folder potato and all contents in it <br> `rm potato.txt` deletes a file potato.txt |

# powershell vs command prompt
CMD has no access to libs, unlike PowerShell, which has full access to . NET libraries.
