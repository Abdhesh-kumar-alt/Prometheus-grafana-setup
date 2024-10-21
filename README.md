Here is a structured and attractive README.md file for your Prometheus and Grafana setup on Docker Compose. It highlights the memory, CPU, and disk dashboards for both Linux and Windows servers.

markdown
Copy code
# Prometheus & Grafana Setup with Docker Compose

This repository contains a complete setup for **Prometheus** and **Grafana** using Docker Compose, with pre-configured dashboards for monitoring memory, CPU, and disk usage across Linux and Windows servers.

## 🚀 Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/prometheus-grafana-setup.git
cd prometheus-grafana-setup
2. Start the Docker Containers
Ensure Docker and Docker Compose are installed on your system. Then, start the services:

bash
Copy code
docker-compose up -d
This will spin up Prometheus and Grafana services, and expose them on their default ports:

Prometheus: http://localhost:9090
Grafana: http://localhost:3000
3. Access Grafana
Once the services are running, open your browser and go to Grafana at http://localhost:3000. Use the default credentials to log in:

Username: admin
Password: admin
📊 Pre-configured Dashboards
Linux Servers Monitoring
Memory Dashboard
Monitors memory usage in gigabytes:

Total Memory: node_memory_MemTotal_bytes / 1024 / 1024 / 1024
Available Memory: node_memory_MemAvailable_bytes / 1024 / 1024 / 1024
Free Memory: node_memory_MemFree_bytes / 1024 / 1024 / 1024
CPU Dashboard
Monitors total CPU usage:

Total CPU Time (seconds): process_cpu_seconds_total
Disk Dashboard
Provides disk usage and performance metrics:

Disk Info: node_disk_info{device="xvda"}
I/O Now: node_disk_io_now{device="xvda"}
I/O Time: node_disk_io_time_seconds_total{device="xvda"}
Bytes Read: node_disk_read_bytes_total{device="xvda"}
Bytes Written: node_disk_written_bytes_total{device="xvda"}
Disk Read Time: node_disk_read_time_seconds_total{device="xvda"}
Disk Write Time: node_disk_write_time_seconds_total{device="xvda"}
Windows Servers Monitoring
Memory Dashboard
Monitors memory usage on Windows servers:

Total Physical Memory: windows_cs_physical_memory_bytes / 1024 / 1024 / 1024
Free Physical Memory: windows_os_physical_memory_free_bytes
Virtual Memory: windows_os_virtual_memory_bytes
Free Virtual Memory: windows_os_virtual_memory_free_bytes
Visible Memory: windows_os_visible_memory_bytes
CPU Dashboard
Provides CPU usage metrics:

Total CPU Time: process_cpu_seconds_total
Disk Dashboard
Monitors disk usage on Windows servers:

Logical Disk Size: windows_logical_disk_size_bytes / 1024 / 1024 / 1024
Free Disk Space: windows_logical_disk_size_bytes
Disk Reads (Total): windows_physical_disk_reads_total
Disk Write Time: windows_physical_disk_write_seconds_total
🛠️ Customizing Dashboards
You can further customize the dashboards using Grafana by adding additional metrics, changing visualization types, or adjusting time ranges.

📂 File Structure
bash
Copy code
├── docker-compose.yml        # Docker Compose setup for Prometheus and Grafana
├── prometheus/               # Prometheus configuration files
│   ├── prometheus.yml        # Prometheus scrape configs and rules
├── grafana/                  # Grafana provisioning and dashboards
│   ├── dashboards/           # Pre-configured dashboards in JSON format
│   ├── datasources/          # Prometheus data source configuration for Grafana
🤝 Contributions
Feel free to submit pull requests or open issues to improve the setup or add new features.

📄 License
This project is licensed under the MIT License.

vbnet
Copy code

### Key Sections:
1. **Setup Instructions**: Helps users quickly get started with cloning the repository and running Prometheus and Grafana via Docker Compose.
2. **Pre-configured Dashboards**: Detailed metrics for memory, CPU, and disk monitoring, both for Linux and Windows servers.
3. **Customizing Dashboards**: Encourages users to further enhance their dashboards.
4. **File Structure**: Clear overview of the repository's structure for easy navigation.

Let me know if you'd like any changes!
