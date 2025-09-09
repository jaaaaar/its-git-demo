# Usage Guide

## System Info Script

### Purpose
Shows basic system information.

### Usage
```bash 
./system_info.sh


#!/bin/bash
echo "=== System Information ==="
echo "Date: $(date)"
echo "User: $(whoami)"
echo "Current directory: $(pwd)"
echo "Home directory: $HOME"
echo ""
echo "=== Disk Usage ==="
df -h | head -5
echo ""
echo "=== Memory Info ==="
free -h 2>/dev/null || echo "Memory info not available"
echo ""
echo "Script completed successfully!"
