\# Corstone-300 FVP (CS300) Demo - YOLOv8 on Ethos-U55



\## What I achieved

\- Built `img\_yolov8\_192` use case in ML Embedded Evaluation Kit

\- Generated AXF firmware: `ethos-u-img\_yolov8\_192.axf`

\- Launched Corstone-300 FVP (Cortex-M55 + Ethos-U55) and verified GUI runs



\## Environment

\- Windows 11

\- WSL2 + WSLg

\- Docker Desktop



\## How to run (WSL)

```bash

FVP=/mnt/c/Users/yoyo1/YOLOv8\_FVP\_READY/FVP\_Corstone\_SSE-300/models/Linux64\_GCC-6.4/FVP\_Corstone\_SSE-300\_Ethos-U55

AXF=/mnt/c/Users/yoyo1/ethos-u-img\_yolov8\_192.axf

"$FVP" -C ethosu.num\_macs=64 "$AXF"

