# packy
Welcome! Here's a quick overview on how to use packy and it's functions!  
**Functions:**  
`packy.install(pack)` - Installs a package by a name  
`packy.remove(pack)` - Removes an installed package by a name  
`packy.installurl(pack)` - Installs a package by github url (there's some issues with it, more on that later)  
`packy.update()` - Updates all of the variables with the latest values  
`packy.isinstalled(pack)` - checks if a certain package is installed, returns either True or False, example:  
```py
if packy.isinstalled("coolpack"):
  #do stuff if it's true
else:
  #do stuff if it isn't true
 ```
 `packy.search(pack)` - Searches for a package in the official list, returns the results as a list  
**Variables:**  
`packy.installed[]` - A list containing every single installed package  
`packy.packs[]` - A list containing every official package in the packages.nya file  
# How to add your own
1. Upload your pack onto a github repo  
2. Open the `packs.nya` file  
3. Type in the required information like this:  
```
name "https://github.com/link/to/repo" (anything,you,have,to,pip,install,separated,by,commas) [mainfile.py]
```
here's an example:  
```
emmatext "https://github.com/ffghdfh/emma-text-editor" (colorama,playsound) [emma.py]
```
# some issues
Currently the biggest issue so far is installing by url, because it won't install any required dependencies, and when running for the first time, the user has to specify which file to run (but it'll get saved so you don't have to enter it again)
