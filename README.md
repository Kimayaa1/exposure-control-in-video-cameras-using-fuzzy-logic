# exposure-control-in-video-cameras-using-fuzzy-logic
The primary objective is to investigate the effectiveness of fuzzy logic in optimizing exposure parameters such as aperture, shutter speed, and ISO sensitivity. Fuzzy logic provides a flexible and adaptive approach to exposure control by incorporating human-like reasoning based on imprecise and uncertain information.

The fuzzy logic system is defined using the skfuzzy library in Python. The program defines three fuzzy variables: ambient_light, scene_contrast, and exposure_adjustment. The membership functions for each variable are defined using triangular membership functions. Fuzzy rules are then defined based on the input variables and desired exposure adjustments.
The program creates a fuzzy control system using the defined rules and simulates it using the provided input values for ambient_light and scene_contrast. The computed fuzzy output is then defuzzified to obtain a crisp value representing the recommended exposure adjustment.
we use the `skfuzzy` library to implement a fuzzy logic system for exposure adjustment based on ambient light and scene contrast. 
We define three fuzzy variables: `ambient_light`, `scene_contrast`, and `exposure_adjustment`. Each variable has a set of linguistic terms with corresponding membership functions defined using `fuzz.trimf()`. 

Next, we define fuzzy rules using `ctrl.Rule()`. The rules specify the combinations of input fuzzy sets and the corresponding output fuzzy sets. 

We create a fuzzy control system using `ctrl.ControlSystem()` and pass the defined rules as an argument. 

A control system simulation is created using `ctrl.ControlSystemSimulation()`.

We then set the input values for `ambient_light` and `scene_contrast` using `exposure_simulation.input[]`. 

Using `exposure_simulation.compute()`, the fuzzy control system computes the output based on the input values and the defined rules. 

Finally, we retrieve the crisp output value for `exposure_adjustment` using `exposure_simulation.output[]` and print it.

with an ambient light value of 70 and a scene contrast value of 30, the fuzzy control system determines an exposure adjustment value of 0.5.

