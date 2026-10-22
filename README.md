<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Inter&weight=600&size=26&duration=3200&pause=1100&color=24292F&center=true&vCenter=true&width=760&height=60&lines=Hi%2C+I%27m+Kartikey+Tiwari;Building+real-time+systems+from+silicon+to+sensors;Embedded+systems%2C+edge+AI+and+RF;Latency+matters.+So+does+getting+it+right." alt="Typing banner" />

<p>
  <a href="https://kartikeybuilds.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-24292F?style=flat-square&logo=vercel&logoColor=white" alt="Portfolio" /></a>
  <a href="https://www.linkedin.com/in/kartikey-tiwari-319047342/"><img src="https://img.shields.io/badge/LinkedIn-24292F?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://www.hackster.io/kartikey-tiwari"><img src="https://img.shields.io/badge/Hackster.io-24292F?style=flat-square&logo=hackster&logoColor=white" alt="Hackster.io" /></a>
  <a href="mailto:kartikey120207@gmail.com"><img src="https://img.shields.io/badge/Email-24292F?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

</div>

---

## About

I'm a B.Tech Electronics and Communication student at **NIT Goa**, and I build embedded and edge systems that have to be fast, reliable and measurable. My work runs from PCB design and RTL to real-time C++ and on-device vision, with a habit of validating every model against hardware.

Most recently I interned at QuickPay, where I built a YOLO and DeepStream pipeline on a Jetson Orin Nano running at 30+ FPS and stress-tested autonomous drone platforms. I like problems where the numbers decide whether the design is good.

---

## How I think about systems

```mermaid
flowchart LR
    A["Sense<br/>mmWave, PIR, IMU, camera"] --> B["Process<br/>EKF, YOLO, DSP"]
    B --> C["Communicate<br/>ZeroMQ, LoRa, 2.4 GHz"]
    C --> D["Act<br/>alerts, flight control, audio"]
    E["Hardware and RTL<br/>KiCAD, SystemVerilog, FPGA"] -.-> A
    E -.-> B
    F["Verification<br/>Verilator, cocotb, field tests"] -.-> B
    F -.-> C
```

Every stage gets a hardware layer underneath it and a verification layer on top of it. If I can't measure it, I don't trust it.

---

## Tech stack

**Languages**

![C](https://img.shields.io/badge/C-24292F?style=flat-square&logo=c&logoColor=white)
![C++20](https://img.shields.io/badge/C%2B%2B20-24292F?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-24292F?style=flat-square&logo=python&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-24292F?style=flat-square&logo=mathworks&logoColor=white)
![SystemVerilog](https://img.shields.io/badge/Verilog%20%2F%20SystemVerilog-24292F?style=flat-square)

**Hardware and platforms**

![ESP32](https://img.shields.io/badge/ESP32-24292F?style=flat-square&logo=espressif&logoColor=white)
![NVIDIA Jetson](https://img.shields.io/badge/Jetson%20Orin%20Nano-24292F?style=flat-square&logo=nvidia&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-24292F?style=flat-square&logo=raspberrypi&logoColor=white)
![Arduino](https://img.shields.io/badge/ATmega328P-24292F?style=flat-square&logo=arduino&logoColor=white)
![FPGA](https://img.shields.io/badge/FPGA%20(Gowin)-24292F?style=flat-square)
![RF](https://img.shields.io/badge/RF%20and%20LoRa-24292F?style=flat-square)

**Firmware and systems**

![ZeroMQ](https://img.shields.io/badge/ZeroMQ-24292F?style=flat-square&logo=zeromq&logoColor=white)
![UART SPI I2C](https://img.shields.io/badge/UART%20%7C%20SPI%20%7C%20I2C-24292F?style=flat-square)
![DMA](https://img.shields.io/badge/DMA%20and%20Interrupts-24292F?style=flat-square)
![GStreamer](https://img.shields.io/badge/GStreamer-24292F?style=flat-square&logo=gstreamer&logoColor=white)

**AI, DSP and verification**

![PyTorch](https://img.shields.io/badge/PyTorch-24292F?style=flat-square&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-24292F?style=flat-square&logo=opencv&logoColor=white)
![YOLO](https://img.shields.io/badge/YOLO%20%2B%20DeepStream-24292F?style=flat-square)
![Eigen3](https://img.shields.io/badge/Eigen3%20%2F%20EKF-24292F?style=flat-square)
![Verilator](https://img.shields.io/badge/Verilator%20%2B%20cocotb-24292F?style=flat-square)

**Tools**

![KiCad](https://img.shields.io/badge/KiCad-24292F?style=flat-square&logo=kicad&logoColor=white)
![LTSpice](https://img.shields.io/badge/LTspice-24292F?style=flat-square)
![Linux](https://img.shields.io/badge/Ubuntu-24292F?style=flat-square&logo=ubuntu&logoColor=white)
![Git](https://img.shields.io/badge/Git-24292F?style=flat-square&logo=git&logoColor=white)
![LaTeX](https://img.shields.io/badge/LaTeX-24292F?style=flat-square&logo=latex&logoColor=white)

---

## Selected work

<table>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/kartikeyy12/EdgeFusion">EdgeFusion</a></h3>
      <sub>C++20 &nbsp;|&nbsp; ZeroMQ &nbsp;|&nbsp; OpenCV &nbsp;|&nbsp; Eigen3</sub>
      <p>A real-time sensor fusion pipeline that replaces ROS2 image transport with a custom C++20 stack. A 15-state EKF fuses 200 Hz IMU and 30 Hz camera data over zero-copy ZeroMQ IPC, reaching 277 us latency (25 to 80x faster) and saving 27 MB/s of bandwidth.</p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/kartikeyy12/Fault-Tolerant-RISC-V-SoC">Fault-Tolerant RISC-V SoC</a></h3>
      <sub>SystemVerilog &nbsp;|&nbsp; Yosys &nbsp;|&nbsp; Verilator &nbsp;|&nbsp; cocotb</sub>
      <p>A temporal lockstep dual-core RV32I SoC that compares PC, ALU and register writeback every cycle, paired with a 4x4 systolic array accelerator. Verified with UVM-style tests and synthesized for a Gowin GW1NR-9 FPGA with zero structural errors across 26,897 cells.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/kartikeyy12/LoRa-Perimeter-Detection">LoRa Perimeter Detection System</a></h3>
      <sub>ESP32 &nbsp;|&nbsp; LoRa &nbsp;|&nbsp; 24 GHz mmWave &nbsp;|&nbsp; PIR</sub>
      <p>A low-power sensor node that fuses mmWave radar with PIR to classify movement as human, animal or vehicle, then sends alerts over long-range LoRa. In progress, currently focused on data collection and classification reliability.</p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/kartikeyy12/GFSK-Digital-Walkie-Talkie">GFSK Digital Walkie-Talkie</a></h3>
      <sub>Arduino &nbsp;|&nbsp; NRF24L01 &nbsp;|&nbsp; MATLAB &nbsp;|&nbsp; KiCAD</sub>
      <p>A custom 2.4 GHz half-duplex transceiver on a KiCAD-routed PCB. MATLAB link-budget models were validated in hardware, reaching 1.5 to 2 km of clear audio with 8-bit PCM quantization and a custom PWM-based DAC filter.</p>
    </td>
  </tr>
</table>

---

## GitHub activity

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=kartikeyy12&show_icons=true&hide_border=true&theme=default&bg_color=ffffff&title_color=24292F&icon_color=57606A&text_color=57606A" alt="GitHub stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=kartikeyy12&layout=compact&hide_border=true&theme=default&bg_color=ffffff&title_color=24292F&text_color=57606A" alt="Top languages" />

<br />

<img src="https://streak-stats.demolab.com?user=kartikeyy12&hide_border=true&background=FFFFFF&ring=24292F&fire=24292F&currStreakNum=24292F&currStreakLabel=24292F&sideNums=57606A&sideLabels=57606A&dates=57606A" alt="GitHub streak" />

</div>

---

## Beyond the terminal

I coordinate outreach for the **SPIE Student Chapter at NIT Goa**, running hands-on STEM workshops and school science exhibitions across Goa. I'm also Vice-President of **Exposure Explorers**, the photography club, where I lead the visual documentation of campus events.

---

<div align="center">

Always happy to talk about embedded systems, edge AI or anything with a tight latency budget.

<a href="mailto:kartikey120207@gmail.com">kartikey120207@gmail.com</a>

</div>
