# Usa la misma versión de Python que usaste en Conda (3.9)
FROM python:3.9-slim

# Crea el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia todo el contenido de tu proyecto al contenedor
COPY . /app

# Instala todas las dependencias del archivo requirements.txt sin caché
RUN pip install --no-cache-dir -r requirements.txt

# Indica el puerto que la API va a usar (ej: Flask)
EXPOSE 5000

# Comando para iniciar tu aplicación Flask (asumiendo que se llama app.py)
CMD ["python", "app.py"]