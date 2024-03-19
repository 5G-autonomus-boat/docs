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
