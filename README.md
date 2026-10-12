# System Log Analyzer

This is an automated system-diagnostic-and-log-processing-pipeline.

## Environment Specifications:

- Ubuntu Linux > 11.4+
- g++ compiler
- Python 3+

- Other Tools:
  If you're using a virtual machine or remotely connecting to a linux computer from a Windows OS machine. You will need:
- WinSCP (for file sharing)
- PuTTY

## How to use this project

- Step 1: Clone this GitHub repo

```
https://github.com/ecoderP/system-log-analyzer.git
```

- Step 2: Copy project folder to a Linux environment
- Step 3: cd into project folder and rename system_dump_Sample.txt to system_dump.txt

```
cd system-log-analyzer
```

```
mv system_dump_Sample.txt system_dump.txt
```

Note: Skip renaming if you intend to use real system logs

Step 4: Optional. To use with your system logs, save recent system logs to a a text file

```
sudo tail -n 100 /var/log/syslog --since "1 hour ago" >> system_dump.txt
```

Step 5: Change file permissions for run.sh and run the script

```
chmod +x run.sh
```

```
./run.sh
```

<!--
- run.sh
- system log parser
- controller
- Transfer process ownership to Python.
- Python is responsible for:
  - validating input
  - executing the C++ parser
  - analyzing the generated CSV
  - returning the final application exit status

---

## Architecture Overview

This :

---

## Prerequisites

This pipeline is designed to work in a Linux environment. You should also have:

- Python3 installed
- g++ compiler for C++

---



## Lessons Learned

---

## 📈 Future Improvements

-->

---

## 👨‍💻 Author

Built and Maintained by [ecoderP](https://github.com/ecoderP)
