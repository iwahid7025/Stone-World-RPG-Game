# Stone World RPG

A 2D top-down RPG game built with Unity, featuring grid-based movement, NPC interactions, and random encounter battle mechanics.

## Features

- **Grid-based Movement**: Smooth tile-by-tile character movement with collision detection
- **Animated Character**: Directional animations for walking and idle states (up, down, left, right)
- **NPC Dialogue System**: Interactive dialogue with NPCs using a typewriter text effect
- **Random Encounters**: Pokemon-style battle encounter system triggered by walking on specific tiles
- **Interactable Objects**: Interface-based interaction system for NPCs and other game objects
- **Game State Management**: Clean state transitions between free roam, dialogue, and battle modes

## Project Structure

```
Stone World RPG/
├── Assets/
│   ├── Animation/          # Character animations and animator controller
│   ├── Art/
│   │   ├── Floors/        # Tileset for game world
│   │   ├── Player/        # Character sprites
│   │   └── dialog-box.png # UI dialogue box
│   ├── Scripts/
│   │   ├── PlayerController.cs      # Player movement and input handling
│   │   ├── GameController.cs        # Main game state manager
│   │   ├── DialogManager.cs         # Dialogue system with typewriter effect
│   │   ├── NPCController.cs         # NPC interaction logic
│   │   ├── ChallengerController.cs  # Battle challenger interactions
│   │   ├── Interactable.cs         # Interface for interactable objects
│   │   └── Dialog.cs               # Dialog data structure
│   ├── Scenes/           # Unity scenes
│   └── Tiles/            # Tile assets (cloud tileset)
└── ProjectSettings/      # Unity project configuration
```

## Controls

- **Arrow Keys / WASD**: Move character
- **Z**: Interact with NPCs and objects

## Game Systems

### Movement System
- Grid-based movement with smooth transitions
- Collision detection with solid objects and interactable NPCs
- Layer-based collision using Unity's LayerMask system

### Dialogue System
- Singleton pattern DialogManager for global access
- Typewriter text effect with adjustable speed
- Event-driven dialogue state management
- Multi-line dialogue support

### Encounter System
- 50% chance of triggering a battle on designated battle tiles
- Battle layer detection using overlap circle checks
- Currently displays debug message (battle system to be implemented)

### Game States
- **FreeRoam**: Player can move and interact freely
- **Dialog**: Player movement locked during NPC conversations
- **Battle**: Reserved for battle encounters (implementation pending)

## Technical Details

- **Engine**: Unity (2021.3+)
- **Language**: C#
- **Physics**: Unity 2D Physics system
- **UI**: Unity UI with TextMeshPro support

## Setup Instructions

1. Clone the repository
2. Open the project in Unity (2021.3 or later recommended)
3. Open the scene from `Assets/Scenes/SampleScene.unity`
4. Press Play to test the game

## Development Status

### Implemented
- ✅ Player movement and animations
- ✅ NPC dialogue system
- ✅ Game state management
- ✅ Random encounter detection
- ✅ Interaction system

### In Progress
- 🔨 Battle system implementation
- 🔨 Challenger mechanics

### Planned
- 📋 Battle UI
- 📋 Combat mechanics
- 📋 Additional NPCs and dialogues
- 📋 More maps and areas
- 📋 Save/Load system

## Credits

- **Font**: Orange Kid TTF
- **Tileset**: Cloud tileset
- **Character Sprites**: Custom character sprites

## License

This project is for educational and portfolio purposes.
