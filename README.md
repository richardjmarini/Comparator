# Comparator
Discrete Comparator

![schematic_screenshot](MainBoard/images/schematic.png)
![variable_input screenshot](MainBoard/images/variable_input.png)
![variable_input_inverted_output screenshot](MainBoard/images/variable_input_inverted_output.png)
![constant_input screenshot](MainBoard/images/constant_input.png)
![constant_input_inverted_output screenshot](MainBoard/images/constant_input_inverted_output.png)

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


