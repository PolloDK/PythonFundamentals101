# FK Economics Setup

Repositorio base para preparar el entorno de trabajo de `FK Economics`.

La idea de este proyecto es dejar un setup simple y funcional para trabajar con:

- 🐍 Python
- 📓 Jupyter Notebook
- 🌐 scraping y recoleccion de datos
- 🧹 paso de datos no estructurados a estructurados
- 🤖 programacion asistida con IA
- 📊 analisis y exploracion de datos

## 🎯 Objetivo

Este repo servira como base para:

- ✅ instalar el entorno de trabajo de la clase
- ✅ dejar VS Code configurado de forma simple
- ✅ trabajar con Python y notebooks desde el primer dia
- ✅ usar herramientas de IA para acelerar aprendizaje y desarrollo

## 🧰 Stack recomendado

- 💻 `VS Code`
- 🐍 `Python 3.11+`
- 📦 `pip`
- 📓 `Jupyter`
- ⚙️ `Node.js LTS`

## 1. 🚀 Instalar herramientas base

### 💻 VS Code

Descarga:

- https://code.visualstudio.com/

Extensiones recomendadas:

- `Python`
- `Pylance`
- `Jupyter`
- `Prettier`
- `Material Icon Theme`
- `Markdown All in One`

### 🐍 Python

Descarga:

- https://www.python.org/downloads/

Recomendacion:

- usar Python `3.11` o superior
- en Windows, marcar `Add Python to PATH`

Verificacion:

```bash
python --version
```

Si no funciona:

```bash
python3 --version
```

### ⚙️ Node.js

Node.js es necesario para varias herramientas modernas de IA y CLIs.

Descarga:

- https://nodejs.org/

Verificacion:

```bash
node -v
npm -v
```

## 2. ⚙️ Configuracion basica de VS Code

Configuraciones recomendadas para partir:

- usar `Command Prompt (cmd)` como terminal por defecto en Windows
- activar `format on save`
- usar `Material Icon Theme`
- seleccionar Python como interprete del proyecto

### Cambiar terminal por defecto a `cmd`

1. Abrir VS Code
2. Ir a `Terminal > Select Default Profile`
3. Elegir `Command Prompt`
4. Abrir una nueva terminal

Tambien puedes buscar en configuracion:

- `Terminal › Integrated › Default Profile: Windows`

Y dejar:

- `Command Prompt`

### Seleccionar Python como interprete

1. Abrir VS Code en este proyecto
2. Presionar `Ctrl + Shift + P`
3. Buscar `Python: Select Interpreter`
4. Elegir la instalacion de Python que quieras usar

Si instalaste Python desde python.org, normalmente veras algo como:

- `Python 3.11.x`
- `Python 3.12.x`

### Ajustes recomendados

Puedes aplicar una configuracion como esta en VS Code:

```json
{
  "editor.formatOnSave": true,
  "terminal.integrated.defaultProfile.windows": "Command Prompt",
  "workbench.iconTheme": "material-icon-theme",
  "python.defaultInterpreterPath": "python"
}
```

## 3. 📦 Instalar paquetes base de Python

Instalacion recomendada:

```bash
python -m pip install --upgrade pip
pip install jupyterlab notebook ipykernel pandas numpy matplotlib seaborn requests beautifulsoup4 lxml openpyxl python-dotenv
```

### ¿Para que sirve cada uno?

- `jupyterlab`: entorno moderno para notebooks
- `notebook`: soporte clasico de Jupyter
- `ipykernel`: integra Python con notebooks
- `pandas`: manejo de datos tabulares
- `numpy`: operaciones numericas
- `matplotlib`: graficos base
- `seaborn`: visualizacion de datos
- `requests`: llamadas HTTP
- `beautifulsoup4`: lectura de HTML
- `lxml`: parser rapido para HTML y XML
- `openpyxl`: lectura y escritura de Excel
- `python-dotenv`: variables de entorno desde `.env`

## 4. 📓 Jupyter

Para abrir Jupyter Lab:

```bash
jupyter lab
```

Para abrir Jupyter Notebook:

```bash
jupyter notebook
```

## 5. 🤖 Herramientas de IA en Windows

Esta seccion resume formas practicas de instalar herramientas de IA en Windows usando las instrucciones publicas de cada proveedor.

<details>
<summary><strong>Copilot en VS Code</strong></summary>

Segun GitHub Docs, la forma base de comenzar es:

1. Tener acceso a Copilot
2. Instalar la extension de Copilot en tu IDE
3. Iniciar sesion

Pasos practicos en Windows:

1. Abrir VS Code
2. Ir a `Extensions`
3. Buscar `Copilot`
4. Instalar la extension oficial
5. Iniciar sesion cuando VS Code lo pida

Referencia oficial:

- https://docs.github.com/copilot/get-started/setting-up-github-copilot/setting-up-github-copilot-for-yourself

</details>

<details>
<summary><strong>Gemini CLI</strong></summary>

El repositorio oficial de Gemini CLI usa `npm` para la instalacion.

Pasos en Windows:

1. Instalar `Node.js LTS`
2. Abrir `cmd`
3. Ejecutar:

```bash
npm install -g @google/gemini-cli
```

4. Luego ejecutar:

```bash
gemini
```

Normalmente la herramienta te guiara para iniciar sesion o usar una API key, segun el flujo disponible.

Referencia oficial:

- https://github.com/google-gemini/gemini-cli

</details>

<details>
<summary><strong>Claude Code</strong></summary>

La documentacion oficial de Anthropic indica para Windows:

- `Windows 10+`
- `Node.js 18+`
- uso mediante `WSL` o `Git for Windows`

Instalacion base:

1. Instalar `Node.js`
2. Instalar `Git for Windows` si hace falta
3. Abrir una terminal compatible
4. Ejecutar:

```bash
npm install -g @anthropic-ai/claude-code
```

5. Luego iniciar la herramienta con:

```bash
claude
```

Referencia oficial:

- https://docs.anthropic.com/en/docs/claude-code/setup

</details>

<details>
<summary><strong>Codex</strong></summary>

OpenAI indica que Codex puede usarse desde la app, terminal o IDE, y que la app de Codex ya esta disponible en Windows para planes de ChatGPT que incluyen Codex.

Camino simple en Windows:

1. Revisar acceso a Codex desde tu plan
2. Instalar o abrir la app de Codex en Windows
3. Iniciar sesion con tu cuenta de ChatGPT
4. Abrir una carpeta de trabajo y empezar a usarlo

Referencias oficiales:

- https://openai.com/codex/get-started/
- https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan%28.csv
- https://help.openai.com/en/articles/6825453-chatgpt-usage-limits

</details>

## 6. 🗂️ Estructura recomendada del repo

Una estructura simple para este curso:

```text
FKEconomics/
├── data/
├── notebooks/
└── src/
```

### Sugerencia por carpeta

- `data/`: datos crudos, intermedios o limpios
- `notebooks/`: exploracion, demos y clases en Jupyter
- `src/`: scripts y codigo reutilizable

## 7. ✅ Checklist rapido

- ⬜ Instalar VS Code
- ⬜ Instalar Python 3.11+
- ⬜ Instalar Node.js LTS
- ⬜ Instalar extensiones base en VS Code
- ⬜ Dejar `cmd` como terminal por defecto
- ⬜ Seleccionar Python como interprete
- ⬜ Instalar paquetes base con `pip`
- ⬜ Abrir Jupyter

## 8. 💻 Llevar este repo a VS Code

Para trabajar con este repositorio en tu computador, tienes dos opciones simples.

### Opcion A: clonar el repositorio

1. Copiar la URL del repositorio
2. Abrir `cmd`
3. Ir a la carpeta donde quieres guardar el proyecto
4. Ejecutar:

```bash
git clone <URL_DEL_REPO>
```

5. Entrar a la carpeta:

```bash
cd PythonFundamentals101
```

6. Abrir VS Code en esa carpeta:

```bash
code .
```

Si `code .` no funciona, puedes abrir VS Code manualmente y luego ir a:

- `File > Open Folder`

### Opcion B: descargar ZIP

1. Entrar al repositorio en GitHub
2. Descargar `Code > Download ZIP`
3. Descomprimir la carpeta
4. Abrir VS Code
5. Ir a `File > Open Folder`
6. Elegir la carpeta del proyecto

### Una vez abierto en VS Code

Haz estas tres cosas:

1. Abrir una terminal
2. Verificar Python con:

```bash
python --version
```

3. Instalar paquetes base:

```bash
python -m pip install --upgrade pip
pip install jupyterlab notebook ipykernel pandas numpy matplotlib seaborn requests beautifulsoup4 lxml openpyxl python-dotenv
```
