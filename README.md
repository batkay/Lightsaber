# Lightsaber
Repository for custom lightsaber PCB and firmware
## Overview
The firmware folder contains the STMCubeIDE project used to program the STM32F446RE, and the LightsaberDesign folder contains the KiCad project for the PCB used. The Outputs folder contains the outputs from KiCad that was sent to JLCPCB for assembly. The project has been changed since Outputs was last updated, so the folder is not up to date. SpiceSimulations contains the LTSpice simulations used when designing the PCB.
## Obtaining audio
The audio file was obtained by taking a wav file from online, importing it into Audacity, then exporting it as a monochannel 8-bit audio file at 8000Hz. This then allowed the file to be played with interrupts instead of using a DMA.
## Known Issues
When playing audio from the speaker, the noise is extremely noisy. The source of this noise is not currently known, but it is likely due to a hardware issue, as the original noise file can very faintly be heard in the noise.