# Ratón Virtual Controlado por Gestos &nbsp;[![](https://img.shields.io/badge/python-3.8.5-blue.svg)](https://www.python.org/downloads/) [![platform](https://img.shields.io/badge/platform-windows-green.svg)](https://github.com/xenon-19/Gesture_Controller)

El Ratón Virtual Controlado por Gestos simplifica la interacción humano-computadora utilizando gestos de mano y comandos de voz. El ordenador casi no requiere contacto directo. Todas las operaciones de entrada/salida pueden controlarse virtualmente mediante gestos de mano estáticos y dinámicos junto con un asistente de voz. Este proyecto utiliza algoritmos de aprendizaje automático y visión por computadora de última generación para reconocer gestos de mano y comandos de voz, funcionando sin necesidad de hardware adicional. Se basa en modelos como CNN implementados por [MediaPipe](https://github.com/google/mediapipe) sobre pybind11. Consta de dos módulos: uno que utiliza la detección de manos de MediaPipe y otro que emplea guantes de un color uniforme. Actualmente, funciona en la plataforma Windows.

Nota: Usa la versión de Python: 3.8.5.

---

## Características

### Reconocimiento de gestos:

#### Gestos incluidos:
- **Neutral**: Detiene/pausa la ejecución del gesto actual.  
- **Mover el cursor**: Desplaza el cursor al punto medio entre las yemas de los dedos índice y medio.
- **Clic izquierdo**: Realiza un clic izquierdo simple.
- **Clic derecho**: Realiza un clic derecho simple.
- **Doble clic**: Realiza un doble clic.
- **Desplazamiento**: Desplazamientos horizontales y verticales proporcionales a los movimientos del gesto de pellizco.
- **Arrastrar y soltar**: Permite mover/transferir archivos de un directorio a otro.
- **Selección múltiple**: Permite seleccionar varios elementos.
- **Control de volumen**: Ajusta el volumen mediante gestos dinámicos.
- **Control de brillo**: Ajusta el brillo mediante gestos dinámicos.

---

## Primeros pasos

### Requisitos previos:
- **Python**: Versiones 3.6 - 3.8.5.
- **Distribución Anaconda**: [Descargar aquí](https://www.anaconda.com/products/individual).

### Procedimiento:

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/Gocardi/ACproyect.git
   ```
2. Crear un entorno virtual:
   ```bash
   conda create --name gest python=3.8.5
   ```
3. Activar el entorno:
   ```bash
   conda activate gest
   ```
4. Instalar las dependencias:
   ```bash
   pip install -r requirements.txt
   pip install PyAudio
   pip install pywin32
   ```
5. Navegar al directorio `src`:
   ```bash
   cd Ruta\del\repositorio\Gesture-Controlled-Virtual-Mouse\src
   ```
6. Ejecutar el asistente de voz:
   ```bash
   python Proton.py
   ```
   Para solo ejecutar el reconocimiento de gestos, descomenta las últimas dos líneas del archivo `Gesture_Controller.py` y ejecuta:
   ```bash
   python Gesture_Controller.py
   ```

---