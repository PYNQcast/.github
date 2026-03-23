# PYNQcast

A multiplayer raycasting game engine built on PYNQ-Z1 FPGA boards with a cloud-hosted AWS game server.
Players connect over UDP, with the FPGA handling real-time rendering via a hardware DDA raycasting engine
and the ARM Cortex-A9 managing game logic and networking.

---

## Repositories

| Repo | Description |
|------|-------------|
| [ClientSide_PYNQ_jupyter](https://github.com/PYNQcast/ClientSide_PYNQ_jupyter) | Bitstream, HWH file, and Python game script: everything needed to run PYNQcast on a PYNQ-Z1 out of the box (Server should be running, *.pem will be provided if needed)|
| [HardwareSide_PYNQ_Raycaster](https://github.com/PYNQcast/HardwareSide_PYNQ_Raycaster) | Full Vivado project and SystemVerilog source for the DDA raycasting engine |
| [ServerSide_PYNQ_Raycaster](https://github.com/PYNQcast/ServerSide_PYNQ_Raycaster) | AWS-hosted game server handling player registration, match state, and UDP tick protocol |
| [Deliverables](https://github.com/PYNQcast/deliverables) | Includes custom diagrams, manim (python) videos and other key documents we used along the way for our project |

---

## Getting Started

To play, only **ClientSide_PYNQ_jupyter** is required. Clone it onto your PYNQ-Z1 board and follow
the instructions in its README. The hardware and server repos are provided for reference and reproducibility.

---

## Built With

- PYNQ-Z1 (Zynq-7020 SoC)
- SystemVerilog / Vivado
- Python / PYNQ framework
- AWS (EC2, Redis, DynamoDB, S3)

---

## Demo

[Watch the demo video](https://youtube.com/your-video)

--<img width="3053" height="2228" alt="Main_architecture" src="https://github.com/user-attachments/assets/de1d4e53-3b09-4547-8572-446aa6dc2ea6" />


