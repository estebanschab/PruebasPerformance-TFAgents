# PruebasPerformance-TFAgents
Implementación de pruebas de performance sobre un tutorial de Agente de Aprendizaje por refuerzo con TensorFlow Agents, GPU vs CPU.


# Pasos a seguir para instalar y configurar el software y las librerías necesarias en un sistema Windows x64

1- Instalar de Microsoft Visual Studio

2- Instalar Anaconda (https://www.anaconda.com/products/individual)

2- Instalar o actualizar los Controladores de GPU de NVIDIA® (Comprobar en la documentación de TensorFlow la versión requerida para asegurar la compatibilidad)

3- Instalar de NVIDIA CUDA ToolKit (Comprobar en la documentación de TensorFlow la versión requerida para asegurar la compatibilidad)

4- Instalación de NVIDIA CuDNN

5- Configuración de variables de entorno en el sistema para CUDA

6- En Anaconda Prompt

   -Crear un nuevo entorno en Anaconda:
   
   conda create -n TensorFlow_GPU_Test python=3.7
   
   -Activar el entorno creado:
   
   conda activate TensorFlow_GPU_Test
   
   -Instalar TensorFlow y las dependencias necesarias:
   
   pip install tensorflow 
   
   -En Anaconda Prompt Instalar Jupyter Notebook, Seaborn y Matplotlib:
   
   pip install jupyter ipykernel seaborn matplotlib
   
   -Agregar el entorno Anaconda "TensorFlow_GPU_Test" a Jupyter Notebook:
   
   python -m ipykernel install --user --name TensorFlow_GPU_Test --display-name "TensorFlow-GPU"
   
   -instalar tf-agents:
   
   pip install --user tf-agents[reverb]
   
   -instalar las siguientes librerías para ejecutar el tutorial de Reinforce Agent
   
   conda install -c conda-forge xvfbwrapper
   
   conda install -c conda-forge ffmpeg 
   
   conda install -c conda-forge imageio
   
   pip install pyvirtualdisplay
   
   pip install pyglet
   

7- Instalar xming server para virtualizar el renderizado de OpenAI-Gym


Para ejecutar los cuadernos, en Anaconda Prompt:
   conda activate base
   jupyter notebook
Luego abrir el cuaderno deseado y seleccionar el entorno de ejecución "TensorFlow-GPU"





