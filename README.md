# Battle Simulation in Python

This project is a simulation of a battle between two armies using concepts of Object-Oriented Programming (OOP) in Python. Each unit of the army has properties such as name, health, attack, and defense, allowing for a dynamic combat system between the units.

## Code Description

The code is organized into several classes that represent the units and armies in combat.

### Classes

1. **Unit**
   - Base class representing a unit in the army.
   - Properties:
     - `name`: Name of the unit.
     - `health`: Health points of the unit.
     - `attack`: Damage the unit can inflict.
     - `defense`: Resistance to attacks.

   - Methods:
     - `is_alive()`: Returns `True` if the unit has health; otherwise, returns `False`.

2. **Archer, Infantry, Cavalry**
   - Classes that inherit from `Unit`.
   - Each class initializes its unit with specific attributes.

3. **Army**
   - Represents an army composed of several units.
   - Properties:
     - `name`: Name of the army.
     - `units`: List of units in the army.
   
   - Methods:
     - `recruit_unit(unit)`: Adds a unit to the army.
     - `has_units()`: Checks if the army has any living units.

### Combat Functions

- **combat(unit1, unit2)**
  - Simulates the combat between two units. Each unit attacks the other, and their health points are updated.

- **battle(army1, army2)**
  - Simulates a battle between two armies, performing multiple rounds of combat until one army has no living units.

### Battle Logging

The results of the battle are logged into a log file (`battle.log`) using the `logging` module. Details of the armies and the final outcome of the battle are recorded.

## Execution

To run the battle simulation:

1. Ensure you have Python installed on your machine.
2. Save the code in a file named `battle.py`.
3. Open the terminal and navigate to  directory where you saved the file.
4. Run the script with the following command:
   bash
   python battle.py
5. Check the battle.log file to see the battle results.

### Example Usage
When running the script, the combats between units will be displayed in the console, and the results of the battle will be saved in battle.log.
Round 1
Archer (100 HP) vs Infantry (150 HP)
Archer deals 5 damage to Infantry
Infantry deals 10 damage to Archer
...
Red Army has won

### Notes
You can customize the number of recruited units and their types by modifying the recruitment loop.
Ensure you have write permissions in the directory where the script is executed to create the log file.

### License
This repository is open-source and available under the MIT License.

### Author
- **Name**: Rosalía González Caviedes
- **Email**: rosaliagonzalezc@gmail.com
- [LinkedIn profile](https://www.linkedin.com/in/rosaliagonzalezcaviedes/)
- [Github profile](https://github.com/liagcaviedes)







