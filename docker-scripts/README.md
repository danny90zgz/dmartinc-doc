# Docker Scripts

## Usage

### Linux

Just copy+paste (at a `$PATH` path directory if you want to have it available everywhere) and grant `execute permission`.
   
Example:

    * Allocate at `/usr/local/bin`.
    * chmod +x /usr/local/bin/THE_SCRIPT
    
### Windows

Although these are `bash` scripts, they can be executed at a Windows environment with `Git Bash` software. 

Just allocate them at `PATH_TO_GIT\Git\usr\bin` and use them from `Git Bash` console.  

## Available scripts


### [dockerEnter](dockerEnter)
Just access some container.

### [dockerEnterWin](dockerEnterWin)
Just access some container (at windows host).

### [dockerLogs](dockerLogs)
Shows container logs until it's stopped (`CTRL+C`).

### [dockerRmiDangling](dockerRmiDangling)
Removes each dangling image.
 
A dangling image just means that a new build of the image have been created, but it was not given a new name (was given the old/same name). 

So the old image becomes the "dangling image". Those old image are the ones that are untagged and displays "<none>" on its name when you run `docker images`.

### [dockerRmStoppedContainers](dockerRmStoppedContainers)
Removes each stopped container.

### [dockerShow](dockerShow)
Shows docker system information by sequentially executing `docker images`, `docker ps -a` and `docker system df`.