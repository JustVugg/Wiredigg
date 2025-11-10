<p align="center">
  <img src="wiredigg.png" alt="Logo" width="800"/>
</p>


[![Platform](https://img.shields.io/badge/platform-Windows-blue)](https://github.com/yourusername/wiredigg)  
[![Python](https://img.shields.io/badge/python-3.7%2B-brightgreen)](https://www.python.org/)  
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Wiredigg is an advanced, AI-powered Python tool for real-time network packet capture, deep protocol analysis, anomaly detection, and threat intelligence.  
Designed for network administrators, security professionals, and IT enthusiasts, Wiredigg combines cutting-edge machine learning with a modern user interface to deliver actionable insights and unparalleled network visibility.

---

## **Key Features**

### **AI & Machine Learning Integration**
- **OllamaValidator**: Leverages advanced AI to validate ML-detected anomalies and reduce false positives.
- **Incremental ML Training**: Continuously improves anomaly detection accuracy with user feedback.
- **Threat Classification**: Automatically classifies threats based on severity and type.
- **False Positive Management**: Mark and retrain the ML model to refine detection.

### **Real-Time Network Analysis**
- **Packet Capture**: Monitor and filter network traffic in real-time.
- **Protocol Analysis**: Detailed breakdown of protocols (TCP, UDP, ICMP, HTTP, etc.).
- **Advanced Filtering**: Filter traffic by protocol, IP, port, and more.
- **Promiscuous Mode**: Enable or disable promiscuous mode for packet capture.

### **IoT and Cloud Analytics**
- **Device Identification**: Detect and classify IoT devices on the network.
- **Risk Evaluation**: Assess the security risks of IoT devices based on behavior and traffic patterns.
- **Cloud Protocol Analysis**: Analyze traffic patterns for cloud services.

### **Security Dashboards**
- **Threat Intelligence**: Built-in database for malicious IPs, domains, and patterns.
- **Interactive Tables**: Sortable and filterable tables for packets and threats.
- **Visualization**: Graphs for protocol statistics, network flows, and threat analysis.

### **Custom Packet Sending**
- **Simple Packet Testing**: Send user-defined packets to test network connectivity.
- **Customizable Parameters**: Specify destination IP, protocol, port, and data.

### **Reporting and Export**
- **Multi-Format Reports**: Export detailed threat reports in HTML, JSON, or text formats.
- **Customizable Content**: Include packet details, threat type, and severity in reports.

### **Modern User Interface**
- **Dark Mode**: Aesthetic improvements with a Nordic dark theme.
- **Tooltips**: Contextual tooltips for better usability.
- **Auto-Scroll**: Automatically scroll through live packet captures.

---

## **Requirements**

- Python 3.7+
- Required Python packages:
  - `tkinter`
  - `numpy`
  - `matplotlib`
  - `networkx`
  - `scikit-learn`
  - `netifaces`
  - `pandas`
  - `requests`

---

## **Installation**

1. Clone the repository:
   ```bash
   git clone https://github.com/Zrufy/wiredigg.git
   cd wiredigg
   ```

2. Install required packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the application:

   ```bash
   python wiredigg.py
   ```

> **Note:** Administrator/root privileges are required for packet capture on most systems.

---

## **Usage Guide**

### **Capturing Network Traffic**

1. Select a network interface from the dropdown list.
2. Click **"Start Capture"** to begin monitoring network traffic.
3. Use filters to focus on specific protocols, IPs, or ports.
4. Click **"Stop Capture"** when done.

### **Analyzing Threats**

1. Navigate to the **"Security Analysis"** tab.
2. Click **"Analyze Threats"** to scan captured packets for potential security issues.
3. Double-click on a detected threat for detailed information.
4. View threat details, payload analysis, and security recommendations.

### **Using Machine Learning Detection**

1. Click **"ML Detection"** to analyze traffic with the machine learning model.
2. Mark false positives to improve the model's accuracy.
3. Use batch actions to process multiple detections at once.

### **Working with IoT Devices**

1. Navigate to the **"IoT/Cloud"** tab.
2. Click **"Identify IoT Devices"** to detect and classify network devices.
3. View detailed information about each device and assess potential risks.

### **Generating Traffic Predictions**

1. Navigate to the **"Predictive Analysis"** tab.
2. Click **"Generate Predictions"** to view traffic forecasts.
3. Monitor potential traffic anomalies and trends.

### **Custom Packet Sending**

1. Use the **"Send Simple Packet"** feature to test network connectivity and response.
2. Enter destination IP, protocol (TCP/UDP), port, and data.
3. Click **"Send"** to transmit the packet.
4. View response data if available.

---

## **Architecture**

Wiredigg is built on a multi-threaded architecture to ensure a responsive UI while handling intensive packet capture and analysis:

* **Main Thread**: UI management and user interaction.
* **Capture Thread**: Packet sniffing and initial processing.
* **Analysis Threads**: Security analysis and ML detection.
* **Background Training**: Continuous improvement of the ML model.

---

## **Contributing**

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository.
2. Create your feature branch:

   ```bash
   git checkout -b feature/amazing-feature
   ```
3. Commit your changes:

   ```bash
   git commit -m "Add some amazing feature"
   ```
4. Push to the branch:

   ```bash
   git push origin feature/amazing-feature
   ```
5. Open a Pull Request.

---

## **License**

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## **Acknowledgements**

* **Tkinter** for the UI framework.
* **Matplotlib** for data visualization.
* **NetworkX** for network graph analysis.
* **Scikit-learn** for machine learning capabilities.
* **Netifaces** for network interface detection.
* **Requests** for HTTP communication.

---

> ⚠️ **Note:** Wiredigg is designed for legitimate network analysis and security purposes only.
> Always ensure you have proper authorization before capturing network traffic in any environment.
