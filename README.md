## FIO Test Results Visualizer 

A comprehensive web-based tool for visualizing and analyzing FIO (Flexible I/O Tester) benchmark results. 
Features 
 - Interactive Charts: IOPS, throughput, and CLAT latency visualization
 - Multi-test Comparison: Compare results from different test configurations
 - Time-series Analysis: IOPS and CLAT performance over time
 - Detailed Metrics: Comprehensive test parameters and performance data
 - Smart Detection: Automatic handling of single-job vs multi-job tests

### Quick Start 
```
#podman run -d --name simple-fio-visualizer -p 8501:8501 -v <fio-test-results-directory>:/mnt:ro,Z quay.io/abose/simple-fio-visualizer:latest
```

### Requirements
 - summary.json file in the directory(ies) [ <code> while executing fio use --output-format=json --output=summary.json </code> ]
 - iops and latency log for defined intervals in the job file.
```
   write_iops_log=iops
   write_lat_log=latency
   log_avg_msec=5000
```

## Output
<img width="1253" height="1250" alt="image" src="https://github.com/user-attachments/assets/511c0355-e59f-4e6a-8c5a-43b16e083f59" />
