# Prometheus-grafana-setup
This repo created for prometheus and grafana setup on docker-compose 
###njeffnjreknfej
Create for memory dashbord:
---------------------------------------------
node_memory_MemTotal_bytes/1024/1024/1024 
node_memory_MemAvailable_bytes/1024/1024/1024
node_memory_MemFree_bytes/1024/1024/1024

Create for CPU Information
---------------------------------------
process_cpu_seconds_total

Create disk dashboard 
---------------------------------------------------------------------------------------------
node_disk_info{device="xvda",major="202",minor="0",model="",path="",revision="",serial="",wwn=""}
node_disk_io_now{device="xvda"}
node_disk_io_time_seconds_total{device="xvda"}
node_disk_read_bytes_total{device="xvda"}
node_disk_read_time_seconds_total{device="xvda"}
node_disk_write_time_seconds_total{device="xvda"}
node_disk_written_bytes_total{device="xvda"}

=======================================================
windows Servers: 
========================
memory
windows_cs_physical_memory_bytes/1024/1024/1024
windows_os_physical_memory_free_bytes
windows_os_virtual_memory_bytes
windows_os_virtual_memory_free_bytes
windows_os_visible_memory_bytes

cpu
-----------------------------------
HELP process_cpu_seconds_total ==> Total user and system CPU time spent in seconds.

memory
------------------------------------
windows_logical_disk_size_bytes/1024/1024/1024 Total space in bytes, updates every 10-15 min (LogicalDisk.PercentFreeSpace_Base)
windows_logical_disk_size_bytes   ==> Total space in bytes, updates every 10-15 min (LogicalDisk.PercentFreeSpace_Base)
windows_physical_disk_reads_total The number of read operations on the disk (PhysicalDisk.DiskReadsPerSec)
windows_physical_disk_write_seconds_total Seconds that the disk was busy servicing write requests (PhysicalDisk.PercentDiskWriteTime)


