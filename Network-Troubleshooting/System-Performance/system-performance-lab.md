# Windows System Performance Investigation

## Objective
Investigate Windows system resource usage to understand how CPU, memory, disk, and running applications affect computer performance.

## Environment
- Operating System: Windows 11
- Tools: Windows Task Manager, Google Chrome Task Manager
- Applications: Google Chrome

## 1. Windows Task Manager — Processes

Observed system resource usage:

| Resource | Observed Usage |
|---|---:|
| CPU | Approximately 13% |
| Memory | Approximately 25% |
| Disk | Approximately 0% |

Google Chrome was the largest resource consumer for both CPU and memory.

## 2. Chrome Task Manager

Opened Chrome Task Manager using `Shift + Esc`.

Observations:
- 8 browser tabs were open.
- The Windows Troubleshooting Portfolio tab used the most memory.
- Its CPU usage fluctuated, generally staying relatively low but occasionally reaching higher values.
- Network activity was displayed in KB/s when processes transferred data.

The CPU fluctuations did not appear consistently high, suggesting normal browser activity rather than a persistent performance issue.

## 3. System Memory Investigation

Used Windows Task Manager's Performance tab to inspect memory.

| Metric | Result |
|---|---:|
| Installed Memory | 64 GB |
| Memory In Use | 16.2 GB |
| Memory Usage | Approximately 28% |
| Available Memory | Approximately 47.8 GB |

The system had substantial available memory, with no obvious indication of memory pressure.

## 4. Preliminary Conclusion

The system showed relatively low CPU usage and substantial available memory during the investigation. Chrome was the largest application resource consumer, but its CPU usage fluctuated rather than remaining consistently elevated.

No obvious CPU or memory bottleneck was identified during these observations.

Further investigation of disk activity and performance is needed before reaching a complete conclusion.

## Skills Practiced
- Using Windows Task Manager
- Monitoring CPU and memory usage
- Using Chrome Task Manager
- Identifying resource-intensive applications
- Interpreting network activity measurements
- Documenting system performance findings
