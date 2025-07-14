# Analog IC Design

# **Chapter 01**

### **1.1 Why Analog?**

• **Many experts in the 1980s thought analog circuits would disappear** because digital circuits were becoming very powerful. <br>
• But analog circuits are still **very important** today. <br>
• Some signals from nature (like sound, light, or movement) are **analog**.   <br>
• To process these signals, we first use analog circuits, then convert the signal to digital.   <br>
• Examples where analog is needed:  <br>
    &nbsp;&nbsp;&nbsp;◦ Natural signals (microphone sound, camera sensors)  <br>
    &nbsp;&nbsp;&nbsp;◦ Communication signals traveling long cables or wireless   <br>
    &nbsp;&nbsp;&nbsp;◦ Sensors (accelerometers in cars to trigger airbags)  <br>
• Analog circuits help amplify, filter, and convert signals for digital use.  <br>

### **1.2 Applications of Analog Circuits**

• Natural signals are analog and very weak, so analog circuits **amplify and filter** these signals before digital processing.  <br>
• Digital communication signals lose quality over long cables and need analog circuits to **restore and clean** the signal.  <br>
• Wireless receivers handle very weak, noisy signals using analog circuits that work at high frequencies.  <br>
• Optical communication uses light signals, but at the receiver, analog circuits process very fast, low-level electrical signals.  <br>
• Sensors (mechanical, electrical, optical) convert physical things to electrical signals. Analog circuits amplify and measure these small signals precisely.  <br>
• Example: accelerometers in cars measure tiny changes in capacitance to detect accidents. 

### **1.3 Why CMOS?**

• CMOS technology uses **n-type and p-type MOSFETs together**, invented in the 1960s.  <br> 
• CMOS is popular because:
     &nbsp;&nbsp;&nbsp;◦ Uses very little power (only when switching) <br>
     &nbsp;&nbsp;&nbsp;◦ Easy to make small transistors (scaling) <br>
     &nbsp;&nbsp;&nbsp;◦ Cheaper fabrication costs  <br>
• Initially, CMOS was mainly for digital circuits, because MOSFETs were slower and noisier than bipolar transistors.  <br>
• But scaling (making transistors smaller) made CMOS faster and better.  <br>
• Today, CMOS is used for **high-speed analog circuits** too, competing with bipolar devices.  <br>

### **1.4 Why This Book?**

• Analog circuit design has changed as devices get smaller and voltages get lower.  <br>
• Analog and digital circuits are now made on the same chip.  <br>
• This creates new design challenges.  <br>
• Good analog designers need:
   &nbsp;&nbsp;&nbsp;  ◦ **Engineer’s skills**: to understand the whole circuit quickly <br>
   &nbsp;&nbsp;&nbsp;  ◦ **Mathematician’s skills**: to analyze subtle effects with math <br>
   &nbsp;&nbsp;&nbsp;  ◦ **Artist’s skills**: to invent new circuit designs  <br>
• This book teaches analog design with both simple understanding and detailed analysis.  <br>
• It guides you through how circuits have evolved and the thought process behind new designs.  <br>

### **1.5 General Concepts**

**1.5.1 Levels of Abstraction**
• We study circuits at different levels:
   &nbsp;&nbsp;&nbsp;  ◦ **Device physics level**: How electrons move inside a transistor <br>
   &nbsp;&nbsp;&nbsp;  ◦ **Transistor level**: Electrical behavior of transistors <br>
   &nbsp;&nbsp;&nbsp;  ◦ **Architecture level**: How groups of devices form blocks (like amplifiers) <br>
    &nbsp;&nbsp;&nbsp; ◦ **System level**: How blocks work together as a whole system   <br> 
• Designers switch between these levels to understand details and improve performance.  <br>
• In the industry, people working at all levels must communicate to make good chips.

**1.5.2 Robust Analog Design**
• Real circuits must work well even when conditions change:
    &nbsp;&nbsp;&nbsp; ◦ Manufacturing differences (Process)<br>
    &nbsp;&nbsp;&nbsp; ◦ Supply voltage changes (Voltage)<br>
    &nbsp;&nbsp;&nbsp; ◦ Temperature changes (Temperature)  <br>
• These changes are called **PVT variations**.
• Robust design means the circuit works correctly within a range of PVT changes.  <br>
• CMOS devices vary a lot from chip to chip, so designing robust analog circuits is difficult.  <br>
• Designers use simulation and special techniques to handle these variations.  <br>
