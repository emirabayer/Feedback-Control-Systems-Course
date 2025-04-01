# Feedback-Control-Systems-Course
This repository consists of the lab and project reports that include the MATLAB code and simulation/hardware implementation results for the Introduction to Feedback Control Systems course at Bilkent.

***course link:*** https://catalog.bilkent.edu.tr/course/c14342.html

<br>


<br>

## Lab 1 - DC Motor System Identification & PI Controller Design: From First-Order Approximation to Hardware Implementation
This lab involved modeling a DC motor’s velocity response using a first-order transfer function approximation, validated through Simulink simulations and hardware experiments. After filtering noisy raw data with a low-pass filter (LPF), I derived the system’s gain (𝐾 = 13.75) and time constant (𝜏 = 0.131) via MATLAB analysis, achieving a transfer function of 𝑌(𝑠) = 13.75/(0.131𝑠 + 1). I then designed three PI controllers, tuning coefficients (𝐾ₚ, 𝐾ᵢ) to meet strict criteria (0% steady-state error, <8% overshoot, <0.8s settling time), and implemented the optimal controller on hardware. The final design achieved 0% overshoot and 0.41s settling time, with minor hardware-simulation discrepancies due to noise. This project demonstrated my proficiency in system identification, control theory, and embedded systems integration, combining MATLAB/Simulink modeling with real-world validation.
<br>
<br>

## Lab 2: - Frequency Domain Analysis of DC Motor: Bode Plot Generation, Experimental Validation & Time Delay Compensation
This lab focused on frequency-domain system identification of a DC motor, beginning with generating theoretical Bode plots from the transfer function found in lab 1 using MATLAB, while deliberately avoiding the built-in bode function to demonstrate manual computation skills. By applying sinusoidal inputs at varying frequencies (0.1–100 rad/s) to the physical motor, I captured experimental data, processed it via FFT to extract magnitude and phase responses, and overlaid these results (marked as 'x') onto the theoretical Bode plot for validation. To address hardware-induced phase discrepancies, I incorporated a first-order Padé approximation to model a 10 ms processing delay, refining the transfer function. This project showcased my ability to bridge theoretical modeling (Laplace domain analysis) with practical hardware experimentation, while employing advanced MATLAB scripting (FFT, semilogx) and control theory concepts (Padé approximation, frequency response) to achieve accurate system identification.
<br>
<br>
