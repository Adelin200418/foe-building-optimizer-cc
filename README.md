# FOE Building Optimizer

A space optimization tool for Forge of Empires that helps you efficiently place buildings within expansion blocks.

## Features

- **Place 4x4 Expansion Blocks**: Click on the grid to place expansion blocks that define your available space
- **Define Custom Buildings**: Add buildings of any size (width x height) with specified quantities
- **Automatic Optimization**: Algorithm automatically places buildings to maximize space efficiency
- **Visual Feedback**: See your expansion area in green and placed buildings in orange

## How to Use

1. **Open the App**: Simply open `index.html` in your web browser (no build process needed!)

2. **Set Grid Size**:
   - Adjust the grid dimensions if needed (default is 20x20)
   - Click "Create Grid" to apply

3. **Place Expansions**:
   - Click anywhere on the grid to place a 4x4 expansion block (shown in green)
   - Click again on the same area to remove an expansion block
   - The counter shows how many expansion blocks and total cells you have

4. **Add Buildings**:
   - Enter the width and height of a building
   - Specify how many of this building type you want to place
   - Click "Add Building" to add it to the list
   - You can remove buildings from the list if needed

5. **Run Optimizer**:
   - Click "Run Optimizer" to automatically place all buildings
   - Buildings are placed using a greedy algorithm (largest first)
   - Orange cells show placed buildings
   - Results show space efficiency and placement success

## Algorithm

The optimizer uses a greedy bin-packing approach:
- Sorts buildings by area (largest first) for better space utilization
- Attempts to place each building in the first available position
- Reports success rate and space efficiency

## Tech Stack

- Pure HTML/CSS/JavaScript
- No dependencies or build process required
- Works offline in any modern browser
