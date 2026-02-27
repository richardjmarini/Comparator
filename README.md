# Comparator
Discrete Comparator

![schematic_screenshot](MainBoard/images/schematic.png)
![spice_screenshot](MainBoard/images/variable_inverting_input_simulation.png)
![spice_screenshot](MainBoard/images/fixed_inverting_input_simulation.png)

## 🛠  Dependencies

This project requires the following dependencies:

### 🧱 Runtime & Build

  - **Ubuntu/Debian**:
    ```bash
    sudo apt install ngspice kicad
    ```

## Example
  - **Generate the Netlist**:
```
kicad-cli sch export netlist \
    --format spice \
    -o MainBoard/MainBoard.cir \
    MainBoard/MainBoard.kicad_sch
```
  - **Run the Simulation**:
```
ngspice MainBoard/MainBoard.cir
```


