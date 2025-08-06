# Misson100K
**High altitude long distance wireless live video/telemetry transmission system for weather balloons.**

I'm thrilled to present my work on a remote wireless live video transmission.

This solution delivers stable HD video, for example, over a distance of more than 20 kilometers using Wi-Fi,Yes you heard it right. It was founded upon ALFA Network dual band AC1200 wireless adapters, three on the receiver's side, and one at the transmitter, to build up a beam forming(MIMO), high bandwidth network.

For maximum range and signal quality, I used PCB antennas(Maple Leaf), leveraging antenna diversity with three antennas to avoid interference and signal loss. The micro controller is a Raspberry Pi, with Open HD being used to handle real time video encoding and transmission from the Raspberry Pi camera.

The system is powered by a high capacity lithium battery with a UBEC BEC for voltage stabilization, and a cooling fan in order to maintain thermal stability.

I housed the whole installation within a weather balloon payload such that it would be transported to stratospheric altitudes. A sonde device provides real time telemetry data, such as GPS, altitude, and environmental conditions yet another collection of functionality for the system.


**This project demonstrates how I built a real time HD video transmission system that works over 20 kilometers using OpenHD, Raspberry Pi, and long-range Wi-Fi hardware. The setup was mounted on a weather balloon, with telemetry and video feed transmitted back to the ground in real time.**

🛠️ Supplies

    ✅ ALFA Network Long-Range Dual-Band AC1200 Wi-Fi Adapters (at least 3 for receiver, 1 for transmitter)

    ✅ Raspberry Pi Zero / 3 / 4 / 5

    ✅ Raspberry Pi Camera (compatible with OpenHD)

    ✅ High capacity LiPo battery

    ✅ UBEC/Buck converter (for regulated power supply)

    ✅ Maple Leaf / Custom PCM Antennas

    ✅ Small CPU cooling fan

    ✅ MicroSD Card (with OpenHD image)

    ✅ Laptop or Linux system (for ground station)

    ✅ Insulation tape, zip ties, and weather balloon payload case

    ✅ Optional: Extra Wi-Fi Adapters for redundancy

📦 Step-by-Step Instructions
Step 1: Get Compatible Hardware

    Choose hardware supported by OpenHD, OpenIPC, WFB-NG, or EZ-Wifibroadcast.

    Make sure all network cards are compatible with Raspberry Pi and support monitor mode.

Step 2: Install OpenHD on Air Unit (Raspberry Pi)

    Use the official OpenHD installer to create a bootable image.

    Flash the image to the Pi’s microSD card.

    Insert the SD card into the Pi and connect the Raspberry Pi Camera.

Step 3: Install OpenHD on Ground Station (Linux or Pi)

    Option 1: Flash a USB drive with OpenHD Ground Station image.

    Option 2: Use terminal:

    sudo apt update
    sudo apt install openhd

Step 4: Connect and Configure Hardware

    Connect the camera to the Raspberry Pi CSI port.

    Power the Raspberry Pi using a LiPo battery through a UBEC/Buck converter.

    Connect Wi-Fi adapters via USB (use powered hubs if needed).

    Add the cooling fan for thermal management.

Step 5: Optional Add-ons

    Add more Wi-Fi adapters at the ground station for antenna diversity and improved stability.

    Consider using directional antennas for higher range and signal integrity.

Step 6: Tune OpenHD Settings

    Adjust resolution and bitrate based on desired video quality and range:

        720p30 recommended for smoother feed at long distances.

        Lower bitrate for more stable connections.

Step 7: Final Checks & Launch Prep

    Ensure all hardware is secured and insulated.

    Test signal strength and latency before launch.

    Verify GPS lock and telemetry readout.

    Launch the weather balloon, monitor video and telemetry in real-time.

🎈 Telemetry (Sonde Device)

    The setup includes a sonde device that transmits altitude, GPS location, and environmental data.

    Use ground station software to visualize telemetry alongside video.

🧪 Results

    Achieved stable live HD video transmission over 20km.

    Maintained low latency and high signal integrity throughout balloon ascent.



