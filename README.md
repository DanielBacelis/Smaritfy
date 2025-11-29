# Smaritfy
Recomendador Musical Inteligente basado en IA
<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/e84a87cd-c458-477c-8ab4-7289fe71a3dd" />


## 1. Introducción 
El presente documento tiene como objetivo presentar la arquitectura del sistema Smartify, un recomendador musical inteligente inspirado en la plataforma Spotify. Este sistema busca mejorar la experiencia del usuario a través de un modelo de inteligencia artificial capaz de analizar gustos, emociones y contexto de uso para ofrecer recomendaciones musicales altamente personalizadas.


#  Arquitectura del Sistema Smartify (Modelo C4)


## 1. Introducción
El sistema **Smartify** es un recomendador musical inteligente inspirado en Spotify. Su objetivo es mejorar la experiencia del usuario mediante un modelo de **Inteligencia Artificial** que analiza **gustos, emociones y contexto** de uso para ofrecer recomendaciones altamente personalizadas.


## 2. Justificación
A diferencia de las plataformas actuales que se basan solo en patrones de escucha y popularidad, Smartify utiliza la **IA para interpretar el estado de ánimo y las emociones** del usuario, buscando generar una experiencia de entretenimiento más humana y adaptativa.


## 3. Metodología de Arquitectura: Modelo C4
Para la documentación se emplea el **Modelo C4**, que descompone el sistema en cuatro niveles jerárquicos:

* **Nivel 1: Diagrama de Contexto (C1)**: Relación entre el sistema y sus actores externos.
* **Nivel 2: Diagrama de Contenedores (C2)**: Descripción de los principales subsistemas o módulos.
* **Nivel 3: Diagrama de Componentes (C3)**: Detalles de las partes internas de cada contenedor.
* **Nivel 4: Diagrama de Código (C4)**: Estructura lógica del software.

---



## 4. Estructura del Sistema (Diagramas C4)


### 4.1. C1: Diagrama de Contexto
Smartify interactúa con el **Usuario** (vía App Móvil/Web), un **Servicio de Música** externo y la **Nube** (para hosting/computación).

### 4.2. C2: Diagrama de Contenedores
El sistema se divide en contenedores principales, comunicados vía **API REST**:
* **Aplicación Cliente (Frontend)**
* **Servidor Backend**
* **Motor de IA (Microservicio)**
* **Base de Datos**

### 4.3. C3: Diagrama de Componentes (Backend)
El Servidor Backend incluye:
* **Gestor de Usuarios**
* **Módulo de Recomendación**
* **Administrador de Listas de Reproducción**
* **Analizador de Emociones**

### 4.4. C4: Diagrama de Código Lógico
Clases clave (Organización Conceptual):
* `Usuario`
* `Cancion`
* `RecomendadorIA`
* `ListaReproduccion`

---



## 5. Descripción de Módulos Técnicos


* **Módulo Frontend**: Interfaz de usuario para interacción directa (Web/Móvil).
* **Módulo Backend**: Procesa solicitudes, gestiona usuarios y coordina el flujo de datos.
* **Módulo de Inteligencia Artificial (IA)**: Analiza patrones de escucha y **genera recomendaciones personalizadas**.
* **Base de Datos**: Almacena información persistente (usuarios, canciones, historial, configuraciones).
* **API REST**: Protocolo de comunicación principal entre contenedores.

---



## 6. Requerimientos del Sistema


### 6.1. Requerimientos Funcionales (RF)
* **RF1**: Gestión de perfil (registro, login, edición).
* **RF2**: Generación de recomendaciones personalizadas basadas en IA.
* **RF3**: Creación, edición y eliminación de listas de reproducción.
* **RF4**: Reproducción de contenido (canciones, álbumes, artistas).
* **RF5**: Registro del comportamiento del usuario para optimizar la IA.

### 6.2. Requerimientos No Funcionales (RNF)
* **RNF1: Disponibilidad**: Mínima del 99%.
* **RNF2: Rendimiento**: Tiempo de respuesta inferior a 2 segundos.
* **RNF3: Usabilidad**: Interfaz intuitiva, moderna y responsiva.
* **RNF4: Seguridad**: Protección de datos mediante cifrado y autenticación segura.
* **RNF5: Escalabilidad**: Capacidad de soportar millones de usuarios.

---

## 7. Diagramas UML


### 7.1 Diagrama C4 Nivel 1: Contexto
Este diagrama (C1) muestra cómo el sistema Smartify interactúa con sus actores externos principales: el usuario, el servicio de música y la nube.

<img width="592" height="706" alt="image" src="https://github.com/user-attachments/assets/bc866d5e-c72e-450a-a64c-fdf0e3c02a8b" />


### 7.2 Diagrama C4 Nivel 2: Contenedores

Este diagrama (C2) descompone Smartify en los contenedores principales: la aplicación cliente, el servidor backend, el motor de IA y la base de datos. La comunicación se realiza mediante API REST.

<img width="508" height="558" alt="image" src="https://github.com/user-attachments/assets/a1fd6028-d570-4d9a-a19e-98bb25026c8e" />

### 7.3 Diagrama C4 Nivel 3: Componentes
Este diagrama (C3) se enfoca en la estructura interna del Servidor Backend, mostrando componentes clave como el gestor de usuarios, el módulo de recomendación, el administrador de listas de reproducción y el analizador de emociones.

<img width="900" height="553" alt="image" src="https://github.com/user-attachments/assets/982cba8c-6f07-40e4-a385-339f9d73f170" />

### 7.4 Diagrama C4 Nivel 4: Código Lógico
Este diagrama (C4) representa la organización conceptual del software, enfocándose en las clases clave: Usuario, Canción, RecomendadorIA y ListaReproducción, y cómo interactúan entre sí.

<img width="900" height="586" alt="image" src="https://github.com/user-attachments/assets/144fd6e0-5d5f-4d2c-b6db-d9bb0c912155" />

## 8. Conclusión
Smartify representa una arquitectura sólida y modular basada en el **Modelo C4**, con un fuerte enfoque en la personalización y la sensibilidad emocional a través de la IA. Este diseño garantiza **escalabilidad** y adaptabilidad para futuras evoluciones.
##

