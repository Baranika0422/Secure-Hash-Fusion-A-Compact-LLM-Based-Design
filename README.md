# Secure-Hash-Fusion-A-Compact-LLM-Based-Design
This project implements the RTL design and verification of the SHA-1 hash algorithm in SystemVerilog using OSS CAD tools, validated through testbench simulation and a Python reference model, with an extensible interface supporting both SHA-1 and SHA-256 for cryptographic hardware verification.

****Project Files****

sha1_padding.sv – Message padding and length encoding module

tb_sha1_padding.sv - Testbench with standard test vectors (“abc”, “a”) for padding(512 bits)

sha_design.sv – SHA-1 compression and round logic

sha1_top.sv - Top-level FSM coordinating padding and hashing

tb_sha1_top.sv – Testbench with standard test vectors (“abc”, “a”) for sha1_hash

sha_design.py - SHA1 design implementation using python for verification.

parameterised_sha_design - Parameterized SHA-1 / SHA-256 engine



****Tools & Environment****

HDL & Verification: SystemVerilog, Verilog HDL

Simulation: Icarus Verilog, GTKWave

Synthesis: Yosys (OSS CAD Suite)

Reference Modeling: Python (SHA-1 implementation)

Verification Sources: Python model, online SHA compilers

AI Assistance: LLMs (ChatGPT, Gemini, Claude)

Target Platform: Cryptographic hardware / FPGA-oriented RTL design

****Key Achievements****

Designed and implemented RTL architecture of SHA-1 using SystemVerilog

Developed a complete testbench for functional verification

Verified RTL output against Python reference model and online SHA tools

Implemented message padding, expansion, and 80-round compression logic

Achieved correct 160-bit hash output for standard test vectors

Extended design to a parameterized SHA-1 / SHA-256 dual-mode engine

Used LLM assistance to optimize and generalize cryptographic RTL code

Achieved efficient timing: ~1.52 µs (SHA-1) and 1.2 µs (SHA-256) per hash

****Future Work****
Deploy and validate design on real FPGA hardware

Optimize power, area, and timing for ASIC-level implementation

Add support for additional SHA family algorithms (SHA-512, SHA-3)

Enhance security with side-channel attack resistance techniques

Automate verification using formal verification methods
