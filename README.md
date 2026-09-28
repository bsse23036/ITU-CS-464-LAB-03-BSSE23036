# ITU-CS-464-LAB-03-BSSE23036

This repository contains the Unity greybox project for Lab-03. The project consists of a blockout level constructed entirely from primitive game objects (cubes, spheres, capsules) turned into reusable prefabs.

---

## Level 1: Tactical Data Center (Treasure Maze)

### Overview & Gameplay Flow

This level adapts a tactical node-based blueprint into a treasure-collection maze. The player spawns at the main entrance (Alpha Spawn) and must navigate a linear 3-meter wide central corridor. The primary objective is to venture off the main path into three isolated side rooms to collect hidden treasure chests before navigating to the exit (Bravo Spawn). The gameplay challenge relies entirely on spatial layout, line-of-sight manipulation, and architectural bottlenecks.

### Obstacles and Environmental Hazards

- **Choke Points & Doorways:** Entrances to the treasure rooms are restricted to exactly 1.5 meters wide. These bottlenecks force the player to commit to a tight space that barely clears the 1m-wide player capsule.
- **Low Cover Barricades:** 1.2-meter tall blocks are positioned strategically in the central corridor and at choke points. This specific height successfully hides a crouching player's proportions while leaving a standing player exposed.
- **Blind Corners:** All enclosing walls are built to a strict 3-meter height. This scale prevents the player from seeing inside the treasure rooms until they commit to the doorway, forcing blind exploration.

### Reason for Level Design Choices

- **Validating Optional Space:** Placing the treasure chests at the very back of the three side rooms provides a clear spatial reward, justifying the player's choice to explore off the main path.
- **Player-Centric Sizing:** The dimensions deliberately contrast comfortable, open movement (3m corridors) with restrictive, cautious navigation (1.5m doorways) based entirely on the player capsule's mechanical limits.
- **Flow vs. Risk:** The linear Spawn-to-Exit route ensures new players will not get lost, while branching into the perpendicular treasure rooms introduces navigational risk by forcing the player to turn their back on the main hallway.

---
