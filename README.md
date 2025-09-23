# 🤖 Mobile Robot Rescue Mission – Path Planning Application
This project is a **Flutter-based application** for **map-based path planning** with obstacle avoidance. It allows users to define a **working area**, **start point**, **goal point**, and **obstacles**, then runs a path planning algorithm to compute an efficient route.

---

## ✨ Features

- **Custom Map Selection**  
  - Select or create a map based on the real world.  
  - Save maps for later use.  

- **Define Environment**  
  - Set the **working area**.  
  - Define the **start position** and **end (goal) position**.  
  - Add **obstacles** to the map.  

- **Path Planning Algorithm**  
  - Computes a path from the start to the goal point while avoiding obstacles.  
  - Uses **cellular decomposition** to divide the map into smaller regions (cells).  
  - Finds the path through **cell centers** for efficient navigation.  

- **Dynamic Ground-Based Path Planning**  
  - Once a path is calculated between cell centers, it is **stored in memory**.  
  - Future queries for the same cell-to-cell paths are **retrieved directly** instead of recalculated.  
  - Significantly improves **time efficiency** for repeated computations.  

---

## 🚀 How It Works

1. Select or create a **map**.  
2. Define:  
   - Working area  
   - Obstacles  
   - Start point  
   - Goal point  
3. The application:  
   - Divides the map into **cells** (cellular decomposition).  
   - Computes the optimal path via **cell centers**.  
   - Stores computed cell-to-cell paths for future reuse.  
4. Retrieve paths efficiently in future runs without recalculating.  

---

## 🛠️ Tech Stack

- **Frontend:** Flutter  
- **Backend / Logic:** Path Planning Algorithm (Cellular Decomposition + Memory Optimization)  
- **Storage:** Local map and path data storage for reuse  

---



---

## 🎯 Use Cases

- Robotics navigation  
- Drone and ground vehicle simulations  
- Obstacle-aware path planning  
- Real-time applications where **fast path retrieval** is crucial  

---

## 🔮 Future Enhancements

- Support for multiple path planning algorithms (A*, RRT, D* Lite, etc.)  
- Cloud sync for maps and path data  
- Integration with real-world GPS and sensor data  
- Visualization improvements for 3D maps  

---

## 📸 Screenshots

*(Add screenshots of your Flutter app here)*  

---

## 📜 License

This project is open-source. You are free to use, modify, and distribute under the terms of the license provided in this repository.

