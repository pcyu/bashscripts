# bashscripts
> cd ~ && code .bashrc

Using Visual Studio Code and Ubuntu, paste these scripts into .bashrc file.

#### Customized Terminal Tab Names

```set-title(){
  ORIG=$PS1
  TITLE="\e]2;$@\a"
  PS1=${ORIG}${TITLE}
}
```

```console
arlia@village:~$ set-title "mongod"
```

outputs "mongod" terminal tab name