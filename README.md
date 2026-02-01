# Conveyor Automation System

An industrial conveyor automation system developed in **Siemens TIA Portal** as a training project.
Each conveyor is controlled using a **Function Block**, which allows scalable and maintainable control logic.
The system uses sensor-based conditions to ensure safe material transfer and prevent collisions.

## System Overview
- The system enters a **ready state** when the *Start* button is pressed.
- Each conveyor section is equipped with sensors to detect object presence.
- Conveyor operation is determined by the status of adjacent conveyor sections.

## Control Logic
A conveyor is allowed to run if **any** of the following conditions are met:

- If the **previous conveyor sensor is triggered** and the **current conveyor is not occupied**,  
  the current conveyor runs until its own sensor detects the object.

- If the **current conveyor sensor is triggered** and the **next conveyor is not occupied**,  
  the current conveyor runs until the object is detected by the next conveyor’s sensor.

## Safety and Interlocking
- Conveyor start and stop actions are controlled through conditional logic.
- Interlocking between conveyor sections prevents object collisions and unsafe operation.
- Conveyors stop automatically once transfer conditions are satisfied.

## What I Learned
- Designing PLC logic using Function Blocks
- Designing sensor-based interlock logic
- Preventing collisions in multi-conveyor systems

## Possible Improvements
- Fault handling for sensor failures
- HMI-based conveyor status visualization
