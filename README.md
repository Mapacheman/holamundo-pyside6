# holamundo-pyside6
Aplicación de ejemplo con PySide6 para mostrar 'Hola Mundo'
## Pasos de Instalación y Ejecución

### 1. Instalación de Python 3

#### Windows
Para instalar Python en Windows:

1. Dirígete a [python.org](https://www.python.org/downloads/).
2. Descarga el instalador de Python 3 para Windows.
3. Ejecuta el instalador y asegúrate de seleccionar la opción **"Add Python to PATH"**.
4. Finaliza la instalación.

#### Linux
En una distribución basada en Debian (como Ubuntu), puedes instalar Python con:

```bash
sudo apt update
sudo apt install python3

### 2. Instalación y Activación de pip

#### Windows

pip generalmente se instala junto con Python. Para verificar que pip está disponible, ejecuta:
python -m ensurepip --upgrade

## Si necesitas actualizar pip, usa el siguiente comando:
python -m pip install --upgrade pip

## pip también se puede instalar fácilmente con:
sudo apt install python3-pip

##Para verificar la instalación de pip, ejecuta:
pip3 --version

#### 3. Creación y Activación de Entorno Virtual

#### Windows

Para crear un entorno virtual, abre la terminal en la carpeta de tu proyecto y ejecuta:
python -m venv venv
## Para activar el entorno virtual, usa el siguiente comando:
.\venv\Scripts\activate

####Linux
Para crear un entorno virtual en Linux, usa:
python3 -m venv venv

## Y para activarlo:
source venv/bin/activate

### 4. Instalación de Dependencias

Una vez que el entorno virtual esté activado, instala las dependencias necesarias para el proyecto. En este caso, la principal dependencia es **PySide6**.

## Ejecuta el siguiente comando para instalar PySide6:
pip install pyside6

### 5. Ejecución de la Aplicación

Ahora que tienes todo instalado, puedes crear un archivo Python con el siguiente código para mostrar el mensaje "Hola Mundo" utilizando PySide6:

```python
import sys
from PySide6.QtWidgets import QApplication, QLabel

app = QApplication(sys.argv)
label = QLabel("¡Hola Mundo!")
label.show()
app.exec()

## Guarda este código en un archivo llamado app.py (o el nombre que prefieras).

## Para ejecutar la aplicación, usa el siguiente comando en la terminal (asegúrate de estar en el entorno virtual):
python app.py
