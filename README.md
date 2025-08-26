## Conf
`/etc/default/grub`
```
GRUB_CMDLINE_LINUX_DEFAULT="quiet splash"
sudo update-grub
```


## Ubuntu
```
sudo git clone https://github.com/Mantodkaz/mobpsycho-plymouth-themes \
  /usr/share/plymouth/themes/mobpsycho

sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/mobpsycho/mobpsycho.plymouth 100
sudo update-alternatives --config default.plymouth

sudo update-initramfs -u
```
