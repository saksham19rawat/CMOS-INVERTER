# CMOS-INVERTER

A *CMOS inverter* is the most basic logic gate in digital electronics, made using **CMOS (Complementary Metal-Oxide-Semiconductor)** technology. It is used to implement the **NOT function — meaning it inverts the input signal**.

Before, I start with the CMOS inverter, I believe it is worth mentioning what an Inverter is. Inverter is something that inverts. In electronics it is very popularly explained as something that performs the NOT logic, that is complements the input. So a HIGH(1.8V) becomes LOW(0V) and vice versa. Ideally, the output follows the input and there is no delay or propogation issues of the circuit. But in reality, an inverter can be a real piece of work. It can have serveral isseus like how fast can it react to the changes in the input, how much load can it tolerate before it's output breaks and so many more including noise, bandwidth, etc.

# DESIGNING THE CIRCUIT
## Schematic File
![image alt](https://github.com/saksham19rawat/CMOS-INVERTER/blob/main/cmos/Screenshot%202025-05-25%20151432.png?raw=true)
## Symbol File
![image alt](https://github.com/saksham19rawat/CMOS-INVERTER/blob/main/cmos/Screenshot%202025-05-22%20233729.png?raw=true)
## Netlist
![image alt](https://github.com/saksham19rawat/CMOS-INVERTER/blob/main/cmos/Screenshot%202025-05-22%20171844.png?raw=true)
## Ngspice
![image alt](https://github.com/saksham19rawat/CMOS-INVERTER/blob/main/cmos/Screenshot%202025-05-22%20171853.png?raw=true)

DC analysis would be used to plot a Voltage Transfer Characteristics (VTC) curve for the circuit. It will sweep the value of Vin from high to low to determine the working of circuit with respect to different voltage levels in the input. The following plot is observed when simulated :
![image alt](https://github.com/saksham19rawat/CMOS-INVERTER/blob/main/cmos/Screenshot%202025-05-22%20171903.png?raw=true)


![image alt](https://user-images.githubusercontent.com/43693407/143764318-d0893545-f47c-44b8-a27c-8de8bc4f0759.jpg)



**The meeting point (also called threshold voltage) should be at a value of VDD/2 for maximum noise margins**

In the above image we can see the **Vth value** is **8.380288e-01**



![image alt](https://github.com/saksham19rawat/CMOS-INVERTER/blob/main/cmos/Screenshot%202025-05-22%20172256.png?raw=true)

![image alt](https://github.com/saksham19rawat/CMOS-INVERTER/blob/main/cmos/Screenshot%202025-05-22%20172359.png?raw=true)

After changing the Width of pmos to 2 we can see the value of Vth shifts towards the right

Now Vth is **8.6982931e-01**
