#README
Esta carpeta contiene la información necesaria para analizar la diversidad y estructura genética del ciervo rojo europeo (*Cervus elaphus*)

Los datos se tomaron de:

Zachos FE, Frantz AC, Kuehn R, Bertouille S, Colyn M, Niedzialkowska M, Pérez-González J, Skog A, Šprem N, Flamand M (2016) Genetic structure and effective population sizes in European red deer (*Cervus elaphus*) at a continental scale: insights from microsatellite DNA. Journal of Heredity 107(4): 318-326. http://dx.doi.org/10.1093/jhered/esw011

Zachos FE, Frantz AC, Kuehn R, Bertouille S, Colyn M, Niedzialkowska M, Pérez-González J, Skog A, Šprem N, Flamand M (2016) Data from: Genetic structure and effective population sizes in European red deer (*Cervus elaphus*) at a continental scale: insights from microsatellite DNA. Dryad Digital Repository. http://dx.doi.org/10.5061/dryad.1v6p1

**El proyecto esta organizado en las carpetas:**

#*DATA 
Este directorio esta formado por dos carpetas:
####**Data_in:**
1. **ciervorojo.xlsx. **La base de datos de excel descargada del repositorio de Dryad con los genotipos de microsatélites de 668 individuos de ciervo rojo europeo.
2. **deer_strata.csv**. Es la misma base de datos pero ordenada y limpia
3. **reddeer.gen**. Base de datos ordenada de tal manera que el paquete adegenet pueda leeerlo (objeto genpop).

####**Data_out:**
Esta carpeta contiene los resultados obtenidos de los análisis realizados en forma de tablas de resumen.

#*BIN
Este directorio contiene los scripts utilizados para describir la diversidad y estructura genética de 33 poblaciones de ciervo rojo a partir de datos microsatelitales. Se recomienda que los scripts, que se describen a continuación, se corran en el siguiente orden:
####1.descargar base de datos.sh
Este script descarga la base de datos en formato excel que contiene los genotipos de 668  individuos de ciervo rojo europeo del repositorio de Dryad.

####2.Basic_genetics.R
Este script hace un análisis genético exploratorio. Calcula frecuencia alélica, heterocigosis y polimorfismo y evalua si las poblaciones se encuentran en equilibrio Hardy-Weinberg. Para correr este script se utiliza el archivo reddeer.gen ubicado en la carpeta Data_in

####3.Diferenciación_genetica.R
Este script calcula la diferenciación genética de datos microsatelitales de 33 poblaciones de ciervo rojo europeo. Nos da estadísticos de resumen de diferenciación global y por locus, realiza un análisis de varianza molecular (AMOVA) y un análisis discriminante de componentes principales (DAPC) y distancias de Nei. Para correr este script se utilizan los archivos reddeer.gen y deer_strata.csv  ubicados en la carpeta Data_in

#*FIGURES
En esta carpeta se encuentran los siguientes gráficos generados a partir de los scripts: 
1. Estimadores de diferenciación poblacional
2. Número óptimo de componentes principales
3. Análisis discriminante de componentes principales
4. neighbor joining

