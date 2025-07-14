# Analog IC Design

# **Chapter 01**

### **1.1 Why Analog?**

• **Many experts in the 1980s thought analog circuits would disappear** because digital circuits were becoming very powerful.
• But analog circuits are still **very important** today.
• Some signals from nature (like sound, light, or movement) are **analog**.
• To process these signals, we first use analog circuits, then convert the signal to digital.
• Examples where analog is needed:
    ◦ Natural signals (microphone sound, camera sensors)
    ◦ Communication signals traveling long cables or wireless
    ◦ Sensors (accelerometers in cars to trigger airbags)
• Analog circuits help amplify, filter, and convert signals for digital use.

### **1.2 Applications of Analog Circuits**

• Natural signals are analog and very weak, so analog circuits **amplify and filter** these signals before digital processing.
• Digital communication signals lose quality over long cables and need analog circuits to **restore and clean** the signal.
• Wireless receivers handle very weak, noisy signals using analog circuits that work at high frequencies.
• Optical communication uses light signals, but at the receiver, analog circuits process very fast, low-level electrical signals.
• Sensors (mechanical, electrical, optical) convert physical things to electrical signals. Analog circuits amplify and measure these small signals precisely.
• Example: accelerometers in cars measure tiny changes in capacitance to detect accidents.

### **1.3 Why CMOS?**

• CMOS technology uses **n-type and p-type MOSFETs together**, invented in the 1960s.
• CMOS is popular because:
    ◦ Uses very little power (only when switching)
    ◦ Easy to make small transistors (scaling)
    ◦ Cheaper fabrication costs
• Initially, CMOS was mainly for digital circuits, because MOSFETs were slower and noisier than bipolar transistors.
• But scaling (making transistors smaller) made CMOS faster and better.
• Today, CMOS is used for **high-speed analog circuits** too, competing with bipolar devices.

### **1.4 Why This Book?**

• Analog circuit design has changed as devices get smaller and voltages get lower.
• Analog and digital circuits are now made on the same chip.
• This creates new design challenges.
• Good analog designers need:
    ◦ **Engineer’s skills**: to understand the whole circuit quickly
    ◦ **Mathematician’s skills**: to analyze subtle effects with math
    ◦ **Artist’s skills**: to invent new circuit designs
• This book teaches analog design with both simple understanding and detailed analysis.
• It guides you through how circuits have evolved and the thought process behind new designs.

### **1.5 General Concepts**

**1.5.1 Levels of Abstraction**
• We study circuits at different levels:
    ◦ **Device physics level**: How electrons move inside a transistor
    ◦ **Transistor level**: Electrical behavior of transistors
    ◦ **Architecture level**: How groups of devices form blocks (like amplifiers)
    ◦ **System level**: How blocks work together as a whole system
• Designers switch between these levels to understand details and improve performance.
• In the industry, people working at all levels must communicate to make good chips.

**1.5.2 Robust Analog Design**
• Real circuits must work well even when conditions change:
    ◦ Manufacturing differences (Process)
    ◦ Supply voltage changes (Voltage)
    ◦ Temperature changes (Temperature)
• These changes are called **PVT variations**.
• Robust design means the circuit works correctly within a range of PVT changes.
• CMOS devices vary a lot from chip to chip, so designing robust analog circuits is difficult.
• Designers use simulation and special techniques to handle these variations.
