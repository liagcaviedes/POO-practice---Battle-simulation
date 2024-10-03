
# Simulación de Batalla en Python

Este proyecto es una simulación de una batalla entre dos ejércitos utilizando conceptos de Programación Orientada a Objetos (POO) en Python. Cada unidad del ejército tiene propiedades como nombre, salud, ataque y defensa, lo que permite una dinámica de combate entre las unidades.

## Descripción del Código

El código se organiza en varias clases que representan las unidades y los ejércitos en combate.

### Clases

1. **Unidad**
   - Clase base que representa una unidad en el ejército.
   - Propiedades:
     - `nombre`: Nombre de la unidad.
     - `salud`: Puntos de salud de la unidad.
     - `ataque`: Daño que la unidad puede infligir.
     - `defensa`: Resistencia a los ataques.

   - Métodos:
     - `esta_vivo()`: Devuelve `True` si la unidad tiene salud, de lo contrario `False`.

2. **Arquero, Infanteria, Caballeria**
   - Clases que heredan de `Unidad`.
   - Cada clase inicializa su unidad con atributos específicos.

3. **Ejercito**
   - Representa un ejército compuesto por varias unidades.
   - Propiedades:
     - `nombre`: Nombre del ejército.
     - `unidades`: Lista de unidades en el ejército.
   
   - Métodos:
     - `reclutar_unidad(unidad)`: Agrega una unidad al ejército.
     - `tiene_unidades()`: Verifica si el ejército tiene unidades vivas.

### Funciones de Combate

- **combate(unidad1, unidad2)**
  - Simula el combate entre dos unidades. Cada unidad ataca a la otra y se actualizan sus puntos de salud.

- **batalla(ejercito1, ejercito2)**
  - Simula una batalla entre dos ejércitos, realizando múltiples rondas de combate hasta que uno de los ejércitos no tenga unidades vivas.

### Registro de Batalla

Se registra el resultado de la batalla en un archivo de log (`resultados.txt`) . Se registran los detalles de los ejércitos y el resultado final de la batalla.

## Ejecución

Para ejecutar la simulación de batalla:

1. Asegúrate de tener Python instalado en tu máquina.
2. Guarda el código en un archivo llamado `batalla.py`.
3. Abre la terminal y navega al directorio donde guardaste el archivo.
4. Ejecuta el script con el siguiente comando:

   ```bash
   python batalla.py


