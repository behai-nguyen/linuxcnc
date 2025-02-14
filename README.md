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

## License
[MIT license](http://www.opensource.org/licenses/mit-license.php)
and the [GPL license](http://www.gnu.org/licenses/gpl.html).
