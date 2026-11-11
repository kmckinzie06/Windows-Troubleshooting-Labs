# Windows System Performance Investigation

## Objective
Investigate Windows system resource usage to understand how CPU, memory, disk, and running applications affect computer performance.

## Environment
- Operating System: Windows 11
- Tools: Windows Task Manager, Google Chrome Task Manager
- Applications: Google Chrome

## 1. Windows Task Manager — Processes

Initial observed system resource usage:

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

## 4. Disk Performance Investigation

Used Windows Task Manager's Performance tab to inspect Disk 0 (C:).

| Metric | Observation |
|---|---:|
| Drive Type | SSD |
| Active Time | 0–2% |
| Average Response Time | Approximately 10 ms |
| Read Speed | Approximately 30 KB/s |
| Write Speed | Approximately 300 MB/s (fluctuating) |

The SSD remained mostly idle during the observation period. Write speed fluctuated, indicating occasional write activity, but active time remained between 0% and 2%.

No obvious storage bottleneck was identified during this investigation.

## 5. Final Conclusion

The system was observed under normal operating conditions.

- CPU usage was approximately 13% during the initial observation.
- Memory usage was approximately 28%, with substantial available RAM.
- SSD active time remained between 0% and 2%.

Chrome was the largest application resource consumer, but its CPU usage fluctuated rather than remaining consistently elevated.

No obvious CPU, memory, or storage bottleneck was identified during the investigation.

These findings represent a snapshot of system performance under the observed conditions. Further testing under heavier workloads would be needed to identify performance issues that occur only under load.

## Skills Practiced

- Using Windows Task Manager
- Monitoring CPU, memory, and disk usage
- Using Chrome Task Manager
- Identifying resource-intensive applications
- Understanding disk read/write activity
- Interpreting performance measurements
- Documenting troubleshooting findings
