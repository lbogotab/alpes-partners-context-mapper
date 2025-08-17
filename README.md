# 🗺️ Proyecto de Modelado con Context Mapper

Este proyecto contiene la definición de múltiples mapas de contexto para un caso de estudio (Alpes Partners) utilizando **Context Mapper DSL** dentro de un entorno **Dev Container**.

---

# Equipo : Sancochoft

## 👥 Integrantes

| Nombre y Apellido | Usuario GitHub  | Correo                     |
| ----------------- | --------------- | -------------------------- |
| Leiner Barrios    | leinerbarrios   | lj.barrios@uniandes.edu.co |
| Jhorman Galindo   | galindodev      | j.galindop@uniandes.edu.co |
| Alejandro Bogotá  | lbogotab        | l.bogotab@uniandes.edu.co  |
| Jaime Gallo       | salchichongallo | j.gallom@uniandes.edu.co   |

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
├── event-storming/                         # Lenguaje ubicuo
│   ├── P2_AS-IS.jpg
│   └── P2_TO-BE.jpg
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

| Archivo `.cml`                                         | Descripción                             |
| ------------------------------------------------------ | --------------------------------------- |
| `punto_1-AsIs.cml`                                     | Mapa de contexto actual (AS-IS) inicial |
| `Punto_3-AsIs.cml`                                     | Versión avanzada del modelo actual      |
| `Punto_3-ToBe.cml`                                     | Modelo objetivo propuesto (TO-BE)       |
| [Lenguaje Ubicuo AS-IS](./event-storming/P2_AS-IS.jpg) | Lenguaje Ubicuo AS-IS                   |
| [Lenguaje Ubicuo TO-BE](./event-storming/P2_TO-BE.jpg) | Lenguaje Ubicuo TO-BE                   |

---

## Imágenes

### Punto 1 - Dominios y Subdominios AS-IS

![dominios-subdominios-as-is](./src-gen/punto_1-AsIs_ContextMap.png)

### Punto 2 - Lenguaje Ubicuo AS-IS

![lenguaje-as-is](./event-storming/P2_AS-IS.jpg)

### Punto 2 - Lenguaje Ubicuo TO-BE

![lenguaje-to-be](./event-storming/P2_TO-BE.jpg)

### Punto 3 - Mapa de contexto AS-IS

Un solo mapa de contexto. Ver Código para ver subdominios.

![mapa-contexto-as-is](./src-gen/Punto_3-AsIs_ContextMap.png)

### Punto 3 - Mapa de contexto TO-BE

![mapa-contexto-to-be](./src-gen/Punto_3-ToBe_ContextMap.png)

## 📄 Requisitos

- Docker
- Visual Studio Code
- Extensiones: Remote - Containers, Context Mapper
