# FunRAR
This shell program finds all WinRAR split archives in your specified working directory, extracts them, and copies the extracted files to wherever you want them! No more dealing with multiple split archives, unrar-ing multiple .r00 files and taking 30 minutes to move everything.

### Installation

 1. Clone the repo: `git clone https://github.com/Starttoaster/funrar.git`

 2. Change directory: `cd funrar/`

 3. Move funrar: `sudo cp funrar /usr/local/bin/funrar`

 4. Ensure funrar is executable: `sudo chmod +x /usr/local/bin/funrar`

 5. Run funrar: `funrar`


### User Preferences

By default, the directory this shell program searches through is your home directory. It will recursively search and find any split archives from your user's /home. 
Additionally, it places the files, by default, at the root of your user home directory. These options are customizable using variables designated at the top of the script. At any time you can change these variables with 
`sudo nano /usr/local/bin/funrar` (or replace with your favorite text editor) and change the "WORKDIR" and "DESTINATION" variables to your liking.

### Cleanup

At the end the script will list out all the directories containing split archives and ask you if you would like to delete them. Either select `y` or `n` to choose to delete, or keep them for now.
