# set_cpu_governor_ubuntu_22.04

After enabling the service

cat /sys/devices/system/cpu/cpu*/cpufreq/scaling_governor

Should return "performance" on all cores
