CENTOS7.5_PATH=http://centos-mirror.rbc.ru/pub/centos/7.5.1804/isos/x86_64/CentOS-7-x86_64-Minimal-1804.iso

CENTOS7_PATH=${CENTOS7.5_PATH}

centos7-import:
	sudo chyves iso import ${CENTOS7_PATH}

centos7-create:
	sudo chyves centos7 create 15G
	sudo chyves centos7 set uefi_firmware=BHYVE_UEFI.fd
	sudo chyves centos7 set os=linux
	sudo chyves centos7 set ram=2G
	sudo chyves centos7 set loader=uefi
	sudo chyves centos7 set description="Default CentOS 7 guest"
	sudo chyves centos7 set uefi_console_output=vnc
	sudo chyves centos7 set uefi_vnc_client=freerdp
	sudo chyves centos7 set uefi_vnc_mouse_type=usb3
	sudo chyves centos7 set uefi_vnc_pause_until_client_connect=yes
	sudo chyves centos7 set uefi_vnc_res=800x600

centos7-install:
	sudo chyves centos7 start CentOS-7-x86_64-Minimal-1503-01.iso

centos7-start:
	sudo chyves centos7 start

centos7-stop:
	sudo chyves centos7 stop

alt:
	sudo chuves altlinux create 20G
	sudo chyves altlinux set uefi_firmware=BHYVE_UEFI.fd
	sudo chyves altlinux set os=linux
	sudo chyves altlinux set ram=2G
	sudo chyves altlinux set description="Default ALT Linux guest"
	sudo chyves altlinux set uefi_console_output=vnc
	sudo chyves altlinux set uefi_vnc_client=freerdp
	sudo chyves altlinux set uefi_vnc_mouse_type=usb3
	sudo chyves altlinux set pause_until_client_connect=yes
	sudo chyves altlinux set uefi_vnc_res=800x600

alt-install:
	sudo chyves altlinux start alt-workstation-8-x86_64.iso

alt-start:
	sudo chyves altlinux start alt-workstation-8-x86_64.iso

alt-stop:
	sudo chyves altlinux stop

