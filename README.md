# Buscaminas en MARIE.js

Este proyecto consiste en la implementación del juego Buscaminas utilizando la arquitectura educativa MARIE.js, junto con un script en Python para la generación del tablero.

## Descripción

El sistema está dividido en dos partes:

- Python: genera un tablero de Buscaminas de 16x16 con minas aleatorias y calcula las minas vecinas.
- MARIE.js: ejecuta la lógica del juego, procesa la entrada del usuario y muestra el tablero mediante un display de colores.

El tablero generado en Python se convierte en un bloque de memoria compatible con MARIE, el cual es utilizado por el programa en ensamblador.

---

## Características

- Tablero de 16x16 (256 celdas)
- Número de minas configurable
- Representación visual mediante colores
- Sistema de banderas
- Expansión automática de celdas vacías (BFS)
- Detección de victoria y derrota

---

## Tecnologías utilizadas

- Python
- MARIE.js (simulador de arquitectura)
- Google Colab

---

## Cómo ejecutar

### 1. Generar tablero (Python)

Ejecutar el script en Google Colab:

1. Ejecutar el código  
2. Ingresar el número de minas  
3. Se generarán:
   - `tablero_buscaminas.png`
   - `codigo_marie_actualizado.mas`

---

### 2. Ejecutar en MARIE.js

1. Abrir el simulador:  
   https://marie.js.org/

2. Cargar el archivo

3. Ejecutar el programa

---

## Cómo jugar

El programa recibe tres entradas:

1. Fila (0–15)  
2. Columna (0–15)  
3. Acción:  
- 1 → Revelar celda  
- 2 → Colocar/Quitar bandera  

---

## Representación de colores

| Estado | Color |
|------|------|
| Oculto | Gris oscuro |
| Bandera | Amarillo |
| Mina | Negro |
| 0 | Gris claro |
| 1 | Azul |
| 2 | Verde |
| 3 | Rojo |
| 4 | Azul oscuro |
| 5 | Rojo oscuro |
| 6 | Cian |
| 7 | Violeta |
| 8 | Blanco |

---

## Autores

- Estefanía Solórzano  
- Giuliana Auqui  
- Daniel Pérez  
- Pamela Barbosa  

---

## Referencias

- MARIE.js: https://github.com/MARIE-js/MARIE.js
