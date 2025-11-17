# RISC-V-PROCESSOR-DESIGN

A fully modular RISC-V processor designed from scratch using Verilog/SystemVerilog.  
Includes ALU, Register File, Control Unit, Decoder, Immediate Generator, Branch Logic, PC, Memory Interfaces, and complete verification testbenches.  
Designed for academic learning, research, and RISC-V architecture exploration.

---

## 📸 CPU Architecture – Image Upload
(<img width="1506" height="399" alt="Screenshot 2025-11-15 125034" src="https://github.com/user-attachments/assets/d9f35667-e4af-4d83-bef4-41241771ba22" />
)


---

## 📸 Waveforms / Simulation Outputs
(<img width="1308" height="684" alt="Screenshot 2025-11-15 124818" src="https://github.com/user-attachments/assets/6c521b52-6da7-4e6f-a3f7-81766164e423" />
)

---

# 📘 RISC-V Architecture Overview

RISC-V is an open-source **Reduced Instruction Set Computer (RISC)** architecture designed for simplicity, modularity, and extensibility.  
It is widely adopted in industry and academia for CPUs, microcontrollers, accelerators, and AI hardware.

Your processor implements the **RV32I** base instruction set.

---

# ⚔️ RISC vs CISC (Complete Comparison)

| Feature | RISC (Used in RISC-V) | CISC (x86, 8051, etc.) |
|--------|-------------------------|--------------------------|
| **Instruction Count** | Small, simple | Large, complex |
| **Instruction Size** | Fixed (32 bits) | Variable (1–15 bytes) |
| **Execution Cycle** | Mostly single-cycle | Multi-cycle |
| **Hardware Complexity** | Low | High |
| **Pipelining** | Easy, efficient | Hard due to variable length |
| **Power Consumption** | Low | High |
| **Performance Scaling** | Very good | Limited |
| **Decoding Logic** | Simple | Complex |
| **Microcode** | Not required | Required |

### ✔ Why RISC is Better?
- Faster execution  
- Better optimization  
- Lower energy usage  
- Easier for verification  
- Highly suitable for SoC and embedded systems  

---

# ⭐ Advantages of RISC Architecture

- Simple instruction set  
- Faster instruction execution  
- Ease of pipelining  
- Low power and heat generation  
- Predictable timing  
- Lower hardware complexity  
- Higher clock frequency possible  
- Smaller silicon area → cheaper chips  

---

# 🚀 Advantages of **RISC-V**

- Completely **open-source ISA**  
- Royalty-free → anyone can design CPUs  
- Highly modular (RV32/64/128, M, A, F, D extensions)  
- Perfect for custom instructions & accelerators  
- Industry adoption (NVIDIA, Tesla, Google, Qualcomm, India’s SHAKTI, etc.)  
- Great for research and CPU design learning  
- Large open-source ecosystem (Spike, QEMU, LLVM, GNU Toolchain)

---

# 🔧 Supported Instruction Types in This CPU

### **✔ R-Type**
ADD, SUB, AND, OR, XOR, SLT, SLL, SRL, etc.

### **✔ I-Type**
ADDI, ANDI, ORI, XORI, LW, JALR, etc.

### **✔ S-Type**
SW

### **✔ B-Type**
BEQ, BNE, BLT, BGE

### **✔ U-Type**
LUI, AUIPC

### **✔ J-Type**
JAL

---

# 🧠 Pipeline Overview (Simple Explanation)

Although your current CPU is **single-cycle**, the design is pipeline-ready.

### Standard 5-step RISC Pipeline:

1. **IF – Instruction Fetch**  
   PC fetches instruction from memory.

2. **ID – Instruction Decode**  
   Decode the instruction, read registers.

3. **EX – Execute**  
   ALU computes address or result.

4. **MEM – Memory Access**  
   Load/store operations.

5. **WB – Write Back**  
   Result written back to register file.

---

## ❗ Pipeline Hazards (For Future Work)

### ⭐ Data Hazards  
RAW, WAR, WAW  
Solution: Forwarding, Stall

### ⭐ Control Hazards  
Due to branches  
Solution: Branch prediction, early resolution

### ⭐ Structural Hazards  
When hardware units conflict  
Solution: Separate instruction and data memory

---

# 🧪 Verification & Simulation

Testbenches included for:
- ALU  
- Register File  
- Decoder  
- Control Unit  
- PC  
- Memories  
- Full top-level processor  

Add waveform images here later.


---

# 🌍 Applications of RISC-V

- Microcontrollers (IoT, Embedded)
- Academic CPU design projects
- ASIC / FPGA implementations
- AI & ML accelerators
- GPU integration
- Robotics
- Automotive ECUs
- Smart consumer devices
- Space & defense applications
- Custom hardware research

---

# 🔮 Future Enhancements

- Full 5-stage pipeline  
- Hazard detection unit  
- Forwarding unit  
- Branch predictor  
- Multipliers (M extension)  
- CSR (Control & Status Registers)  
- Interrupt + exception support  
- Cache design  
- AXI/AHB interface  

---

# 📚 Tools Used

- **Verilog/SystemVerilog**
- **Vivado / Questa / Xcelium**
- **GTKWave / SimVision**
- **RISC-V GNU Toolchain**
- **FPGA (optional)**

---

# 👨‍💻 Contributors
- **Rohan N D**

---

# 📄 License
This project is open-source under the **MIT License**.

---


