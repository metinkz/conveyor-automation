# conveyor-automation
Automation of standard industrial conveyors made in TIA Portal.

System can be set to ready state by pressing "start" button for working condition.
Conditions are checked via sensors placed in every conveyor.

Conveyors run if any of the conditions are met below;
- If previous sensor is triggered and current conveyor is not occupied, current conveyor runs until sensor on the current conveyor is triggered by the object.
- If current sensor is triggered and next conveyor is not occupied, current conveyor runs until sensor on the next conveyor is triggered by the object.

Execution and stopping of the conveyors are controlled via given conditions to prevent collision and accident.
