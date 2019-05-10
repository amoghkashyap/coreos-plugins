# coreos-plugins
on Host

export http_proxy=http://10.158.100.6:8080
export https_proxy=http://10.158.100.6:8080
export PATH="/opt/nvidia/bin/:$PATH"
export PATH="/opt/bin:$PATH"

on K8s
export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/nvidia/lib64/
export PATH=$PATH:/usr/bin/nvidia/
