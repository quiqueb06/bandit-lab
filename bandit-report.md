## Bandit Level 1
**Objetivo:** Encontrar la contraseña del siguiente nivel.

Comandos utilizados:
```bash
ls
cat ./-

Contraseña obtenida:
NH2SXQwcBdpmTE9S77R9NcyR63Yn69Z7

## Bandit Level 2
**Objetivo:** Leer el archivo con espacios en el nombre llamado `spaces in this filename`.

Comandos utilizados:
pwd
cat ./*

Contraseña obtenida:
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

## Bandit Level 3

**Objetivo**: Encontrar la contraseña del siguiente nivel oculta en un archivo dentro de la carpeta inhere.

Comandos utilizados:
cd inhere
ls
ls -a
cat ...Hiding-From-You

Contraseña obtenida:
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

## Bandit Level 4

Objetivo: Identificar y leer el único archivo que contiene texto legible (ASCII) dentro de un directorio con múltiples archivos de datos binarios.

Comandos:
ls
cd inhere/
file ./*
cat ./-file07

Contraseña obtenida:
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

## Bandit Level 5

Objetivo: Localizar un archivo de 1033 bytes de tamaño que sea legible por humanos dentro de las subcarpetas del directorio actual.

Comandos:
ls
cd inhere/
find -size 1033
cd maybeinhere07/
cat .file2

Contraseña obtenida:
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

## Bandit Level 6

Objetivo: Localizar un archivo en todo el servidor basado en su propietario, grupo y tamaño exacto.

Comandos:
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password


Contraseña obtenida:
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

## Bandit Level 7

Objetivo:
Extraer una contraseña específica de un archivo de texto de gran tamaño filtrando por una palabra clave.

Comandos:
grep "millionth" data.txt


Contraseña obtenida:
dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

## Bandit Level 8

Objetivo:
Encontrar la única línea de texto que no se repite dentro de un archivo con múltiples entradas duplicadas.

Comandos:
sort data.txt | uniq -u


Contraseña obtenida:
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM

## Bandit Level 9

Objetivo:
Extraer una cadena de texto legible de un archivo binario filtrando por un patrón de caracteres específicos.

Comandos:
strings data.txt 


Contraseña obtenida:
FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey

## Bandit Level 10

Objetivo:
Decodificar un archivo que contiene una cadena de texto representada en formato Base64 para obtener la contraseña en texto plano. 

Comandos:
base64 -d data.txt


Contraseña obtenida:
dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr

...
