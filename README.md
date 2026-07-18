<!-- 14/02/2025. -->

# linuxcnc

Documentation of my learning process to build a CNC machine using LinuxCNC.

## Documentation

1. [Raspberry Pi 4B: Natively Build a 64 Bit Fully Preemptible Kernel (Real-Time) with Desktop](https://behainguyen.wordpress.com/2024/11/03/raspberry-pi-4b-natively-build-a-64-bit-fully-preemptible-kernel-real-time-with-desktop/)

*In this article, I present a step-by-step procedure to natively patch and build a 64-bit Fully Preemptible Kernel (Real-Time) for my Raspberry Pi 4B (Pi 4B). We start with a pre-made operating system image that includes a desktop environment. After building and installing the real-time patch kernel, querying the kernel information with the command <code>uname -a</code> should report something similar to:*

*``Linux picnc 6.6.59-rt45-v8-behai-rt-build+ #1 SMP PREEMPT_RT Sat Nov  2 10:20:46 AEDT 2024 aarch64 GNU/Linux``.*

*This indicates that the token **``PREEMPT_RT``** is present in the output. **Natively** in this instance means that we patch and build the kernel using the very Pi 4B on which the newly built kernel is installed.*

2. [Raspberry Pi 4B: LinuxCNC Max Jitter or Latency Test](https://behainguyen.wordpress.com/2025/02/13/raspberry-pi-4b-linuxcnc-max-jitter-or-latency-test/)

*I conducted the LinuxCNC Max Jitter or Latency Test on my Raspberry Pi 4 Model B Rev 1.5, equipped with 8GB of RAM and running Debian GNU/Linux 12 (Bookworm) 6.12.11. The results are rather erratic, and I'm not sure how to interpret them. In this post, I present the results and describe the tests.*

3. [Raspberry Pi 4B LinuxCNC: Initial Setup for the Mesa 7I96S Ethernet Motion Control](https://behainguyen.wordpress.com/2025/02/14/raspberry-pi-4b-linuxcnc-initial-setup-for-the-mesa-7i96s-ethernet-motion-control/)

*In this post, I describe the initial setup for the Mesa <a href="https://store.mesanet.com/index.php?route=product/product&product_id=374" title="7I96S STEP/IO Step & dir plus I/O card" target="_blank">7I96S Ethernet motion control STEP/IO Step & Dir plus I/O card</a>. The setup includes selecting the power supply and configuring the network IP address.*

4. [Raspberry Pi 4B LinuxCNC: Wiring the Mesa 7I96S Ethernet Motion Control, Closed-Loop CL57T Stepper Driver, and Nema 23 Stepper Motor](https://behainguyen.wordpress.com/2025/02/16/raspberry-pi-4b-linuxcnc-wiring-the-mesa-7i96s-ethernet-motion-control-closed-loop-cl57t-stepper-driver-and-nema-23-stepper-motor/)

*This post documents the wiring of the Mesa <a href="https://store.mesanet.com/index.php?route=product/product&product_id=374" title="7I96S STEP/IO Step & dir plus I/O card" target="_blank">7I96S Ethernet motion control STEP/IO Step & Dir plus I/O card</a> to the <a href="https://www.omc-stepperonline.com/closed-loop-stepper-driver-v4-1-0-8-0a-24-48vdc-for-nema-17-23-24-stepper-motor-cl57t-v41" title="CL57T Closed-Loop Stepper Driver" target="_blank">CL57T closed-loop stepper driver</a>, which in turn controls the closed-loop <a href="https://www.omc-stepperonline.com/nema-23-closed-loop-stepper-motor-3-0nm-424oz-in-encoder-1000ppr-4000cpr-23hs45-4204d-e1000" title="Mema 23 Stepper Motor" target="_blank">Mema 23</a> stepper motor.*

5. [Raspberry Pi 4B: Natively Built 64 Bit Fully Preemptible Kernel (Real-Time) Gets Overridden](https://behainguyen.wordpress.com/2025/02/19/raspberry-pi-4b-natively-built-64-bit-fully-preemptible-kernel-real-time-gets-overridden/)

*Running <a href="https://linuxcnc.org/docs/html/config/pncconf.html" title="PnCconf Mesa Configuration Wizard" target="_blank">PnCconf</a> on the natively built 64-bit Fully Preemptible Kernel (Real-Time) kernel, as <a href="https://behai-nguyen.github.io/2024/11/03/pi-4b-preempt-rt-kernel-patch.html" title="Raspberry Pi 4B: Natively Build a 64 Bit Fully Preemptible Kernel (Real-Time) with Desktop" target="_blank">previously discussed</a>, resulted in the following message: <code>You are using a simulated-realtime version of LinuxCNC, so testing / tuning of hardware is unavailable</code>. In this post, we will examine what has happened, prove that the finding is correct, and present the results of the jitter or latency test we conducted on the Raspberry Pi OS.*

6. [Raspberry Pi 4B LinuxCNC: Wiring the Mesa 7I96S Card and a Contactor to Control a Grinder/Router via the LinuxCNC Application](https://behainguyen.wordpress.com/2025/07/01/raspberry-pi-4b-linuxcnc-wiring-the-mesa-7i96s-card-and-a-contactor-to-control-a-grinder-router-via-the-linuxcnc-application/)

*This post documents how to wire the Mesa <a href="https://store.mesanet.com/index.php?route=product/product&product_id=374" title="7I96S STEP/IO Step & dir plus I/O card" target="_blank">7I96S Ethernet motion control STEP/IO Step & Dir plus I/O card</a> to a contactor, enabling the LinuxCNC application to switch a wood router (or grinder) on and off using G-code commands.*

7. [Raspberry Pi 4B LinuxCNC: Main Power Distribution (Wiring)](https://behainguyen.wordpress.com/2025/09/04/raspberry-pi-4b-linuxcnc-main-power-distribution-wiring/)

*By “main power,” I mean the wiring from the AC inlet to the three power supply units used in the LinuxCNC system I am building. In this post, I list the relevant components and share the wiring pictures.*

8. [Raspberry Pi 4B LinuxCNC: Mesa 7I96S Ethernet Motion Control, Expanded to Four CL57T Drivers and Four Nema 23 Closed-Loop Stepper Motors](https://behainguyen.wordpress.com/2026/06/29/raspberry-pi-4b-linuxcnc-mesa-7i96s-ethernet-motion-control-expanded-to-four-cl57t-drivers-and-four-nema-23-closed-loop-stepper-motors/)

*I now have four CL57T drivers and four Nema 23 closed-loop stepper motors for the X, Y, Y-tandem, and Z axes. This video briefly recaps the configuration and wiring, and concludes by running a test G-code program that draws a square on the X-Y plane, showing the X-axis motor and both Y-axis motors running.*

9. [Raspberry Pi 4B LinuxCNC: Homing to the Origin (0, 0, 0)](https://behainguyen.wordpress.com/2026/07/06/raspberry-pi-4b-linuxcnc-homing-to-the-origin-0-0-0/)

*My LinuxCNC 2.9.4 home position was set to coordinates I didn't quite understand. I am documenting the Gemini-assisted troubleshooting process I used to set it to the origin <code>(0, 0, 0)</code>. This is not a tutorial, but rather a record of my learning progression.*

10. [Raspberry Pi 4B LinuxCNC: Resolving the “Unexpected realtime delay on task0…” Startup Error](https://behainguyen.wordpress.com/2026/07/10/raspberry-pi-4b-linuxcnc-resolving-the-unexpected-realtime-delay-on-task0-startup-error/)

*After launching LinuxCNC, it consistently reported <code>Unexpected realtime delay on task0 with period 500000</code>. Despite this startup error, LinuxCNC otherwise appeared to operate normally. I am documenting the AI-assisted troubleshooting process I used to resolve this error. Again, this is not a tutorial, but rather a record of my learning progression.*

11. [Raspberry Pi 4B LinuxCNC: Wiring and “Configuring” Eight NPN Normally Open Inductive Proximity Sensors to the Mesa 7I96S Card](https://behainguyen.wordpress.com/2026/07/18/raspberry-pi-4b-linuxcnc-wiring-and-configuring-eight-npn-normally-open-inductive-proximity-sensors-to-the-mesa-7i96s-card/)

*This post describes how to wire eight NPN NO (Normally Open) inductive proximity sensors to the <a href="https://store.mesanet.com/index.php?route=product/product&product_id=374" title="7I96S STEP/IO card" target="_blank">Mesa 7I96S card</a>. The title and the wiring diagram refer to eight sensors, but I wired, configured, and tested only one. I originally bought eight sensors, but unfortunately managed to fry one, leaving seven available for future use. Again, this is not intended to be a tutorial, but rather a record of my learning progression.*

## License
[MIT license](http://www.opensource.org/licenses/mit-license.php)
and the [GPL license](http://www.gnu.org/licenses/gpl.html).
