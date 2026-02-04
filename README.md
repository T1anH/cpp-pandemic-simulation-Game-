# C++ Pandemic Simulation

A C++ simulation engine that models disease transmission, recovery, and agent behavior in a shared environment. The system simulates interactions between multiple entity types over discrete time steps, allowing observation of infection spread dynamics and system behavior under different conditions.

This project emphasizes object-oriented design, system architecture, and simulation logic rather than graphics or gameplay.

---

## Overview

The simulation represents a virtual world populated by multiple interacting entities, including people, viruses, and environments. Each entity follows defined behaviors and state transitions, such as movement, infection, recovery, and interaction with other entities.

The simulation advances in discrete time steps, updating entity states, resolving interactions, and dynamically creating or removing entities as the system evolves.

---

## Key Features

- Agent-based pandemic simulation
- Time-stepped simulation loop
- Multiple interacting entity types
- Dynamic entity creation and removal
- Proximity-based infection transmission
- State machines for agent behavior
- Command-driven runtime control

---

## Architecture & Design

### Object-Oriented Design
- Polymorphic entity hierarchy using inheritance and virtual functions
- Base `GameObject` class extended by specialized entities
- Behavior defined through overridden update methods

### System Architecture
- Central world state managing all entities
- Discrete simulation tick loop
- Separation of concerns between simulation logic, input handling, and rendering
- Model–View–Command architecture for maintainability

---

## Entity Types

- **Students / Agents** – Move through the environment and interact with others
- **Virus Entities** – Model infection and transmission logic
- **Buildings / Locations** – Define spatial interaction boundaries
- **World Controller** – Manages global state and simulation flow

---

## Command Interface

The simulation supports a command-driven interface that allows:
- Runtime control of agent movement
- Triggering state transitions
- Spawning or removing entities
- Adjusting simulation behavior without recompilation

This design enables flexible experimentation and debugging.

---

## Tech Stack

- C++
- Object-Oriented Programming
- State Machines
- Discrete-Time Simulation
- Command Pattern

---

## Key Takeaways

This project demonstrates:
- Strong C++ fundamentals
- Clean object-oriented system design
- Simulation engine architecture
- Managing complex interactions in a shared world state
- Designing extensible systems without excessive conditional logic
