# packy
Add your own files to the packy manager here!  
**here are the current commands:**  
`packy list` lists all the files / packages that are available to download  
`packy install <file name>` installs a specific file / package  
`packy search` search for specific file / package  
`packy installed` list all the installed files  
`packy remove <file name>` remove a specific file / package  
`packy autoremove` remove any leftover files from any removed packages, but unneeded in most cases because remove *should* in theory get rid of everything

there are also a few **options** you can use  
`-y` if there's anything that requires entering y or n, it'll automatically choose y  
`-r` you can install code with a raw.githubconsent.com link with this, example: `packy install -l raw.github.consent.com/epic/file.file`  
`-f` you can force download a package that has been already downloaded, this might fix some issues if you messed with the code in any of the packages  
`-q` this disables most of the install log but will keep "Downloading package..." and "Finished downloading." and will show any error code if couldn't download  
`-shut` this disables ***ALL*** of the output, idk why you would need this
`-v` shows current packy version  

IF you'd like to update packy or if it has issues, or just wanna do it for fun, you can reinstall packy with the following command:  
`packy reinstall`
