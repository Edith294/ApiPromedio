# API de Promedio de Calificaciones con Flask

API REST desarrollada con Python y Flask que calcula el promedio de calificaciones de un estudiante.

## Tecnologías utilizadas

- Python
- Flask

## Estructura del proyecto
```
api_promedio/
├── venv/
├── app.py
└── requirements.txt
```
## Probar con postman
<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/43845cf5-ef91-4772-893d-ebcb29de5259" />


## Instalación

### 1. Clonar el repositorio
```bash
git clone https://github.com/TU_USUARIO/TU_REPOSITORIO.git
cd api_promedio
```

### 2. Crear y activar el entorno virtual
```bash
python -m venv venv
```

En Windows:
```bash
venv\Scripts\activate
```

En Linux/Mac:
```bash
source venv/bin/activate
```

### 3. Instalar dependencias
```bash
pip install -r requirements.txt
```

### 4. Ejecutar la aplicación
```bash
python app.py
```

El servidor correrá en: `http://127.0.0.1:5000`

## Endpoint disponible

| Método | Ruta | Descripción |
|--------|------|-------------|
| POST | /promedio | Calcula el promedio de calificaciones |

## Prueba en Postman

**Método:** `POST`  
**URL:** `http://127.0.0.1:5000/promedio`  
**Body → raw → JSON:**
```json
{
  "nombre": "Juan",
  "calificaciones": [80, 90, 85, 70]
}
```

## Resultado esperado
```json
{
  "nombre": "Juan",
  "promedio": 81.25
}
```
