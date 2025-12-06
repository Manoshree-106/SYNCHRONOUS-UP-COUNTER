### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

/* write all the steps invloved */

**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 
<img width="787" height="571" alt="Screenshot 2025-12-06 174849" src="https://github.com/user-attachments/assets/305c9136-5334-4754-b9d1-a00f0730d36a" />


Developed by:Manoshree N RegisterNumber:25017532
*/

**RTL LOGIC UP COUNTER**
<img width="1810" height="855" alt="Screenshot 2025-12-06 174523" src="https://github.com/user-attachments/assets/922b9687-1687-464d-a1f1-d061e4cf9a33" />


**TIMING DIAGRAM FOR IP COUNTER**
<img width="1896" height="471" alt="Screenshot 2025-12-06 174743" src="https://github.com/user-attachments/assets/bda6b2e0-5c60-405f-8290-fa2a246193af" />


**TRUTH TABLE**

**RESULTS**
Thus, implement 4 bit synchronous up counter and validate functionality.

