# Rebel Assault Game

**Rebel Assault** es un juego 2D basado en sprites desarrollado en C# utilizando principios de Programación Orientada a Objetos (POO). Aunque la estructura del proyecto podría optimizarse, contiene una arquitectura modular con múltiples clases que pueden ser útiles como base para proyectos académicos o prototipos de videojuegos.

> ⚠️ El código está abierto a mejoras. Se aceptan Pull Requests con gusto.

---

## 🎮 Características Principales

- Movimiento: W-A-S-D
- Juego 2D de combate entre personajes y enemigos.
- Uso intensivo de clases para modelar entidades y lógica del juego.
- Manejo básico de interfaz gráfica, colisiones, y sistema de combate.
- Implementación de una barra de vida, puntajes y sistema de audio.
- Utiliza la biblioteca [NAudio](https://github.com/naudio/NAudio) para el manejo del audio.
- Interfaz gráfica desarrollada en **Windows Forms (.NET Framework)**.
- Disparo: Presiona la tecla **Z** para lanzar un proyectil.- El disparo del proyectil se realiza con la tecla **Z** por defecto.


---

## 🧱 Estructura de Clases

### 🔸 `Character.cs`
Gestiona los atributos y comportamientos básicos de un personaje en el juego (vida, daño, posición, etc.).

### 🔸 `CombatSystem.cs`
Encapsula la lógica del sistema de combate. Coordina la interacción entre el jugador, enemigos, proyectiles y colisiones.

### 🔸 `Enemy.cs`
Clase de prueba (`Test Class`) completamente documentada. Representa enemigos básicos y fue usada para experimentación durante el desarrollo.

### 🔸 `EnemyPro.cs`
Versión avanzada del enemigo, con comportamientos más complejos.

### 🔸 `GameManager.cs`
Actúa como el núcleo central del juego. Gestiona los componentes principales, el ciclo del juego y la lógica global.

### 🔸 `GameObject.cs`
Clase base para representar cualquier objeto genérico dentro del juego con propiedades comunes.

### 🔸 `GameOver.cs`
Clase diseñada para gestionar la pantalla de "Game Over". Está documentada, pero incompleta y no funcional actualmente.

### 🔸 `HealthBar.cs`
Gestiona la visualización de la barra de vida de un personaje. Se actualiza en función del estado actual de salud.

### 🔸 `MainCharacter.cs`
Representa al personaje principal controlado por el jugador. Extiende `Character` y añade funcionalidades específicas del jugador.

### 🔸 `Mapa.cs`
Controla la representación visual del mapa del juego y su desplazamiento (scrolling del fondo).

### 🔸 `Projectile.cs`
Modelo de proyectil en el juego con atributos como dirección, daño y propietario (jugador o enemigo).

### 🔸 `ScoreEntry.cs`
Define una entrada de puntuación con información básica del jugador (nombre y puntaje).

### 🔸 `ScoreManager.cs`
Gestiona las puntuaciones: guardado, carga y procesamiento de entradas en el sistema de puntajes.

### 🔸 `SoundManager.cs`
Encapsula la lógica de reproducción de sonidos. Utiliza la biblioteca NAudio para la gestión avanzada de audio en .NET.

## 📚 Documentación del Código

Todas las clases y funciones están documentadas con el formato XML estándar de C#, te servira para:

- Entender fácilmente el propósito y funcionamiento de cada método.
- Visualizar descripciones detalladas directamente desde el IDE (como Visual Studio).
- Generar documentación automática si se desea.

Ideal para quienes quieran profundizar en las clases, extender la lógica del juego o simplemente aprender de la estructura.

---

## 🚀 Cómo empezar

1. Clona el repositorio:
   ```bash
   git clone https://github.com/SsantiDev/Csharp-Game-Sprites.git
