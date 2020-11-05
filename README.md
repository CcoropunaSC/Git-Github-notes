<p align="center"><a href="https://git-scm.com" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/3/3f/Git_icon.svg" width="150"></a>
<a href="https://github.com" target="_blank"><img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="150"></a></p>

# Notes of **Git** and **Github**

## Contents
- [GIT](#git)
    - [See the **Git** Commands](#ee-the-git-commands)
    - [Global Settings](#global-settings)
    - [Area in **Git**](#areas-in-git)
    - [Start a Repository](#start-a-repository)
- [GITHUB](#github)

## Git

### See the Git Commands
<code>$git</code>

### Global Settings
* Configuración de información del usuario
<code>$ git config --help</code>      
* Configurar el nombre del usuario                   
<code>$ git config --global user.name "Username"</code>  
* Configurar el email del usuario
<code>$ git config --global user.email "email"</code>  
* Listar la configuración        
<code>$ git config --list</code>      
* Listar la configuración con el shorcuts                         
<code>$ git config -l</code>                               

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
*Activar el sistema de control de versiones **git**
<code>$ git init </code>                                           

<div align="right">
  <small><a href="#contents">🡡 to top</a></small>
</div>

### CICLO DE VIDA O ESTADOS DE LOS ARCHIVOS EN GIT
1. **TRACKED**
    * Archivos rastreados por **git**.
    * Sin cambios pendientes para guardar.
    * Ultima actualización ha sido guardada en el **repositorio**. Para ello se utiliza los siguientes comandos.
        <code>$ git add </code>
        <code>$ git commit</code>

2. **STAGED**
    * Son los archivos que se encuentran en **Staging**.
    * Archivos rastreados por **git**.
    * Hay registros de los archivos que han sido afectados por <code>$ git add </code> Este comando pasa los archivos del directorio al **staging**, pero, aún no se encuentra en el **repositorio**.
    * Falta ejecutar el comando <code>$ git commit</code> Este comando pasa del staging al repositorio.

3. **UNSTAGED**
    * Son rastreados por **git**, **"Traked pero Unstaged"**
    * Tiene actualizaciones pendientes para pasar al **staging** y despúes al **repositorio**
    * Se encuantran en el **directorio**
    * Aún no han sido affectados por <code>$git add </code>

4. **UNTRACKED**
    * No son rastreados por **git**
    * Los archivos han sido recientemente creados
    * Nunca han sido afectados por <code>$git add </code>

## Github


