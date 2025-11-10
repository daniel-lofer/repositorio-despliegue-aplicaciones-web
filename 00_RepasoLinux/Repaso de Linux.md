# Repaso de Linux

[TOC]

## Capítulo 2 - Ficheros y directorios

**Tabla de los directorios más importantes de sistema Linux**

![2025-09-25 17_04_00-1_2_3_merged (1).pdf - Adobe Acrobat Reader (64-bit)](./Repaso%20de%20Linux.assets/2025-09-25%2017_04_00-1_2_3_merged%20(1).pdf%20-%20Adobe%20Acrobat%20Reader%20(64-bit).png)

### 2.3 Visualización, creación y cambio de directorios (pwd, ls, cd, mkdir)

`pwd` 

Muestra en qué directorio se encuentra en el momento de escritura del comando

```bash
$ pwd
```

![2025-09-29 15_57_09-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2015_57_09-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

`ls`

Este comando sirve para mostrar el contenido del directorio en el que nos encontremos

```bash
$ ls
```

![2025-09-29 16_01_18-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_01_18-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

Este posee diferentes variaciones

`ls -a`

Muestra todos los archivos, incluyendo ocultos

```bash
$ ls -a
```

![2025-09-29 16_04_40-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_04_40-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

`ls -l`

Muestra un listado de los archivos de manera detallada

```bash
$ ls -l
```

![2025-09-29 16_04_51-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_04_51-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

`ls -h`

Muestra un listado de los archivos, pero con el tamaño de los ficheros incluido

```bash
$ ls -h
```

![2025-09-29 16_05_05-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_05_05-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

`man`

En el caso que queramos saber para qué se usa un comando, si colocamos `man` delante, se nos dará una guía con información detallada sobre el comando, para salir del manuar, si pulsamos la letra q, saldremos de este.

```bash
$ man [comando]
```

![2025-09-29 16_09_28-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_09_28-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

![2025-09-29 16_09_55-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_09_55-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

`cd`

Este sirve para cambiar de directorio. Si no se escribe nada, irá al directorio principal, en el caso de que se indique a continuación una ruta, se cambia al directorio que se indica.

```bash
$ cd
```

![2025-09-29 16_23_56-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_23_56-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

En el caso de que queramos acceder a un directorio que se encuentre dentro del que ya estamos, deberemos indicar a continuación del comando a cuál queremos acceder

```bash
$ cd [Ubicación]
```

![2025-09-29 16_26_45-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_26_45-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

En el caso de que deseemos utilizar una ruta absoluta, deberemos indicarlo iniciando con una / al inicio



```bash
$ cd /[Ubicación]
```

![2025-09-29 16_29_11-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_29_11-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

Si deseamos retroceder atrás, deberemos indicar tras el comando dos puntos:



```bash
$ cd ..
```

![2025-09-29 16_30_57-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_30_57-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

`mkdir`

Si deseamos crear un directorio, deberemos utilizar este comando.

```bash
$ mkdir nombreCarpeta
```

![2025-09-29 16_38_26-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_38_26-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

Si queremos utilizar más de uno, deberemos introducir mediante espacios los directorios que se deseen crear.

```bash
$ mkdir nombreCarpeta1 nombreCarpeta2 nombreCarpeta3
```

![2025-09-29 16_42_05-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_42_05-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

### 2.4 Visualización de ficheros

`cat`

Si deseamos mostrar por pantalla el contenido de un fichero, este te lo muestra.

```bash
$ cat [ruta del documento]
```

![2025-09-29 16_52_22-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_52_22-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

`more`

Sirve para lo mismo que `cat`, solo que este muestra hasta que se llena la pantalla y, si se quiere ver más, debe presionarse espacio para pasar a la siguiente ventana.

```bash
$ more [ruta del documento]
```

![2025-09-29 16_55_26-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_55_26-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

`less`

Se utiliza igual que los demás, pero se pude ir avanzando usando los cursores. Si deseamos salir del documento, se debe presionar el botón "q".

```bash
$ less [ruta del documento]
```

![2025-09-29 16_58_37-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2016_58_37-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

`head`

Sirve para mostrar las primeras líneas del contenido del fichero.

```bash
$head [ruta del documento]
```

![2025-09-29 17_05_36-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2017_05_36-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

`tail`

Sirve para mostrar las últimas líneas del contenido del fichero.

```bash
$ tail [ruta del documento]
```

![2025-09-29 17_05_48-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2017_05_48-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

Tanto en `head` como en `tail`, se muestran 10 líneas, pero si se indica con `-n`, en este se indica las líneas que deseamos que se muestren.

```bash
$head -n[numero de líneas] [ruta del documento]
```

![2025-09-29 17_10_00-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2017_10_00-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

```bash
$tail -n[numero de líneas] [ruta del documento]
```

![2025-09-29 17_10_13-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2017_10_13-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox-1759158647941-25.png)

### 2.5 Edición de ficheros (touch, vi, ee, mcedit)

`touch`

El comando permite crear un fichero vacío en el documento

```bash
$touch [nombre del archivo].[extensión]
```

![2025-09-29 17_16_28-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2017_16_28-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

~~`ee`~~ 

Deprecado, se recomienda la utilización de editores como gedit, joe o nano.

`vi`

Se utiliza para inicializar el editor de Linux "vi".

```bash
$vi [nombre del documento]
```

![2025-09-29 17_21_14-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2017_21_14-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)



## Ejercicios del capítulo 2

3. Muestra del contenido del directorio actual

```bash
$ ls
```

![2025-09-29 17_23_30-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2017_23_30-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

4. Muestra el contenido del directorio que está justo a un nivel superior

   ```BASH
   $ ls Escritorio
   ```

   ![2025-09-29 17_24_46-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-09-29%2017_24_46-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)
   
4. ¿En qué día de la semana naciste?, utiliza la instrucción cal para averiguarlo.

   ```bash
   $ cal 07 1999
   ```

   ![2025-10-02 16_15_42-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-10-02%2016_15_42-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)
   
   6. Muestra los archivos del directorio /bin
   
      ```bash
      $ ls /bin
      ```
   
   ![2025-10-02 16_19_05-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-10-02%2016_19_05-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)
   
   7. Suponiendo que te encuentras en tu directorio personal (/home/nombre), muestra un listado del contenido de /usr/bin con una sola línea de comando
   
      ```bash
      $ ls /usr/bin
      ```
   
      ![2025-10-02 16_32_49-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-10-02%2016_32_49-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)
   
      8. Muestra todos los archivos que hay en /etc y todos los que hay dentro de cada subdirectorio, de forma recursiva (con un solo comando)
   
         ```bash
         $ls –R /etc
         ```
   
         ![2025-10-02 16_36_11-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-10-02%2016_36_11-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)
   
         9. Muestra todos los archivos del directorio /usr/X11R6/bin ordenados por tamaño (de mayor a menor). Sólo debe aparecer  el nombre de cada fichero, sin ninguna otra información adicional.
   
            ```bash
            $ls -s /usr/X11R6/bin
            ```

10. Muestra todos los archivos del directorio /etc ordenados por tamaño (de mayor a menor) junto con el resto de características, es decir, permisos, tamaño, fechas de la última modificación, etc. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc.

```bash
$ ls -Slh /etc
```

![2025-10-02 16_42_00-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-10-02%2016_42_00-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

11. Muestra todos los archivos del directorio /bin ordenados por tamaño (de menor a mayor). Sólo debe aparecer el tamaño y el nombre de cada fichero, sin ninguna otra información adicional. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc.

    ```bash
    $ ls -Sshr /bin
    ```

    ![2025-10-02 16_42_00-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-10-02%2016_42_00-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox-1759416538384-6.png)

    12. Muestra el contenido del directorio raíz utilizando como argumento de ls una ruta absoluta.

        ```bash
        $ ls /
        ```

        ![2025-10-02 16_53_46-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-10-02%2016_53_46-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

    13. Muestra el contenido del directorio raíz utilizando como argumento de ls una ruta relativa. Suponemos que el directorio actual es /home/danny25/documentos.

        ```bash
        $ ls /home/danny25/documentos
        ```

        ![2025-10-02 16_56_15-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-10-02%2016_56_15-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

    14. Crea el directorio gastos dentro del directorio personal

        ```bash
        $ mkdir /home/danny25/gastos
        ```

        ![2025-10-02 16_58_52-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-10-02%2016_58_52-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

    15. ¿Qué sucede si se intenta crear un directorio dentro de /etc?

        Se deniega porque no hay permisos

        ![2025-10-02 17_00_14-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-10-02%2017_00_14-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

    16.  Muestra el contenido del fichero /etc/fstab

        ```bash
        $ cat /etc/fstab
        ```

        ![2025-10-02 17_08_15-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-10-02%2017_08_15-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

    17.  Muestra las 10 primeras líneas del fichero /etc/bash.bashrc

        ```bash
        $ head /etc/bash.bashrc
        ```

        ![2025-10-02 17_10_57-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-10-02%2017_10_57-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

    18. -

    19.  Crea un fichero vacío dentro del directorio musica, con nombre estilos_favoritos.txt

        ```bash
        $ touch Música/estilos_favoritos.txt
        ```

        ![2025-10-02 17_14_39-cliente24_Danny [Corriendo] - Oracle VirtualBox](./Repaso%20de%20Linux.assets/2025-10-02%2017_14_39-cliente24_Danny%20%5BCorriendo%5D%20-%20Oracle%20VirtualBox.png)

        

    20. Utiliza tu editor preferido para abrir el fichero estilos_favoritos.txt e introduce los estilos de música que más te gusten. Guarda los cambios y sal.

        ```bash
        $ nano Música/estilos_favoritos.txt
        ```

        

    21. Muestra todo el contenido de estilos_favoritos.txt

        ```bash
        $ cat Música/estilos_favoritos.txt
        ```

        

        

    22. Muestra las 3 primeras líneas de estilos_favoritos.txt

        ```bash
        $ head -n3 Música/estilos_favoritos.txt
        ```

        

        

    23. Muestra la última línea de estilos_favoritos.txt

        ```bash
        $ tail -1 Música/estilos_favoritos.txt
        ```

        

        

    24. Muestra todo el contenido del fichero estilos_favoritos.txt excepto la primera línea. Se supone que no sabemos de antemano el número de líneas del fichero.

        ```bash
        $ tail -n+2 Música/estilos_favoritos.txt
        ```

        ## Capítulo 3: Ficheros y directorios

        ### 3.1. Caracteres comodín

        Se pueden usar corchetes como símbolo comodín para no tener que escribir todos los ficheros del 1 al 6.

        ```bash
        $ cat docu[1-6]
        ```

        En el caso de que queramos aquellos que comiencen por docu

        ```bash
        $ cat docu*
        ```

        En el caso de que queramos que comience y termine por una letra, se puede poner el asterisco en medio

        ```bash
        $ ls /usr/bin/a*s
        ```

        En el caso de que queramos que solo sustituya un carácter, utilizaremos el símbolo ?

        ```bash
        $ ls /usr/bin/g?o*
        ```
    
        Este sirve para todos aquellos que comience por la letra "g" y que siga cualquier carácter, seguido de una "o" y el resto del texto.
    
        

## 3.2 Copia y borrado de ficheros

.cp sirve para copiar fichero, puede ser uno o muchos
