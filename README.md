# embeddedlinuxexperiment

Step 1
sudo apt update
Step 2 
sudo apt install gcc-arm-linux-gnueabi qemu-user file build-essential -y



Step 3 — Verify Installation

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
