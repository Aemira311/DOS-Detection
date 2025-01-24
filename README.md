# DOS-Detection
DOS Detection System
Overview:
This project is a Python-based Denial of Service (DOS) Detection System designed to monitor and analyze network traffic for abnormal patterns indicative of DOS attacks. The system generates alerts for large packets and excessive traffic to help protect networks from malicious activity.

Features:
Packet Monitoring: Tracks ICMP packets in real-time.
Traffic Analysis: Identifies abnormal traffic patterns based on defined thresholds.
Alert System: Provides visual alerts using a custom messagebox.
Customizable Thresholds: Allows adjustments for packet size and count limits.

Prerequisites:
Python: Ensure you have Python 3.x installed on your system.

Dependencies:
Scapy: For network packet sniffing and analysis.
Tkinter: For GUI-based alert popups.


To install Scapy, run:
pip install scapy



Here's a suggested content structure for your README.md file to accompany the DOS Detection project:

DOS Detection System
Overview
This project is a Python-based Denial of Service (DOS) Detection System designed to monitor and analyze network traffic for abnormal patterns indicative of DOS attacks. The system generates alerts for large packets and excessive traffic to help protect networks from malicious activity.

Features
Packet Monitoring: Tracks ICMP packets in real-time.
Traffic Analysis: Identifies abnormal traffic patterns based on defined thresholds.
Alert System: Provides visual alerts using a custom messagebox.
Customizable Thresholds: Allows adjustments for packet size and count limits.
Prerequisites
Python: Ensure you have Python 3.x installed on your system.
Dependencies:
Scapy: For network packet sniffing and analysis.
Tkinter: For GUI-based alert popups.
To install Scapy, run: pip install scapy


Setup:
1-Clone this repository.
2-Identify your network interface:
Replace "Loopback Pseudo-Interface 1" in the code with your actual network interface name.

You can list available interfaces using the following command:
from scapy.interfaces import get_if_list
print(get_if_list())

3-Run the code.

How It Works
The system monitors ICMP packets on the specified network interface.

It keeps track of:
Total packets: Per source IP within a defined time window.
Large packets: ICMP packets exceeding the threshold size.

Alerts are triggered when:
The number of packets from a single IP exceeds the DOS threshold.
The number of large packets exceeds the large packet threshold.

Alerts
Large Packet Alert: Displays a warning when an unusually large packet is detected.
DOS Attack Alert: Displays an error message when excessive traffic from a single source is detected.

Customization
You can adjust the following parameters in the code:

DOS_THRESHOLD: Number of packets to trigger a DOS alert.
LARGE_PACKET_SIZE: Packet size threshold for large packets.
TIME_WINDOW: Time duration (in seconds) for traffic analysis.

## Contribution
Contributions are welcome! If you have ideas for enhancements or bug fixes, feel free to open an issue or submit a pull request.

Contact
For any questions or contributions, feel free to reach out:
Email: abdelrahman.emira311@gmail.com
LinkedIn: www.linkedin.com/in/abdelrahman-emira-48b187239
