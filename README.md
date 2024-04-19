<h1 align="Center"> Laboratorio de datos </h1>
<p align="center">
<image src="./_src/images/labo_de_datos.jpg" > 
</p>

## **Introduccion:**

En este repositorio encontramos todas las clases, tanto teoricas como practicas de la materia Laboratorio de datos dada el primer cuatrimestre del 2024. En la carpeta Notebooks podemos encontrar los notebooks con anotaciones que fui haciendo en clase y en la carpeta Practicas los resueltos de la guias de ejercicios junto con sus respectivos PDFs. 

***Disclaimer***: Los hice yo asique cualquier sugerencia para mejorar es bienvenida!

## Consejos:

Si estas en ***Visual Studio Code***, lo mejor seria correr un **virtual enviroment** para asi no descargar todos los modulos que se usan aca en tu maquina. Si no sabes tengo un repo de como crear tu maquina virtual al cual podes acceder [aca](https://github.com/Gabrielnm7/How-to-create-a-virtual-enviroment). Luego seleccionas el kernel en visual studio, abriendo cualquier jupyter notebook podes hacer click aca:

<image src="./_src/images/select_kernel.png">
 
 ## Nota errores en Windows:

Si llega a aparecer un error del tipo:
> No se puede cargar el archivo C:\Users\Usuario\Desktop\testing\venv\Scripts\activate.ps1 porque la ejecución de scripts está deshabilitada en este sistema...

Entonces hay que abrir PowerShell como administrador y ejecutar el siguiente comando:
```bash
Set-ExecutionPolicy -ExecutionPolicy Unrestricted -Scope CurrentUser
```
Una vez que hicimos todo lo anterior podemos volver a como estaba antes ejecuanto de vuelta en Powershell como administrador este codigo:
```bash
Set-ExecutionPolicy -ExecutionPolicy Restricted -Scope CurrentUser
```
Me paso tambien que si no se puede cargar el dataset de gapminder por que hay un error de tipo:
> ModuleNotFoundError: No module named 'pkg_resources'

Para solucionar esto simplemente ejecute dentro del entorno virtual el siguiente comando
```bash
    pip install --upgrade setuptools
```