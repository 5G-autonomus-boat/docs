# Startowa konfiguracja
## Login
Uzytkownik: admin
Haslo: 123
## Moduł GSM
- Interfejs wwan0
- 

## Programy 
- MavProxy
Skonfigurować virtual environment 
```shell
python -m venv ./mavproxy
cd mavproxy/
source bin/activate
```
```shell
sudo apt-get install python3-dev python3-opencv python3-wxgtk4.0 python3-pip python3-matplotlib python3-lxml python3-pygame
pip3 install PyYAML mavproxy --user
echo 'export PATH="$PATH:$HOME/.local/bin"' >> ~/.bashrc
```

Uruchomienie mavproxy
```shell
mavproxy.py --master=mavlink serial port --baudrate 115200 --out ip:14550
```

Skrypcik
```shell
#!/bin/bash
cd /home/admin/mavproxy/
source bin/activate
mavproxy.py --master=/dev/ttyS0  --out $1:14550
```