# Instalação de Drivers Essenciais

## Drivers de Rede e Wi-Fi

- O Debian pode não reconhecer algumas placas Wi-Fi.  
- Se a rede não funcionou na instalação, conecte-se por cabo temporariamente ou baixe os pacotes de firmware em outro computador.

```bash
sudo apt install firmware-linux-nonfree firmware-realtek firmware-iwlwifi
sudo modprobe -r iwlwifi ; sudo modprobe iwlwifi
```

## Drivers de Vídeo

### Intel/AMD:
```bash
sudo apt install firmware-amd-graphics firmware-misc-nonfree
```

### NVIDIA (proprietário):
```bash
sudo apt install nvidia-driver
sudo reboot
```

## Outros drivers

- Consulte a documentação do fabricante ou o wiki do Debian para casos específicos:
  [https://wiki.debian.org/Hardware](https://wiki.debian.org/Hardware)