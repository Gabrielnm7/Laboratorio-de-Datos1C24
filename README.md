<h1 align="Center"> Laboratorio de datos </h1>
<p align="center">
<image src="./_src/images/labo_de_datos.jpg" > 
</p>

## **Introduccion:**

En este repositorio encontramos todas las clases, tanto teoricas como practicas de la materia Laboratorio de datos dada el primer cuatrimestre del 2024. En la carpeta Notebooks podemos encontrar los notebooks con anotaciones que fui haciendo en clase y en la carpeta Practicas los resueltos de la guias de ejercicios junto con sus respectivos PDFs. 
### **Organizacion de carpetas**
| Clase  | Notebook-Practica | Ejercicios | Resuelto |  
| -----  | ----------------- | ---------- | -------- |
| [_Clase 1: Programa e informacion general_](./Clases/clase1-slides.pdf) | [Notebook 1: Numpy, pandas](./Notebooks/clase1-laboDatos-numpy.ipynb) | [Guia practica 1](./Practicas/PDFs/practica1-ldd-1c2024.pdf) | None |  
| [_Clase 2: Estadistica Descriptiva_](./Clases/clase02-estadisticaDescriptiva-slides.pdf) | [Notebook 2: Pandas](./Notebooks/clase2-ldd-estadisticaDescriptiva.ipynb) | [Guia Practica 2](./Practicas/PDFs/practica2-ldd-1c2024.pdf) | None |
| [_Clase 3: Git_](./Clases/clase03-git.pdf) | None | Simulacion de Clonacion y fork con compañeros en clase | None |
| [_Clase 4 y 5: Visualizacion_](./Clases/clase04-visualizacion-slides.pdf) | [Clase 4 y 5](./Notebooks/clase4-ldd-visualizacion.ipynb) | [Guia Practica 3](./Practicas/PDFs/practica3-ldd-1c2024.pdf) | [Resuelto Guia 3](./Practicas/practica3.ipynb) |
| [_Clase 6: Regresión Lineal_](./Clases/clase06-regresionLineal-slides.pdf) | [Notebook 6](./Notebooks/clase6-ldd-regresionlineal.ipynb) | [Guia practica 4](./Practicas/practica4.ipynb) | [Resuelto Guia 4](./Practicas/practica4.ipynb) | 
| [_Clase 7: Cuadrados Minimos_](./Clases/clase07-cuadradosMinimos-slides.pdf) | [Notebook 7](./Notebooks/clase7-ldd-cuadradosminimos.ipynb) | Igual que arriba | Igual que arriba |
| [_Clase 8: Modelo Lineal Multivariado_](./Clases/clase08%20-%20Modelo%20Lineal%20Multivariado.pdf) | None | [Guia Practica 5](./Practicas/PDFs/practica5-ldd-1c2024.pdf) | [Resuelto Guia 5](./Practicas/practica5.ipynb) |
| [_Clase 9: Entrenamiento_](./Clases/clase09-entrenamiento-slides.pdf) | [Notebook clase 9](./Notebooks/Clase9-Multivariado-Clase.ipynb) | Igual que arriba | Igual que arriba |


***Disclaimer***: Los resueltos son hechos por mi asique cualquier sugerencia/correción para mejorar es bienvenida!

## Consejos:

Si estas en ***Visual Studio Code***, lo mejor seria correr un **virtual enviroment** para asi no descargar todos los modulos que se usan aca en tu maquina. Si no sabes tengo un repo de como crear tu maquina virtual al cual podes acceder [aca](https://github.com/Gabrielnm7/How-to-create-a-virtual-enviroment). Luego seleccionas el kernel en visual studio, abriendo cualquier jupyter notebook podes hacer click aca:

<image src="./_src/images/select_kernel.png">
 
 ## Nota errores en Windows:

Si llega a aparecer un error similar al siguiente:
> No se puede cargar el archivo C:\Users\Usuario\venv\Scripts\activate.ps1 porque la ejecución de scripts está deshabilitada en este sistema...

Entonces hay que abrir PowerShell como administrador y ejecutar el siguiente comando:
```bash
Set-ExecutionPolicy -ExecutionPolicy Unrestricted -Scope CurrentUser
```
Una vez que hicimos todo lo anterior podemos volver a como estaba antes ejecuanto de vuelta en Powershell como administrador este codigo:
```bash
Set-ExecutionPolicy -ExecutionPolicy Restricted -Scope CurrentUser
```
Me pasó también que no se puede cargar el dataset de gapminder por que sale este error:
> ModuleNotFoundError: No module named 'pkg_resources'

Para solucionarlo simplemente ejecuté dentro del entorno virtual el siguiente comando
```bash
    pip install --upgrade setuptools
```
Con esto ya puedo utilizar el dataset. 