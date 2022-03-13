# Notes for working with Fedora Linux

The commands below are known to work with Fedora Linux 35

    sudo dnf install make kernel-devel dkms

    lsmod | grep fake
    dmesg | grep fake

    sudo modprobe fake_dp_dual_mode
    sudo rmmod fake_dp_dual_mode

    # sudo dkms build fake_dp_dual_mode/1.0.1 -c ./fedora/dkms.conf
    sudo dkms install fake_dp_dual_mode/1.0.1 -c ./fedora/dkms.conf

    ls /usr/src/fake_dp_dual_mode-1.0.1/
