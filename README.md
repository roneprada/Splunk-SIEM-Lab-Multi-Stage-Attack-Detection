# Splunk-SIEM-Lab-Multi-Stage-Attack-Detection

### 🔧 Incident — Multi-Stage Attack Investigation

**Objective:**  
Detect and analyze a multi-stage attack using log data.

**Detection:**  
Identified repeated failed login attempts followed by a successful login from the same IP.

**Investigation:**  
- Correlated login events with file access and command execution  
- Identified suspicious activity including file download and lateral movement attempts  
- Observed abnormal command execution (`whoami`) indicating system probing  

**Findings:**  
- Brute force login succeeded  
- Unauthorized access to internal systems  
- Attempted lateral movement  
- Command execution activity detected  

**Root Cause:**  
Weak authentication controls allowed attacker access.

**Response Actions:**  
- Blocked malicious IP  
- Disabled compromised account  
- Reset credentials  
- Monitored system for further activity  

**Validation:**  
Confirmed full attack chain and containment through log analysis.
