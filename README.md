# 🧠 Wumpus World Agent (Logic-Based AI Simulation)

A browser-based AI simulation of the classic Wumpus World problem where an agent uses propositional logic and resolution inference to safely navigate a grid containing hidden pits and a Wumpus.

## 📌 Features
- Custom grid size (rows & columns)
- AI agent with Knowledge Base (KB)
- Propositional logic + resolution inference engine
- Breeze (pit warning) and Stench (Wumpus warning) percepts
- Safe-path decision making
- Live HUD (steps, inference count, percepts)
- Visual grid with safe, danger, and unknown states

## 🚀 How to Run
1. Save the code as `index.html`
2. Open it in any browser (Chrome, Firefox, Edge)
3. Set grid size
4. Click **Start**
5. Click **Move** to let the agent explore step by step

## 🎮 How It Works
- Agent starts at (0,0)
- Random pit and Wumpus are generated
- Each move:
  - Agent senses nearby hazards (breeze/stench)
  - Updates Knowledge Base
  - Uses resolution to infer safe cells
  - Chooses next safe move

## 🧠 AI Logic
- Uses propositional symbols:
  - `Pxy` → Pit at (x,y)
  - `Wxy` → Wumpus at (x,y)
  - `¬Pxy`, `¬Wxy` → Negations
- Inference:
  - Breeze → nearby pits possible
  - Stench → nearby Wumpus possible
  - No percept → neighbors are safe
- Decision making via resolution-based theorem proving

## 📊 HUD
- Steps taken
- Logical inference operations
- Current percepts (Breeze/Stench)

## 🎨 UI Legend
- 🟢 Safe / visited
- 🔴 Danger (pit/Wumpus)
- 🟡 Agent position
- ⚪ Unknown cell

## 🏁 Outcome
Agent tries to explore the world safely using logic. If it enters a pit or Wumpus cell → Game Over.

## 📚 Concept Used
Artificial Intelligence, Knowledge-Based Agents, Propositional Logic, Resolution Inference, Wumpus World Problem
