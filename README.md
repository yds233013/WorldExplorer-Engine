# WorldExplorer-Engine

**WorldExplorer-Engine** is a procedurally-generated, tile-based exploration engine built in Java. This project simulates a 2D world where users can generate, explore, and interact with dynamic environments. It includes features like save/load, keyboard-based controls, a HUD interface, and pseudo-randomized world generation based on user-inputted seeds.

## 🚀 Features

- 🗺️ **World Generation**: Procedurally generates a new world from a random seed using rooms and hallways.
- 🧭 **Interactive Exploration**: Navigate using W, A, S, D keys to move your avatar in real-time.
- 💾 **Save & Load**: Quit and resume your exploration at any time with `:Q` and `L` commands.
- 🔠 **HUD (Heads-Up Display)**: Displays tile descriptions and supports custom UI extensions.
- 🎮 **Replayable Worlds**: Deterministic behavior enables reproducibility of any world from input strings.
- 🌟 **Ambitious Features** *(if implemented)*:
  - Light toggles or vision cones
  - Pathfinding enemies
  - Replay visualizations
  - Theme-based or graphical rendering

## 🎮 How to Play

- Run `Main.java` to launch the game.
- Press:
  - `N` followed by a seed and `S` to start a new world (e.g., `N12345S`)
  - `L` to load a previously saved game
  - `:Q` to save and quit
  - Use `W`, `A`, `S`, `D` to move your character

## 🧪 Testing & Autograder Compatibility

- Method `getWorldFromInput(String input)` handles deterministic input testing (e.g., `N12345SWWAAD`).
- Saving is validated using `:Q`, and subsequent `L` reloads the same world state.
- Autograder-compatible structure for testing.

## 📁 Project Structure

```plaintext
src/
├── Core/
│   ├── Main.java
│   ├── World.java
│   └── HyponymsHandler.java
├── TileEngine/
│   ├── TERenderer.java
│   ├── Tileset.java
│   └── TETile.java
├── Utils/
│   ├── RandomUtils.java
│   └── FileUtils.java
📦 Requirements

Java 17+
StdDraw and included tile engine utilities
No external libraries except those provided
