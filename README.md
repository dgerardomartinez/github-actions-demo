## Pipelines de automatización - GitHub Actions
    
    Esta autommatización la realizaremos con ayuda de GitHub Actions, por medio de un SFTP, lo que hará realmente es sincronizar el index.php de la página principal de nuestro web server en este caso tiene instalada la aplicación de WordPress.

---------------------------------------------------------------------------------------------------------------------------------------------

# 1. Clonar el repositorio en nuestra computadora
```
git clone https://github.com/dgerardomartinez/github-actions-final.git
```

2. Crear carpeta .github y dentro de ella workflows.

3. Crear archivo.yml en la carpeta de workflows.

4. Crear una carpeta con el index.php que se modificará, estoy nos servirá para después trasladar los cambios a la página de inicio de nuestro web server.

5. Generar llave ssh privada y pública con este comando
```
ssh-keygen
```
6. Agregar al servidor web en Digital Ocean el valor de la llave pública, esto lo podemos realizar desde el software putty.

7.	Agregar en el repositorio de github la llave privada generada, esto lo realizamos en las configuraciones del repositorio.

8. COMANDOS IMPORTANTES PARA ACTUALIZAR GITHUB
    a.	Git status
    b.	Git add .
    c.	Git commit “add github actions workflow”  
    d.	Git push 

9. Comprobamos si se realizo la automatización en nuestro deployment from GitHub to server via SFTP.

