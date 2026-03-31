# Python Fundamentals 101

Repositorio base para preparar el entorno de trabajo de las clases de Python Fundamentals 101.

La idea de este proyecto es dejar listo un setup práctico para aprender y enseñar:

- 🐍 Fundamentos de Python
- 🤖 Uso de programación asistida con IA
- 📓 Jupyter Notebook para exploración y prototipado
- 🌐 Web scraping
- 🧹 Transformación de datos no estructurados a estructurados
- 🧠 Uso básico de modelos y flujos de trabajo con notebooks

Este repositorio parte como entorno de instalación y configuración. Después se puede ir expandiendo con clases, ejercicios, notebooks y ejemplos reales.

## 🎯 Objetivo del repositorio

Este repo servirá como base para:

- ✅ Estandarizar el entorno de desarrollo de la clase
- ✅ Instalar herramientas esenciales desde cero
- ✅ Trabajar con Python, notebooks y automatización
- ✅ Integrar herramientas modernas de IA para acelerar aprendizaje y desarrollo

## 🧰 Stack recomendado

Herramientas base para este curso:

- 💻 `VS Code`: editor principal
- 🐍 `Python 3.11+`: lenguaje principal
- 📦 `pip`: gestor de paquetes de Python
- 🔒 `venv`: entornos virtuales
- 📓 `Jupyter`: notebooks para exploración y demos
- ⚙️ `Node.js LTS`: necesario para varias herramientas de IA y ecosistema JavaScript

## 1. 🚀 Instalar herramientas base

### 💻 VS Code

Descargar e instalar:

- https://code.visualstudio.com/

Extensiones recomendadas:

- `Python` de Microsoft
- `Pylance`
- `Jupyter`
- `Prettier`
- `Material Icon Theme`
- `Copilot` si se va a usar
- `Markdown All in One` para editar documentación

### ⚙️ Configuración básica de VS Code

Configuraciones recomendadas para partir con una experiencia más simple:

- Usar `Command Prompt (cmd)` como terminal por defecto en Windows en vez de PowerShell
- Activar formateo automático al guardar
- Usar iconos visuales para reconocer mejor archivos y carpetas

### Cambiar la terminal por defecto a `cmd` en Windows

1. Abrir VS Code
2. Ir a `Terminal > Select Default Profile`
3. Elegir `Command Prompt`
4. Abrir una nueva terminal

También se puede hacer desde configuración buscando:

- `Terminal › Integrated › Default Profile: Windows`

Y seleccionando:

- `Command Prompt`

### Ajustes recomendados

Puedes abrir `Settings` en VS Code y buscar estas opciones:

- `Format On Save`
- `Terminal Default Profile Windows`
- `Material Icon Theme`

Si prefieres, también puedes usar una configuración como esta:

```json
{
  "editor.formatOnSave": true,
  "terminal.integrated.defaultProfile.windows": "Command Prompt",
  "workbench.iconTheme": "material-icon-theme"
}
```

### 🐍 Python

Descargar Python:

- https://www.python.org/downloads/

Recomendación:

- Usar Python `3.11` o superior
- En Windows, marcar la opción `Add Python to PATH` al instalar

Verificar instalación:

```bash
python --version
```

Si no funciona:

```bash
python3 --version
```

### ⚙️ Node.js

Node.js es útil para instalar y usar varias herramientas modernas de IA por terminal, SDKs y CLIs.

Descargar versión LTS:

- https://nodejs.org/

Verificar instalación:

```bash
node -v
npm -v
```

## 2. 🧪 Crear el entorno del proyecto

Desde la carpeta del repositorio:

```bash
python -m venv .venv
```

Activar el entorno virtual:

### macOS / Linux

```bash
source .venv/bin/activate
```

### Windows PowerShell

```powershell
.venv\Scripts\Activate.ps1
```

Actualizar `pip`:

```bash
python -m pip install --upgrade pip
```

## 3. 📦 Paquetes básicos de Python

Paquetes recomendados para arrancar:

```bash
pip install jupyterlab notebook ipykernel pandas numpy matplotlib seaborn requests beautifulsoup4 lxml openpyxl python-dotenv
```

### ¿Para qué sirve cada uno?

- `jupyterlab`: entorno moderno para notebooks
- `notebook`: soporte clásico de Jupyter
- `ipykernel`: permite usar el entorno virtual dentro de Jupyter
- `pandas`: manipulación de datos tabulares
- `numpy`: operaciones numéricas y arreglos
- `matplotlib`: gráficos base
- `seaborn`: visualización de datos más amigable
- `requests`: llamadas HTTP simples
- `beautifulsoup4`: parsing de HTML
- `lxml`: parser rápido para HTML y XML
- `openpyxl`: lectura y escritura de Excel `.xlsx`
- `python-dotenv`: manejo de variables de entorno desde archivos `.env`

Si más adelante el curso avanza hacia scraping más robusto, automatización o IA, se pueden sumar paquetes como:

```bash
pip install selenium playwright scikit-learn
```

## 4. 📓 Configurar Jupyter

Registrar el entorno virtual como kernel:

```bash
python -m ipykernel install --user --name pythonfundamentals101 --display-name "Python Fundamentals 101"
```

Levantar Jupyter Lab:

```bash
jupyter lab
```

O usar notebooks clásicos:

```bash
jupyter notebook
```

## 5. 🤖 Programación asistida con IA

La idea del curso no es solo aprender Python, sino también aprender a trabajar con asistentes modernos de desarrollo.

Casos de uso:

- ✍️ Explicar código
- ⚡ Generar borradores de funciones
- 🛠️ Refactorizar
- 🧪 Escribir tests
- 📓 Crear notebooks base
- 🕸️ Ayudar con scraping y limpieza de datos
- 🧹 Traducir datos desordenados a estructuras más limpias

## 6. 🧠 Herramientas de IA recomendadas

### Opción A: Copilot en VS Code

Útil para autocompletado y asistencia directa dentro del editor.

Requiere:

- Cuenta habilitada para la herramienta
- Suscripción o acceso activo
- Extensión `Copilot`

### Opción B: Gemini CLI / herramientas de Google

Dependiendo del flujo que quieras usar, muchas herramientas de IA modernas se apoyan en `Node.js` y/o SDKs de JavaScript o Python.

Antes de instalar cualquier CLI:

- Revisar la documentación oficial del proveedor
- Confirmar método de autenticación
- Guardar llaves en variables de entorno, no en el código

### Opción C: Claude

Claude puede usarse desde web, API o herramientas asociadas según el flujo de trabajo disponible.

Buenas prácticas:

- Mantener prompts claros
- No pegar credenciales ni secretos
- Usarlo como copiloto, no como sustituto de validación técnica

### Opción D: Codex / agentes de código

Para trabajar con agentes por terminal o integración con editor, normalmente necesitarás:

- `Node.js` instalado
- Acceso al proveedor correspondiente
- Variables de entorno o login según la herramienta

La instalación exacta puede cambiar según el proveedor o CLI que se use. Recomendación:

- Instalar siempre desde documentación oficial
- Verificar con `--version`
- Probar primero en un repo simple como este

## 7. 🗂️ Recomendación de estructura futura del repo

Una estructura simple para ir creciendo el curso:

```text
PythonFundamentals101/
├── README.md
├── requirements.txt
├── notebooks/
├── clases/
├── ejercicios/
├── datasets/
├── scripts/
└── recursos/
```

### Sugerencia por carpeta

- `notebooks/`: demos en Jupyter
- `clases/`: material por sesión
- `ejercicios/`: práctica para alumnos
- `datasets/`: datos estructurados o crudos
- `scripts/`: utilidades en Python
- `recursos/`: apuntes, guías y referencias

## 8. 📄 Archivo `requirements.txt`

Más adelante puedes crear un `requirements.txt` con algo como esto:

```txt
jupyterlab
notebook
ipykernel
pandas
numpy
matplotlib
seaborn
requests
beautifulsoup4
lxml
openpyxl
python-dotenv
```

Instalación:

```bash
pip install -r requirements.txt
```

## 9. ✅ Primer checklist de setup

- ⬜ Instalar VS Code
- ⬜ Instalar Python 3.11+
- ⬜ Instalar Node.js LTS
- ⬜ Crear y activar `.venv`
- ⬜ Instalar paquetes base con `pip`
- ⬜ Registrar kernel de Jupyter
- ⬜ Abrir el proyecto en VS Code

## 10. 📚 Próximos pasos

Después del setup, este repo puede crecer con sesiones como:

- `Clase 01`: variables, tipos, condicionales y loops
- `Clase 02`: funciones, módulos y manejo de errores
- `Clase 03`: listas, diccionarios y comprensión de datos
- `Clase 04`: lectura de archivos y CSV
- `Clase 05`: scraping básico con `requests` y `BeautifulSoup`
- `Clase 06`: limpieza y estructuración de datos con `pandas`
- `Clase 07`: notebooks, visualización y análisis exploratorio
- `Clase 08`: uso práctico de asistentes de IA para programar mejor

## 📝 Nota

Este `README` es la base del entorno. La siguiente etapa ideal es agregar:

- `requirements.txt`
- estructura de carpetas del curso
- primer notebook de bienvenida
