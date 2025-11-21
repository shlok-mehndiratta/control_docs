# Control Law Formulation

## Objective
Convert visual error (deviation from path center) into steering commands for the UGV.

## Concept
The UAV provides:
- UGV position  
- Road centerline  

The controller computes:
\[
\text{steering\_angle} = k_p \cdot e + k_d \cdot \dot{e}
\]
where:
- \(e\) = lateral error  
- \(\dot{e}\) = rate of change of error  

## Current Status
- Basic proportional controller under consideration.
- Awaiting refined vision outputs for testing.

## Next Steps
- Conduct closed-loop trials inside the simulation.
- Tune control gains.

