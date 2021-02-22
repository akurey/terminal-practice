# Terminal con ZSH
## Objetivos
- Conocer herramientas que nos puedan ayudar a agilizar el desarrollo.
- Estandarizar el uso de alias para interactuar con git.

## Configuración del ambiente
Para el ejercio se va a utiliar una extensión de la terminal llamada `ZSH`, zsh extiende la terminal con un conjunto de funcionalidades que entre otras cosas pueden ser útilies para reducir el tiempo requerido para interactuar con git, esto mediante un conjunto de aliases.

ZSH brinda también la posibilidad de personalizar la terminal con el uso de temas (para que la terminal tenga colores), plugins de auto-complete, entre otros.

Para descargar ZSH se debe correr el comando `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`.

## Instalar plugins
ZSH tiene una basta colección de plugins que pueden ser de ayuda a la hora de desarrollar, en el siguiente [link](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins) pueden ver una lista completa.

Para efectos de esta práctica se van a utilizar los siguientes:
- git
- gitfast
- colorize
- command-not-found
  
Para agregar los plugins se debe hacer en el archivo de `~/.zshrc` de la siguiente manera
```bash
plugins=(
 git
 colorize
 gitfast
 command-not-found
)
```

## ZSH aliases con git
En el siguiente [link](https://github.com/ohmyzsh/ohmyzsh/wiki/Cheatsheet#git) se puede encontrar una lista de todos los aliases que ZSH provee para interactuar con git. La idea de esta práctica es que todo lo que se vaya a realizar con git, se haga mediante el uso de esos aliases, para así reducir el tiempo al escribir el comando completo.

### Instrucciones
Todas los pasos que a continuación se listan deben ser ejecutado mediante el uso de los aliases proveídos por ZSH.
- Clone este repositorio.
- Cree un branch con la incial de su nombre + el apellido, ejemplo: fsegovia
- Cree un file txt en el cuál va a escribir todos los comandos que ha utilizado hasta este punto.
- Haga commit del archivo
- Escriba nuevamente los comandos utilizados.
- Haga stash de los cambios realizados hasta este punto.
- Devuelvase al branch original.
- Cree un branch llamado `develop-[inicial-nombre]-[primer-apellido]` ejemplo `develop-fsegovia`.
- En este branch de develop cree un archivo con el mismo nombre que el branch anterior.
- Agregue todos los comandos (aliases) que utilizó hasta el momento.
- Haga commit y push del archivo
- Vuelva al primer branch creado.
- Haga pull de su branch de develop.
- Haga pop del stash.
- Si hay conflictos, resuélvalos.
- Agregue la lista final con todos los comandos utilizados.
- Responda las preguntas en la sección de *Retroalimentación* e incluya las respuestas en el archivo.
- Haga commit, push y merge a su branch de develop.

### Retroalimentación
1. Que tan fácil o difícil fue instalar ZSH?
2. Cree usted que puede agilizar el desarrollo este tipo de herramientas?
3. Continuará utilizando ZSH, sus plugins y aliases como parte de su día a día?
4. Algún comentario adicional?