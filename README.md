# linux

command
virt-install --name win11-test --ram 8196 --vcpus=8 \
--disk path=/home/kvm/image/win11/win11-1.qcow2,size=100,bus=virtio   \
--cdrom=/home/kvm/iso/zh-cn_windows_11_business_editions_version_22h2_updated_march_2023_x64_dvd_3523ddc7.iso   \
--cdrom=/usr/share/virtio-win/virtio-win.iso  \
--accelerate --network bridge=br0  \
--os-type=windows   \
--os-variant=win11  \
--graphics vnc,listen=0.0.0.0,port=5930
