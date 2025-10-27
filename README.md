# 1--Proyecto-Tic-Tac-Toe
Este programa implementa el juego clásico de Tic Tac Toe (también conocido como Gato o Tres en Raya) en C++. El juego se desarrolla en un tablero de 3x3 donde dos jugadores se turnan para colocar sus marcas (X y O). El objetivo es conseguir tres marcas en línea ya sea horizontal, vertical o diagonal.
🎮 TIC TAC TOE (Gato/Tres en Raya)
📋 Descripción del Programa
Este programa implementa el juego clásico de Tic Tac Toe (también conocido como Gato o Tres en Raya) en C++. El juego se desarrolla en un tablero de 3x3 donde dos jugadores se turnan para colocar sus marcas (X y O). El objetivo es conseguir tres marcas en línea ya sea horizontal, vertical o diagonal.
✨ Características

Dos modos de juego:

Jugador vs Jugador: Dos personas juegan en el mismo dispositivo turnándose
Jugador vs CPU: Juega contra la computadora con inteligencia artificial básica


Interfaz visual mejorada con caracteres especiales para un tablero atractivo
Validación robusta de todas las entradas del usuario
Detección automática de ganadores y empates
Sistema de menú interactivo fácil de usar
Compatible con Windows, Linux y macOS

🛠️ Requisitos del Sistema

Compilador de C++ (g++, clang++ o Visual Studio)
Sistema operativo: Windows, Linux o macOS
Terminal o consola de comandos

📥 Instalación y Compilación
En Linux/Mac:
bash# Compilar el programa
g++ tictactoe.cpp -o tictactoe

# Ejecutar el programa
./tictactoe
En Windows (con MinGW/g++):
bash# Compilar el programa
g++ tictactoe.cpp -o tictactoe.exe

# Ejecutar el programa
tictactoe.exe
En Windows (con Visual Studio):

Abrir Visual Studio
Crear un nuevo proyecto de C++ (Consola)
Copiar el código en el archivo principal
Compilar y ejecutar con F5

🎯 Instrucciones de Uso
1. Inicio del Programa
Al ejecutar el programa, verás el menú principal con tres opciones:
╔════════════════════════════════╗
║     TIC TAC TOE - MENU        ║
╚════════════════════════════════╝
  1. Jugar contra otro jugador
  2. Jugar contra la CPU
  3. Salir
─────────────────────────────────
  Seleccione una opción:
2. Selección del Modo de Juego

Opción 1: Para jugar con otra persona (ambos en el mismo dispositivo)
Opción 2: Para jugar contra la computadora
Opción 3: Para salir del programa

3. Durante el Juego
El Tablero
El tablero muestra las coordenadas en los bordes:
     1   2   3
   ┌───┬───┬───┐
 1 │   │   │   │
   ├───┼───┼───┤
 2 │   │   │   │
   ├───┼───┼───┤
 3 │   │   │   │
   └───┴───┴───┘
Cómo Jugar

Cuando sea tu turno, el programa te pedirá:

Fila: Ingresa un número del 1 al 3
Columna: Ingresa un número del 1 al 3


Ejemplo de jugada:

   Turno del jugador X
   Ingrese fila (1-3): 2
   Ingrese columna (1-3): 2

Tu marca (X u O) aparecerá en la posición seleccionada
Los jugadores se alternan hasta que:

Un jugador consiga tres en línea (¡Ganador!)
El tablero se llene sin ganador (Empate)



4. Condiciones de Victoria
Un jugador gana al conseguir tres marcas consecutivas en:

Fila horizontal: X X X
Columna vertical:

  X
  X
  X

Diagonal principal: X _ _ / _ X _ / _ _ X
Diagonal secundaria: _ _ X / _ X _ / X _ _

5. Modo Jugador vs CPU

Tú juegas con: X (siempre juegas primero)
La CPU juega con: O
La CPU selecciona automáticamente sus jugadas
El programa te indicará dónde jugó la CPU

🎲 Ejemplos de Partida
Ejemplo 1: Victoria en Fila
     1   2   3
   ┌───┬───┬───┐
 1 │ X │ X │ X │  ← ¡Jugador X gana!
   ├───┼───┼───┤
 2 │ O │ O │   │
   ├───┼───┼───┤
 3 │   │   │   │
   └───┴───┴───┘
Ejemplo 2: Victoria en Diagonal
     1   2   3
   ┌───┬───┬───┐
 1 │ X │ O │ O │
   ├───┼───┼───┤
 2 │ O │ X │   │
   ├───┼───┼───┤
 3 │   │   │ X │
   └───┴───┴───┘
   
¡Jugador X gana con diagonal!
Ejemplo 3: Empate
     1   2   3
   ┌───┬───┬───┐
 1 │ X │ O │ X │
   ├───┼───┼───┤
 2 │ O │ O │ X │
   ├───┼───┼───┤
 3 │ X │ X │ O │
   └───┴───┴───┘
   
¡Es un empate!
⚠️ Mensajes de Error Comunes

"❌ Opción inválida": Has ingresado un número fuera del rango permitido o un carácter no numérico
"❌ Entrada inválida": Has ingresado texto en lugar de números
"❌ Posición ocupada o inválida": La casilla que seleccionaste ya tiene una marca

🔧 Notas Técnicas
Estructuras de Datos

Tablero: Array bidimensional char[3][3]
Jugadores: Constantes de caracteres (X y O)

Algoritmos Implementados

Validación de entrada: Previene errores por datos incorrectos
Verificación de ganador: Revisa filas, columnas y diagonales
Detección de empate: Verifica si el tablero está lleno
IA de la CPU: Selección aleatoria de casillas vacías (nivel básico)

Compatibilidad

Windows: Usa cls para limpiar pantalla
Linux/Mac: Usa clear para limpiar pantalla

🚀 Posibles Mejoras Futuras

 Implementar IA más inteligente (minimax)
 Agregar dificultades (fácil, medio, difícil)
 Sistema de puntuación y estadísticas
 Guardar historial de partidas
 Modo multijugador en red
 Interfaz gráfica (GUI)
 Sonidos y efectos visuales
 Tableros de diferentes tamaños (4x4, 5x5)

👨‍💻 Autor
Cristóbal Lemus

Versión: 1.0
Fecha: 2025
Lenguaje: C++

📄 Licencia
Este proyecto es de código abierto y está disponible para uso educativo.
🤝 Contribuciones
Las sugerencias y mejoras son bienvenidas. Si encuentras algún error o tienes ideas para mejorar el juego, no dudes en compartirlas.

¡Disfruta del juego! 🎮✨
