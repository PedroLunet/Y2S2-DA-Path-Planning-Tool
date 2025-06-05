# Path Planning Tool - Urban Navigation System

![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=for-the-badge&logo=cmake&logoColor=white)
![Algorithm](https://img.shields.io/badge/Algorithm-Dijkstra-red?style=for-the-badge)
![Graph Theory](https://img.shields.io/badge/Graph_Theory-Implementation-green?style=for-the-badge)

A sophisticated path-planning tool developed in C++ for the Design of Algorithms (DA) course at FEUP. This project demonstrates advanced algorithmic implementations with real-world urban navigation capabilities, featuring optimized routing algorithms and comprehensive data management.

## 🌐 About

The Path Planning Tool is a comprehensive urban navigation system that assists users in finding optimal routes between locations. Built with performance and flexibility in mind, it offers:

- Advanced graph-based routing algorithms
- Multi-modal transportation support (driving and walking)
- Real-time route optimization with constraints
- Comprehensive location and distance data management
- Interactive command-line interface for seamless user experience
- Environmentally-conscious routing options

## 🚀 Features

### 🛣️ Routing Capabilities

- **Independent Routing**: Find the fastest route between any two locations using optimized pathfinding
- **Restricted Routing**: Calculate optimal routes with specific transportation or time constraints
- **Environmentally-Friendly Routing**: Discover eco-optimal routes combining driving and walking segments
- **Multi-Modal Support**: Seamless integration of different transportation methods

### 📊 Advanced Algorithms

- **Dijkstra's Algorithm**: Optimized shortest path implementation with O(E log V) complexity
- **Custom Priority Queue**: Mutable priority queue for efficient algorithm execution
- **Graph Processing**: Template-based graph structure supporting weighted edges and vertices
- **Dynamic Filtering**: Real-time edge filtering for constraint-based routing

### 💾 Data Management

- **CSV Integration**: Efficient parsing of location and distance data from CSV files
- **Location Database**: Comprehensive location management with parking availability tracking
- **Distance Matrix**: Optimized storage and retrieval of inter-location distances
- **Data Validation**: Robust error handling and data integrity checks

### 🎯 User Interface

- **Interactive Menu**: Intuitive command-line interface for all operations
- **Real-time Feedback**: Live route calculation and timing information
- **Error Handling**: Comprehensive input validation and error messaging
- **Results Display**: Clear presentation of routes, distances, and timing data

## 🛠 Technical Implementation

### Tech Stack

- **Language**: C++14 with modern STL features
- **Build System**: CMake for cross-platform compilation
- **Data Storage**: CSV files for location and distance data
- **Documentation**: Doxygen for comprehensive API documentation

### System Architecture

```
┌─────────────────────┐
│   Menu Interface    │
├─────────────────────┤
│  Routing Algorithms │
├─────────────────────┤
│   Graph Structure   │
├─────────────────────┤
│   Data Management   │
├─────────────────────┤
│   CSV Data Files    │
└─────────────────────┘
```

### Core Components

- **Graph Structure**: Template-based implementation with vertices and weighted edges
- **Routing Engine**: Dijkstra's algorithm with customizable edge filtering
- **Data Parser**: Efficient CSV parsing for locations and distances
- **Graph Builder**: Dynamic graph construction from parsed data
- **Menu System**: User-friendly interface for all routing operations

## 🏗 Setup and Installation

### Prerequisites

- C++14 compatible compiler (GCC 5.4+, Clang 3.8+, MSVC 2017+)
- CMake 3.26 or higher
- Standard C++ libraries

### Quick Start

```bash
# Clone the repository
git clone [repository-url]
cd Y2S2-DA-Path-Planning-Tool

# Create build directory
mkdir build && cd build

# Configure with CMake
cmake ../src

# Build the project
make

# Run the application
./project1-da-leic
```

### Alternative Build (without CMake)

```bash
# Navigate to source directory
cd src

# Compile manually
g++ -std=c++14 -O2 -o path_planner main.cpp menu/Menu.cpp \
    parse_data/ParseData.cpp parse_data/DataManager.cpp \
    graph_builder/GraphBuilder.cpp routing/Routing.cpp

# Run the executable
./path_planner
```

## 📁 Project Structure

```
Y2S2-DA-Path-Planning-Tool/
├── src/                    # Source code
│   ├── main.cpp           # Application entry point
│   ├── CMakeLists.txt     # Build configuration
│   ├── graph_structure/   # Graph implementation
│   ├── routing/          # Routing algorithms
│   ├── menu/             # User interface
│   ├── parse_data/       # Data management
│   └── graph_builder/    # Graph construction
├── data/                 # CSV data files
│   ├── Locations.csv     # Location database
│   ├── Distances.csv     # Distance matrix
│   └── Example*.csv      # Sample datasets
├── docs/                 # Documentation
│   ├── html/            # Doxygen HTML output
│   └── latex/           # Doxygen LaTeX output
└── README.md            # Project documentation
```

## ⚡ Performance & Complexity

### Algorithm Complexities

- **Dijkstra's Algorithm**: O(E log V) - Optimal shortest path finding
- **Environmentally-Friendly Routing**: O(P × E log V) - P parking locations
- **Graph Construction**: O(V + E) - Linear time graph building
- **Data Parsing**: O(N) - Linear CSV processing

### Memory Efficiency

- Template-based design for minimal memory overhead
- Efficient adjacency list representation
- Optimized priority queue implementation
- Smart pointer usage for automatic memory management

## 🎯 Key Features Implemented

- ✅ Complete graph-based routing system
- ✅ Dijkstra's shortest path algorithm
- ✅ Multi-modal transportation support
- ✅ Constraint-based route filtering
- ✅ Environmental route optimization
- ✅ Comprehensive data management
- ✅ Interactive command-line interface
- ✅ Robust error handling and validation
- ✅ Extensive documentation with Doxygen
- ✅ Cross-platform compatibility

## 🏆 Learning Outcomes

Through this project, we gained practical experience with:

- **Advanced Algorithms**: Implementation of graph algorithms and optimization techniques
- **Data Structures**: Custom graph structures and priority queue implementations
- **Software Engineering**: Modern C++ practices and design patterns
- **Performance Optimization**: Algorithm analysis and complexity optimization
- **Project Management**: Team collaboration and version control with Git
- **Documentation**: Professional API documentation with Doxygen

## 👥 Development Team

This project was developed by Group 2 - Class 15:

- Pedro Lunet
- [Pedro André Freitas Monteiro](https://github.com/pedroafmonteiro)

## 📜 Course Information

Developed for the Design of Algorithms (DA) course - Project 1, Spring 2025  
Faculty of Engineering, University of Porto (FEUP)

---

_Build and run the application to explore advanced path planning capabilities with real urban navigation data. The system demonstrates efficient algorithmic implementations suitable for real-world routing applications._
