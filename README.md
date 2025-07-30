# 🛡️ TCP Port Scanner (Python)

A multi-threaded TCP port scanner built in Python. This tool scans a target IP address or hostname for open TCP ports and attempts to retrieve service banners from active services. It’s designed for learning and personal cybersecurity skill development.

## 📌 Project Status

✅ Working MVP  
🔧 Continuously improving  
🚀 Built as part of my journey through the SCTP Cybersecurity Programme in Singapore

---

## 🔧 Features

- Accepts target domain or IP
- Scans a user-defined TCP port range
- Multi-threaded for speed (via `ThreadPoolExecutor`)
- Attempts to retrieve service banners from open ports
- Clean color-coded terminal output (using `colorama`)
- Educational and lightweight

---

## 🧰 Requirements

- Python 3.7+
- Install dependencies:

```bash
pip install -r requirements.txt
```

requirements.txt:

```nginx
colorama
```

---

## 🚀 How to Use

```bash
python main.py
```

You’ll be prompted to:

- Enter a target IP address or domain (e.g., scanme.nmap.org)
- Specify start and end port (e.g., 20–100)

Example input:
```yaml
Enter target: scanme.nmap.org
Start port: 20
End port: 100
```
Example output:
```kotlin
[+] Port 22 is open — SSH-2.0-OpenSSH_7.4
[+] Port 80 is open — HTTP/1.1 200 OK
```

---

## 🧠 What I Learned

- How TCP connections work at the socket level
- Basic banner grabbing and service fingerprinting
- Python threading for concurrent I/O-bound tasks
- Importance of input validation and exception handling in networking tools

---

## 📁 Project Structure

```bash
port-scanner/
├── main.py              # Main script
├── requirements.txt     # Required Python packages
├── LICENSE              # MIT license
└── README.md            # Project overview and usage
```
