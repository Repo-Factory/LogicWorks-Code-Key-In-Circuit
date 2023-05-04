# Contributors

Conner Sommerfield - User-Programmable Model-Documentation-State Diagram PDF, Circuit Documentation
Ryan Jaber - Factory Preset Model-Documentation-ReadMe

# Files
Factory Preset Model: key that was used: 11101000



1. Gotcha Component With interface.cct:
The unlock code is 11101000. After 16 button presses, the lock will activate and the circuit will force stop causing the system to stop working until the reset button is clicked.

2. Lab 3 Part Underlying Circuit.cct:
You can press the top or bottom button to enter a 1 or 0. releasing any button will cause the clock of all the flip flops to trigger. Press out the factory preset key and when the lock is not triggered, the outputs are displayed as 1s till locked. The entercode will have a high if it is unlocked and the correct key, but will have a low thus shutting off. The function is to incorporate the necessary circuits to create an incrementer, inputs, lock to work together.

3. Lab 3 With Documentation After Lock Changes:
Meant to show how the circuit develops after the locking mechanism is initiated by the 16th press, and any presses after will cause the binary probe for the lock to show a 0 which is locked till reset is pressed.

4. Present State PDF:
This file contains the equations,state diagram, and truth tables that went along with the 11101000 keycode.

5. Readme
For details.

#Design Process
To obtain the circuits we needed to make sure we could incorporate the reset, incrementor, hex boards (2), entercode storage, etc. to minimize hardware use. We chose 3 flip flops based on the three equations we found which can be found in the "Present State" Pdf. We focused on 3 binary probes because when the sequence is pressed, the 4th flip flop will output 1 to show correctness and lock has not been activated.It will output a 0 for when there  are 16 button presses. We attached the incrementer clock to input hex displays to track the amount of pushed buttons since the last reset. We need the hex keyboard to store the current keyed in data for which 11101000 is given as 1 7 on the hex pad. We needed to use the XNOR gates in our part II because it will check all the bits the user is matching to output a 1 but 0 if not matching. The key goal for the circuit design was to minimize the hardware use by maximizing the amount of data we could use efficiently. Using the clock pulses, binary probes, and inverters, we were able to make a logical circuit for developing a Gottcha Anti-Theft Machine.
