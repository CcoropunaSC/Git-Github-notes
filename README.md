<p align="center"><a href="https://git-scm.com" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/3/3f/Git_icon.svg" width="150"></a>
<a href="https://github.com" target="_blank"><img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="150"></a></p>

# Notes of **Git** and **Github**

## Contents
- [Git](#git)
    - [See the **Git** Commands](#ee-the-git-commands)
    - [Global Settings](#global-settings)
    - [Area in **Git**](#areas-in-git)
    - [Start a Repository](#start-a-repository)
    - [Life Cycle or States of Files in **Git**](#Life-Cycle-or-States-of-Files-in-Git)
    - [Basic Commands](#Basic-Commands)
    - [Comands to View  the History](#Comands-to-View-the-History)
- [Github](#github)
- [Plus](#github)
    - [SSH Key Configuration](#SSH-Key-Configuration)

## Git

### See the Git Commands
<code>$ git </code>

### Global Settings
* Configuración de información del usuario <code>$ git config --help</code>      
* Configurar el nombre del usuario <code>$ git config --global user.name "Username"</code>  
* Configurar el email del usuario <code>$ git config --global user.email "email"</code>  
* Listar la configuración <code>$ git config --list</code>      
* Listar la configuración con el shorcuts <code>$ git config -l</code>                               

<div align="right">
  <small><a href="#contents">🡡 to top</a></small>
</div>

### Areas in **Git**
1. Área de trabajo - Directorio <code>$ git init</code>
2. Área de preperación - Staging
3. Repositorio (/.git/)

<div align="right">
  <small><a href="#contents">🡡 to top</a></small>
</div>

### Start a Repository
*Activar el sistema de control de versiones **git** <code>$ git init </code>                                           

<div align="right">
  <small><a href="#contents">🡡 to top</a></small>
</div>

### Life Cycle or States of Files in Git
1. **Tracked**
    * Archivos rastreados por **git**.
    * Sin cambios pendientes para guardar.
    * Ultima actualización ha sido guardada en el **repositorio**. Para ello se utiliza los siguientes comandos.
        <code>$ git add </code>
        <code>$ git commit</code>

2. **staged**
    * Son los archivos que se encuentran en **Staging**.
    * Archivos rastreados por **git**.
    * Hay registros de los archivos que han sido afectados por <code>$ git add </code> Este comando pasa los archivos del directorio al **staging**, pero, aún no se encuentra en el **repositorio**.
    * Falta ejecutar el comando <code>$ git commit</code> Este comando pasa del staging al repositorio.

3. **Unstaged**
    * Son rastreados por **git**, **"Traked pero Unstaged"**
    * Tiene actualizaciones pendientes para pasar al **staging** y despúes al **repositorio**
    * Se encuantran en el **directorio**
    * Aún no han sido affectados por <code>$git add </code>

4. **Untracked**
    * No son rastreados por **git**
    * Los archivos han sido recientemente creados
    * Nunca han sido afectados por <code>$git add </code>

<div align="right">
  <small><a href="#contents">🡡 to top</a></small>
</div>

### Basic Commands
* Cambiar el estado del archivo blog.txt de **UNSTAGED** a **STAGED** o de **UNTRACKED** a **STAGED** <code>$ git add blog.txt </code>
* Puede utilizar este comando para cambiar de estado a todos los archivos presentes en la carpeta actual <code>$ git add . </code>             
* Cambiar el estado de todos los archivos de **STAGED** a **TRACKED** <code>$ git commit </code>   
_OJO:_ al ejecutar el comando <code>$ git commit </code> se va abrir el editor de consola **VIM**
    * Una vez abierta se debe presionar <code>ESC+I</code> para insertar mensaje del commit
    * Para cerrar el editor se debe presionar <code>ESC+SHIFT+ZZ</code>
    * Más sobre **VIM** https://www.vim.org/docs.php

* Hacer el commit sin la necesidad de abrir el editor de consoala <code>$ git commit -m "message"  </code>
* Cambiar estado de UNSTAGED a TRACKED. Esto se puede siempre y cuando los archivos este rastreados, caso contrario es necesario hacer el git add <code>$ git commit -am "message" </code>  

### Comands to View  the History
* Muestra el historial de todos loa commits <code>$ git log </code>                               
* Muestra el historial de los commit en una sola linea <code>$ git log --oneline </code>                     
* Muestra solo los últimos 5 commits <code>$ git log --oneline -n 5  </code>               
* Muestra los commit con el nombre del usuario <code>$ git log --pretty=format:"%h fue %an" </code>
* Muestra todos los commit, sin importar que estén por encima del HEAD <code>$ git log --oneline --all  </code>              
* Muestra los commits decorados y con gráfica de las ramas <code>$ git log --oneline --all --decorate --graph </code>   
## Github
## Plus
#### SSH Key Configuration
* Generar la llav ssh <code>$ ssh-keygen -t rsa -b 4096 -C "email@gmail.com" </code>   
* Encerder el servidor de las llaves de ssh <code>$ eval $(ssh-agent -s)  </code>                           
* Agregar la llave <code>$ ssh-add ~/.ssh/id_rsa </code>                            


