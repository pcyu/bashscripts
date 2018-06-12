# bashscripts
Using Visual Studio Code and Ubuntu.
> cd ~ && code .bashrc

paste these scripts into that .bashrc file.

#### Customized Terminal Tab Names

set-title(){
  ORIG=$PS1
  TITLE="\e]2;$@\a"
  PS1=${ORIG}${TITLE}
}

```console
foo@bar:~$ set-title "mongod"
```

Outputs Terminal Tab Name "mongod"