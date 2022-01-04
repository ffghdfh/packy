# packy
Add your own files to the packy manager here!  
**Here are the current commands:**  
`packy list` lists all the files / packages that are available to download  
`packy install <file name>` installs a specific file / package  
`packy search` search for specific file / package  
`packy installed` list all the installed files  
`packy remove <file name>` remove a specific file / package  
`packy autoremove` remove any leftover files from any removed packages, but unneeded in most cases because remove *should* in theory get rid of everything

there are also a few **options** you can use  
make sure you put the options at the very end of the line, or packy might break!  
`-y` if there's anything that requires entering y or n, it'll automatically choose y  
`-r` you can install code with a raw.githubconsent.com link with this, example: `packy install -l raw.github.consent.com/epic/file.file`  
`-f` you can force download a package that has been already downloaded, this might fix some issues if you messed with the code in any of the packages  
`-q` this disables most of the install log but will keep "Downloading package..." and "Finished downloading." and will show any error code if couldn't download  
`-shut` this disables ***ALL*** of the output, idk why you would need this
`-v` shows current packy version  

IF you'd like to update packy or if it has issues, or just wanna do it for fun, you can reinstall packy with the following command:  
`packy reinstall`

# adding your own file / package
**Here's how you can add your own file / package:**   
First, add all your files to a github repository. Next, create a file in the root folder named (insert package name).nya (replace the "insert package name" with the package name lol)   
Next, specify the path and name of the python file to run first when running the program, like this: (if the file is in the root folder then just write the name of the file)
`path/to/file.py` or if it's in the root folder of the repo then just enter the file name: `file.py` (write all of this in the first line of the file)
if you have any modules that have to be installed (stuff you need to use pip install for), type the specific names of the packages separated with commas into the second line, like this:
`ursina,pygame,pyneapple`
so it should look something like this :D
```
path/to/file.py
pynedog,django
```
and then open up packs.nya in this repo, make a new line and then type in the name of your package followed by the link to your repository. something like this:
```
crap https://someoneelse'srepo.lol
pee https://yourrepo.com
```
and that should be it! If you wanna check if it was actually added, just do `packy list`, every time you run the command, it checks the packs.nya file so no need to update or anything.
