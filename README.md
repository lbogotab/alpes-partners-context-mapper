# 🗺️ Proyecto de Modelado con Context Mapper 

Este proyecto contiene la definición de múltiples mapas de contexto para un caso de estudio (Alpes Partners) utilizando **Context Mapper DSL** dentro de un entorno **Dev Container**.

---


# Equipo : Sancochoft

## 👥 Integrantes

| Nombre y Apellido    | Usuario GitHub      | Correo                      | Código Uniandes |
|----------------------|---------------------|-----------------------------|-----------------|
| Leiner Barrios       | leinerbarrios       | lj.barrios@uniandes.edu.co | 202322761       |
| Jhorman Galindo      | galindodev          | j.galindop@uniandes.edu.co | 202413944       |
| Alejandro Bogotá     | lbogotab            | l.bogotab@uniandes.edu.co  | 202412270       |
| Jaime Gallo          | salchichongallo     | j.gallom@uniandes.edu.co   | 202412276       |



## 📦 Estructura del Proyecto

```bash
.
├── .devcontainer/               # Configuración del Dev Container
│   ├── devcontainer.json
│   └── Dockerfile
├── cml/                         # Archivos fuente en Context Mapper DSL
│   ├── punto_1-AsIs.cml
│   ├── Punto_3-AsIs.cml
│   └── Punto_3-ToBe.cml
├── src-gen/                     # Diagramas generados automáticamente
│   ├── punto_1-AsIs_ContextMap.svg
│   ├── Punto_3-AsIs_ContextMap.svg
│   └── Punto_3-ToBe_ContextMap.svg
└── README.md
```

---

## 🚀 Cómo ejecutar el Dev Container

1. Abre el proyecto en **Visual Studio Code**.

2. Asegúrate de tener instaladas estas extensiones:
   - [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
   - [Context Mapper](https://marketplace.visualstudio.com/items?itemName=org.contextmapper.context-mapper-vscode)

3. Haz clic en la esquina inferior izquierda de VS Code y selecciona:
   > **"Reabrir en contenedor"** (Reopen in Container)

4. Espera a que el entorno se construya. Esto puede tardar unos minutos la primera vez.

---

## 🛠️ Generar los diagramas

Una vez dentro del Dev Container, para cada archivo `.cml`:

1. Abre el archivo deseado, por ejemplo:  
   `cml/Punto_3-ToBe.cml`

2. Haz clic derecho en cualquier parte del archivo y selecciona:
   > **"Context Mapper: Generate Context Map Diagram"**

3. El resultado se generará en `src-gen/` como un archivo `.svg`  
   Ejemplo: `Punto_3-ToBe_ContextMap.svg`

---

## 🧩 Archivos importantes

| Archivo `.cml`                | Descripción                             |
|------------------------------|-----------------------------------------|
| `punto_1-AsIs.cml`           | Mapa de contexto actual (AS-IS) inicial |
| `Punto_3-AsIs.cml`           | Versión avanzada del modelo actual      |
| `Punto_3-ToBe.cml`           | Modelo objetivo propuesto (TO-BE)       |

---

## 📄 Requisitos

- Docker
- Visual Studio Code
- Extensiones: Remote - Containers, Context Mapper
