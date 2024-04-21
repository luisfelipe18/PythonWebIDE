# Python-Web-IDE
-----------
> Un IDE en línea simple para Python  
> Implementado con Vue3 + Python3.10 + Tornado6.1
> Frontend y backend separados

## Descripción de funcionalidades
- Admite la creación, eliminación, consulta y modificación de proyectos, archivos y carpetas
- Admite el autocompletado básico de código Python
- Admite la ejecución y gestión de código Python (no compatible con GUI) y su salida
- Admite la edición y vista previa de archivos Markdown
  
## Notas de actualización
- Nueva implementación basada en Vue3 + Python3.10
- Se incorpora un editor de Markdown
- Se incorporan iconos vscode-icons
- Se cambia el tema del editor

## Compilación y ejecución
### Entorno
- Node: 16.13.2
- Npm: 8.1.2
- Python: 3.10
- Tornado: 6.1

### 前端
```bash
# Instalar dependencias
npm install 或者 yarn install

# Ejecutar en modo desarrollo (el puerto predeterminado es 8080)
npm run serve

# Compilar y empaquetar (la ruta predeterminada del paquete es el directorio dist, el programa backend ya está configurado para cargar recursos desde este directorio)
npm run build
```

### Backend
```bash
# Suponiendo que el entorno de Python ya está instalado (se recomienda utilizar un entorno virtual de Python y activarlo)

# Ingrese al directorio backend  
cd server

# Instalar dependencias
pip install -r requirements.txt

# Ejecutar (el puerto de ejecución es 10086) se puede especificar un puerto con el parámetro --port=10010

# Si la página frontend se ejecuta de forma independiente, no se puede especificar el puerto backend (a menos que se modifique el código frontend)  
python server.py

# Acceder (los proyectos se guardan en projects/ide)

# Ejecutando frontend en modo desarrollo: localhost:8080

# Frontend empaquetado: localhost:10086
```

![py_code](docs/img/py_code.png?raw=true)

![md_code](docs/img/md_code.png?raw=true)

![py_complete](docs/img/py_complete.png?raw=true)

![py_run](docs/img/py_run.png?raw=true)

![projects](docs/img/projects.png?raw=true)
