# bashscripts
Using Visual Studio Code and Ubuntu.
> cd ~ && code .bashrc

paste these scripts into that .bashrc file.

### set-title "mongod"
#### will set your terminal tab title as "mongod"
> set-title(){
  ORIG=$PS1
  TITLE="\e]2;$@\a"
  PS1=${ORIG}${TITLE}
 }