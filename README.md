# bashscripts for ubuntu/vscode
> cd ~ && code .bashrc

#### customized terminal tabs

paste into .bashrc and save.  
```
set-title(){
  ORIG=$PS1
  TITLE="\e]2;$@\a"
  PS1=${ORIG}${TITLE}
}
```

type into terminal
```console
arlia@village:~$ set-title "mongod"
```

outputs "mongod" terminal tab name