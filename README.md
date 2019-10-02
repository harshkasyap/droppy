# Setting Droppy Using Docker

* Help Sought from [here](https://github.com/harshkasyap/droppy)

* Pre-Requisites
    * Docker Installed and nothing else.

* Clone this Repository and Go to this Folder FileRun
    * Windows
        * Just Run this command
            * docker-compose up -d
        * In case You want to change the Drive Location where you want to keep the files,
            * See the last volume section of yml files, change them (left hand side ones). (No need to create the folders, just change the drive.)
    
    * Linux-Based Machine
        * See the last volume section of yml files, change them with something like below, unless you want to keep them at some custom location.
            * /droppy/config::/config
            * /droppy/files:/files

* Copy config.json to the config directory, here public has been updated as true for no authentication.

# Issues

* Not Listening on all interfaces, only on localhost.