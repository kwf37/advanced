### Analog HW 2

## Files
* Audio_model- Provided by Molnar
* sys_model- Provided by Molnar
* hw2_characterize- Instanced the Audio and Sys models with vsins and isins for characterizing input impedances and transfer functions
* hw2_diff_amp- Inverter-style differential amplifier- has about 90dB of gain, rolloff ~20kHz, but unstable ~100MHz
* hw2_diff_amp_test- Test bench for differential amplifier
* unit_inverter- A Unit inverter designed to operate at midrail with Vdd ~1.4V. Missing subc
* unit_inv_test- A test bench for the unit inverter. Set up to do DC sweep and Frequency Response. DC Sweep is good for figuring out biasing, and Frequency response shows the gain and bandwidth. May want to add tests for input/output impedance.

## Brainstorming Ideas
* Linear-Regulator vs. Caps- Should we save on power/area and design everything around bad supply?
* The transfer function from Speaker to Audio out starts with a zero, levels out, then has a pole. We will probably want a R C C feedback network (maybe like HW 1 config inverted) to account for this and get a steady dB out
