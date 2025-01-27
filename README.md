## PostgreSQL usando PostGIS
#### Introducción a postgreSQL usando la extensión postGIS complementando con QGIS

#### Conexión
Después de haber creado el workspace con distintas carpetas (repositorios), iniciamos este archivo con ```git init``` para luego agregarlo al repositorio usando ```git remote add origin -url-```. Usando ```git remote -v``` se puede verificar el repositorio remoto al que está vinculada la carpeta.

#### Documentación
* Para cargar las bases de datos desde QGIS, es necesario crear una nueva conexión desde el panel navegador y completar los parámetros (usuario, clave y nombre de la base de datos). Luego, se pueden agregar los archivos desde el respectivo directorio. Cuando refrescamos en pgAdmin podremos visualizarlo.

* Ejemplos prácticos
    ```ruby
    SELECT *
    FROM -columna-
    ORDER BY ST_Area(geom) # ordena en función del tamaño (geom)
    DESC; # en orden descendente
    ```

    ```ruby
    SELECT sum(columna) # pido la suma del campo
    FROM barrios # tabla barrios
    ```