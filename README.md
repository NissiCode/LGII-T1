# LGII-T1
Primer codigo de Python 
---

## 📌 Descripción del Proyecto

Módulo en Python diseñado para **Google Colab** que permite montar unidades de Google Drive, explorar directorios específicos configurados mediante constantes y procesar/validar archivos de datos de forma estructurada y segura.

---

## ✨ Funcionalidades Principales

| # | Requisito | 🛠️ Implementación / Solución |
| :-: | :--- | :--- |
| **1** | **Filtrado Selectivo** | Muestra exclusivamente archivos `.json` y `.csv` mediante la constante `EXTENSIONES_VALIDAS`. |
| **2** | **Metadatos Detallados** | Obtiene el tamaño exacto en **KB** (`os.path.getsize`) y la fecha/hora de última modificación (`os.path.getmtime`). |
| **3** | **Parseo Estructurado** | Si detecta `inventario.json`, lo analiza con `json.load()` y valida que sea una lista de registros válida. |
| **4** | **Retorno Modular** | `list_files_in_directory(directorio)` retorna un diccionario estandarizado ideal para consumir desde APIs. |

> 🛡️ **Manejo de Excepciones Integrado:** Controla errores comunes como directorios inexistentes (`FileNotFoundError`) o archivos JSON corruptos (`json.JSONDecodeError`).

---

## 🗂️ Estructura del Repositorio

```text
📦 explorador-drive
 ├── 📄 explorador_drive.py       # Código fuente principal
 ├── 📜 LICENSE                   # Licencia de uso MIT
 ├── 🙈 .gitignore                # Archivos ignorados por Git
 └── 📘 README.md                 # Documentación del proyecto



2️⃣ Clonación y Ejecución
Ejecuta los siguientes comandos en una celda de tu cuaderno de Google Colab:

Python
!git clone [https://github.com/](https://github.com/)<tu-usuario>/<tu-repositorio>.git
%cd <tu-repositorio>
%run explorador_drive.py



📄 Licencia
Este proyecto se distribuye bajo la Licencia MIT. Para más información, consulta el archivo LICENSE.
