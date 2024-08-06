#### AI-Project1
This project involves developing and comparing the performance of four different bot algorithms to rescue a captain trapped in a randomly generated ship layout filled with obstacles (walls) and aliens. The primary objective is to navigate from the bot's starting position to the captain's location while avoiding or surviving encounters with aliens.

## Key Components:
- Ship Layout Generation:
A ship grid of dimension D×D is generated randomly with '0' closed cells, '1' representing open cells, 'B' for the bot, 'A' for aliens, and 'C' for the captain.
- Visualization:
Functions are provided to visualize the ship's layout and the bot's path, including the game status (success, failure, or no path found).
- Pathfinding and Movement:
Heuristic Function: Uses Manhattan distance to estimate the cost from the current position to the goal.
A-Star Algorithm: Finds the shortest path from the bot to the captain using the heuristic function.
Alien Movement: Aliens move randomly to adjacent open cells after each bot move.
Bot Algorithms:
Bot 1: Uses A-Star to find the shortest path to the captain without considering aliens.
Bot 2: Recalculates the path to the captain in each iteration to adapt to the changing positions of aliens.
Bot 3: Considers cells adjacent to aliens as blocked when calculating the path to the captain.
Bot 4: Uses a heuristic that penalizes paths closer to aliens, thus avoiding them more effectively.
- Simulation and Evaluation:
Each bot's performance is evaluated over multiple epochs, recording success and survival rates.
Success rates and survival times are calculated and plotted to compare the efficiency and robustness of each bot algorithm.
- Results Visualization:
Plots showing the success rates of each bot algorithm against the number of aliens provide a clear comparison of their performance.
This project demonstrates the implementation and comparison of various pathfinding and heuristic strategies in dynamic and uncertain environments, with potential applications in robotics and AI navigation systems.
