> [!WARNING]  
> Este proyecto aún se encuentra en desarrollo.  


# Descripción

Este es un script orientado a mejorar la lectura e interpretación de los datos de un fichero `.eml` -correspondientes a
las cabeceras de correos electrónicos-, con el fin de facilitar tareas de SOC como:

- Análisis de correos sospechosos.
- Extracción de datos de phishing.
- Detección de spoofing en correos.

## Características

- Detectar si un fichero EML está bien construido.
- Extraer los datos más relevantes de un fichero EML.
- Exportar los datos del fichero EML en formato JSON.


# Instalación

1. Instalar [Python 3.9](https://www.python.org/downloads) (mínimo).
2. Clonar el repositorio.


# Utilización

## Ejecución

Este script se puede ejecutar de 2 formas:

- Comando de terminal.
- Módulo de Python.

### Comando de terminal

Será necesario otorgar permisos de ejecución al script:

```shell
sudo chmod +x script.py
```

> [!NOTE]  
> Como el script contiene el shebang `#!/usr/bin/env python3`, el sistema lo ejecutará con el intérprete de Python.

Tras eso, se puede ejecutar el script como:

```shell
./script.py <args>
```

### Módulo de Python

Solo es necesario usar el intérprete de Python de la forma habitual:

```shelll
python3 script.py <args>
```

## Argumentos

El script funciona con 1 solo argumento obligatorio: **un fichero EML**.

Opcionalmente, se puede usar un flag para exportar los resultados como JSON.

> [!NOTE]  
> Si no se proporciona el fichero, se mostrará la ayuda (equivalente a `./script.py -h`).

### `<fichero EML>`

El script recibe un fichero EML y comprueba que este sea válido para poder operar.

Si todo es correcto, se procede a analizar las cabeceras del correo.

### `-e` / `--export`

Opcionalmente, el script puede exportar los datos del fichero EML en formato JSON.

Esto puede ser útil para automatizar procesos o compartir con otros usuarios.

## Ejemplo

> [!WARNING]  
> Esta sección aún está en proceso.
