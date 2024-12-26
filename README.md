**NAME:HARISH S**

**REG NO:24901078**

**EXP NO 11 SYNCHRONOUS-UP-COUNTER**


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

**PROCEDURE**

/* write all the steps invloved */

**PROGRAM**

![image](https://github.com/user-attachments/assets/50b925dd-bf17-45e8-aa12-6f361ee7b969)



**RTL LOGIC UP COUNTER**
![image](https://github.com/user-attachments/assets/80e9ebf5-ce45-47e3-aa92-be7fa9419a58)



**TIMING DIAGRAM FOR IP COUNTER**

![image](https://github.com/user-attachments/assets/2d72ec4b-9713-4ef6-8553-2e9ddf65d80d)


**TRUTH TABLE**

![image](https://github.com/user-attachments/assets/83c6d108-9b8c-4164-9f3a-a90b18244f0f)


**RESULTS**
Thus to implement 4 bit synchronous up counter and validate functionality done successfully.
