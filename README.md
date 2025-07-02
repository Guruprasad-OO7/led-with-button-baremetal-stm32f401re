 🔩 STM32F401RE Bare-Metal LED Toggle Using Onboard Button

This project demonstrates how to control the onboard LED (PA5) using the onboard push button (PC13) on the STM32 Nucleo-F401RE development board. The code is written in pure bare-metal C, without using STM32 HAL or any abstraction libraries — just direct register access!

🎯 Project Objective:-
🔘 Press the user button (PC13)  
💡 Toggle the onboard LED (PA5)  
➡️ Achieved entirely via register-level programming

🛠️ Tools & Requirements:-
- Development Board: STM32 Nucleo-F401RE  
- Toolchain: Keil uVision / STM32CubeIDE / STM32CubeProgrammer  
- Language: C (Bare-Metal)  
- CMSIS: Only for basic startup files (optional)

📐 Pin Configuration

 Onboard LED     PA5     
 Onboard Button  PC13     

 🧠 Key Concepts:-
- RCC Clock Enable via `RCC->AHB1ENR`
- GPIO Mode Config via `MODER`
- Internal Pull-up Config via `PUPDR`
- Button Read via `IDR`
- LED Write via `ODR`
- Crude software delay
- Bit masking and shifting
