# Comparator
Discrete Comparator

## Runtime & Build
  - **Ubuntu/Debian**:
    ```bash
    sudo apt install ngspice kicad
    ```
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

## Schematic
![schematic_screenshot](MainBoard/images/schematic.png)

## Simulation(s)
### Alternating Signal via Inverting Input
![variable_input screenshot](MainBoard/images/variable_input.png)
![variable_input_inverted_output screenshot](MainBoard/images/variable_input_inverted_output.png)
### Constant Signal via Inverting Input
![constant_input screenshot](MainBoard/images/constant_input.png)
![constant_input_inverted_output screenshot](MainBoard/images/constant_input_inverted_output.png)
