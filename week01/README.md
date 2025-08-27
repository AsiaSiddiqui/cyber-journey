# Week 01 — Lab Setup & Wireshark 101

## 🎯 Aim
- Cybersecurity lab banani aur Wireshark ka basic use seekhna.  
- Apna pehla network packet capture (.pcap) file create karna.  

---

## 🖥️ Environment Setup
- **Host Machine:** (Apna OS likhein — e.g., Windows 11 Home, 8GB RAM, Core i5)  
- **Virtualization Tool:** Oracle VirtualBox  
- **Virtual Machine Installed:** Windows 10 (ISO from Microsoft official site)  
- **Tools Installed:** Wireshark  

---

## ⚙️ Steps Performed
1. Microsoft ki official site se Windows 10 ISO download kiya.  
2. VirtualBox me Windows 10 VM banaya (2 vCPU, 4GB RAM).  
3. Base snapshot save kiya for future rollbacks.  
4. Wireshark install kiya.  
5. Wireshark me live capture start kiya.  
6. CMD se command run kiya:  
   ```bash
   ping 8.8.8.8 -n 4
**7.Browser me http://example.com open kiya.
8.Capture stop kiya aur filter lagaya:**
icmp || http
**9.TCP packet follow kiya aur stream save ki.
10.Capture ko first_capture.pcap file ke naam se save kiya.**

📸 **Screenshots**
VirtualBox VM creation screenshot
Windows VM running screenshot
Wireshark capture running
ICMP packets filtered
HTTP packet view
Follow TCP Stream window

🔍 **Findings**
.ICMP packets clearly show request (ping) and reply (pong).
.HTTP packets visible when accessing example.com.
.TCP stream follow karke pura conversation samajh aata hai between client & server.

📚 **What I Learned**
CIA Triad (Confidentiality, Integrity, Availability) ka concept revise hua.
VirtualBox me VM banana aur snapshot lena seekha.
Wireshark me packet capture, filtering aur TCP stream analysis ka hands-on mila.
Apne pehle .pcap file ko analyze karna seekha.

✅ **Deliverables:**
first_capture.pcap file
4–6 screenshots
Ye README.md documentation

