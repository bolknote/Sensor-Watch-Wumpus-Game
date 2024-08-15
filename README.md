# The Wumpus game for [Sensor Watch](https://github.com/joeycastillo/Sensor-Watch)

![screenshot@2x](https://github.com/user-attachments/assets/d432ff68-15f9-4654-850f-7845c071c5a7)

The game begins with you appearing in a random room of the labyrinth as a dodecahedron. The room number is displayed in the top right corner. Each room is connected by tunnels to three other rooms, and you can only move or shoot through these tunnels.

There may be monsters and other hazards around you. If they are one move away, you can see them in the bottom right corner. If there are multiple, the letters will change. W represents the Wumpus, Bt represents a giant bat, and Pt represents a pit. The Wumpus can move through the labyrinth, but bats and pits cannot.

You can shoot arrows at the Wumpus and the bats. You have a total of five arrows. If you run out of arrows, you will die. When shooting, you can choose the distance and specify the rooms through which the arrow will pass. If there is no tunnel between the specified rooms, the arrow will choose a direction randomly. If the arrow hits you, you will die. If you move into a room with a Wumpus, a bat, or a pit, you will die.

At the start of the game, you have two action choices: GO or SHOT. Selection is done with the top-left button, and confirmation is with the top-right button. If you choose GO, you will then need to select one of the three rooms you can move to. Watch out for the monster and trap indicators! Check if there is anything dangerous nearby!

If you choose SHOT, you first need to specify the distance of the shot, and then one by one, specify the rooms through which the arrow will travel. Draw a map! After the first room, the player cannot see, so you will need your map to indicate the second and subsequent rooms.

The game ends in victory (the word "GREAT" on a green background) if you manage to shoot the Wumpus.

### Installation Instructions

1. Copy the two files (`.c` and `.h`) into the `movement/watch_faces/complication` directory of your firmware.
2. Add the line `#include "wumpus_face.h"` to the `movement/movement_faces.h` file.
3. Compile the firmware and upload it to your watch.
