# ParkHub — Juego de simulación de parqueadero

Videojuego de escritorio desarrollado en Java donde el jugador debe estacionar un carro sorteando obstáculos en distintos niveles de dificultad. Proyecto universitario de Programación Orientada a Objetos — Universidad Nacional de Colombia.

## ¿Qué hace?

- El jugador controla un carro con las teclas del teclado
- Debe llegar al espacio de parqueo evitando obstáculos (muros y carros)
- Tiene múltiples niveles con dificultad progresiva
- Registra jugadores y partidas en una base de datos (MySQL)
- Pantallas de inicio, juego, victoria y derrota con imágenes personalizadas

## Tecnologías

- Java (Swing / AWT para la interfaz gráfica)
- POO: clases `Jugador`, `Obstaculos`, `SesionActual`, patrón DAO
- MySQL + JDBC para persistencia de datos
- Maven como gestor de dependencias

## Estructura del proyecto

```
src/
└── main/java/com/mycompany/parkhub/
    ├── ParkHub.java         # Punto de entrada
    ├── Inicio.java          # Pantalla de login/registro
    ├── Formulario.java      # Ingreso de datos del jugador
    ├── Juego.java           # Lógica nivel 1
    ├── Juego2.java          # Lógica nivel 2
    ├── Jugador.java         # Modelo de jugador
    ├── JugadorDAO.java      # Acceso a datos de jugadores
    ├── PartidaDAO.java      # Acceso a datos de partidas
    ├── Obstaculos.java      # Modelo de obstáculos
    ├── ConexionBD.java      # Conexión a la base de datos
    ├── Ganaste.java         # Pantalla de victoria
    └── Perdiste.java        # Pantalla de derrota
```

## Cómo ejecutar

1. Asegúrate de tener Java 11+ y Maven instalados
2. Crea la base de datos usando el archivo `parkhub.sql`
3. Configura tu conexión en `ConexionBD.java`
4. Compila y ejecuta con Maven:
```bash
mvn compile
mvn exec:java
```

## Autor

David Chacón Agudelo — Ingeniería de Sistemas, UNAL
