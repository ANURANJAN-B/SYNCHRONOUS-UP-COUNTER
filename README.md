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

Developed by: ANURANJAN.B
RegisterNumber:25003110


**RTL LOGIC UP COUNTER**

<img width="1918" height="1069" alt="498418498-c304f5a8-a4c1-43a0-8fcc-12fd22b69165" src="https://github.com/user-attachments/assets/43d9de92-8aaa-4afe-b040-481ab1bf1a52" />

**TIMING DIAGRAM FOR IP COUNTER**

<img width="1919" height="1079" alt="498418452-cd1e7e6e-7df7-49c2-bdfa-5883bcddbd71" src="https://github.com/user-attachments/assets/18aaf523-262d-4342-900b-4bda64af84ca" />

**TRUTH TABLE**

<img width="544" height="275" alt="498418372-9b2bcbbb-615d-4512-9758-64fc6193b63f" src="https://github.com/user-attachments/assets/888f465f-7017-42d1-b38f-dd3cbc3c68e3" />

**RESULTS**
Thus the Synchronous 3 bit Up counter is implemeted and verified.
