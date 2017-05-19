**AVANCE 3**
En este momento el proyecto se ve con más forma, probablemente lo más difíe limpiar la base de datos y acomodarla de la manera en la que la necesitaba.
Leí el manual de adegenet y eso me dio mucha luz a cerca de cuales eran y como hacer los análisis, también la página de http://popgen.nescent.org/ fue de mucha ayuda.
Hasta el momento he corrido los siguientes scripts:

**1.descargar base de datos.sh**. 
Este script descarga la base de datos en formato excel que contiene los genotipos de 668  individuos de ciervo rojo europeo del repositorio de Dryad.

**2.Basic_genetics.R**
Este script hace un análisis genético exploratorio. Calcula frecuencia alélica, heterocigosis y polimorfismo y evalua si las poblaciones se encuentran en equilibrio Hardy-Weinberg. Para correr este script se utiliza el archivo reddeer.gen ubicado en la carpeta Data_in

**3.Diferenciación_genetica.R**
Este script calcula la diferenciación genética de datos microsatelitales de 33 poblaciones de ciervo rojo europeo. Nos da estadísticos de resumen de diferenciación global y por locus, realiza un análisis de varianza molecular (AMOVA) y un análisis discriminante de componentes principales (DAPC) y distancias de Nei. Para correr este script se utilizan los archivos reddeer.gen y deer_strata.csv  ubicados en la carpeta Data_in
