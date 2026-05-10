# embeddedlinuxexperiment

Step 1 — Update Linux
sudo apt update
Step 2 — Install ARM Compiler and QEMU
sudo apt install gcc-arm-linux-gnueabi qemu-user file build-essential -y

Wait until installation completes.

Step 3 — Verify Installation

Run:

arm-linux-gnueabi-gcc --version

You should see compiler version output.

Then run:

qemu-arm --version

You should see QEMU version output.

Step 4 — Compile Again
arm-linux-gnueabi-gcc -static arm_app.c -o arm_app
Step 5 — Run Program
qemu-arm ./arm_app

Expected output:

Embedded Linux ARM Application Started
Cross Compilation Successful
Application Running in ARM Environment
