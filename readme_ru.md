**⭐Запросы на вытягивание или любые формы вклада будут признательны⭐**

# SpoofDPI

Можете прочитать на других языках: [🇬🇧English](https://github.com/xvzc/SpoofDPI), [🇰🇷한국어](https://github.com/xvzc/SpoofDPI/blob/main/readme_ko.md), [🇨🇳简体中文](https://github.com/xvzc/SpoofDPI/blob/main/readme_zh-cn.md), [🇷🇺Русский](https://github.com/xvzc/SpoofDPI/blob/main/readme_ru.md)

Простое и быстрое программное обчеспечение, созданное для обхода **Deep Packet Inspection**  
  
![image](https://user-images.githubusercontent.com/45588457/148035986-8b0076cc-fefb-48a1-9939-a8d9ab1d6322.png)

# Установка
## Бинарник
SpoofDPI будет автоматически установлен в директорию `~/.spoof-dpi/bin`.  
Для запуска SpoofDPI в любой директории добавьте строку ниже к Вашему `~/.bashrc || ~/.zshrc || ...`
```
export PATH=$PATH:~/.spoof-dpi/bin
```

### curl
Установите последний бинарник с помощью curl
- OSX
```
curl -fsSL https://raw.githubusercontent.com/xvzc/SpoofDPI/main/install.sh | bash -s osx
```
- Linux
```
curl -fsSL https://raw.githubusercontent.com/xvzc/SpoofDPI/main/install.sh | bash -s linux
```
### wget
Установите последний бинарник с помощью wget
- OSX
```
wget -O - https://raw.githubusercontent.com/xvzc/SpoofDPI/main/install.sh | bash -s osx 
```
- Linux
```
wget -O - https://raw.githubusercontent.com/xvzc/SpoofDPI/main/install.sh | bash -s linux 
```
## Go
Вы также можете установить SpoofDPI с помощью **go install**  
`$ go install github.com/xvzc/SpoofDPI/cmd/spoof-dpi`  
  > Не забудьте, что $GOPATH должен быть установлен в Вашем $PATH

## Git
Вы также можете собрать SpoofDPI
`$ git clone https://github.com/xvzc/SpoofDPI.git`  
`$ cd SpoofDPI`  
`$ go build ./cmd/...`  

# Употребление
```
Usage: spoof-dpi [options...]
--addr=<addr>       | default: 127.0.0.1
--dns=<addr>        | default: 8.8.8.8
--port=<port>       | default: 8080
--debug=<bool>      | default: false
--banner=<bool>     | default: true
--url=<url>         | Can be used multiple times. If set, 
                    | it will bypass DPI only for this url. 
                    | Example: --url=google.com --url=github.com
--pattern=<regex>   | If set, it will bypass DPI only for packets 
                    | that matches this regex pattern.
                    | Example: --pattern="google|github"
```
**Перевод:**
```
Употребление: spoof-dpi [параметры...]
--addr=<адрес>       | Адрес. По умолчанию 127.0.0.1
--dns=<адрес>        | Адрес DNS-сервера. По умолчанию 8.8.8.8
--port=<порт>        | Порт. По умолчанию 8080
--debug=<булев>      | Включать ли режим отладки. По умолчанию false
--banner=<булев>     | По умолчанию true
--url=<url>          | Можно использовать несколько раз. Если 
					 | задано, будет применятся
					 | обход только для данного url.
					 | Пример: --url=google.com --url=github.com
--pattern=<regex>    | Если задано, будет применятся обход
                     | только для пакетов, которые соответствуют
                     | этому регулярному выражению.
					 | Пример: --pattern="google|github"
```
> Если Вы используете любые vpn-расширения по типу Hotspot Shield в браузере  
  Chrome, зайдите в Настройки > Расширения и отключите их.

### OSX
Выполните `$ spoof-dpi`, и прокси автоматически установится

### Linux
Выполните `$ spoof-dpi` и откройте свой любимый браузер с параметром прокси
`google-chrome --proxy-server="http://127.0.0.1:8080"`

# Как он работает
### HTTP
Т. к. большинство веб-сайтов в мире уже поддерживают HTTPS, SpoofDPI не делает обход Deep Packet Inspection для HTTP-запросов. Однако он всё же предоставляет прокси-соединение для всех HTTP-запросов.

### HTTPS
 Несмотря на то, что TLS 1.3 шифрует каждый процесс рукопожатия, имя доменов всё же отображаются как простой текст в пакете приветствия клиента. 
 В других словах, если кто-то другой посмотрит на пакет, они могут с лёгкостью узнать, куда направлен пакет. 
 Имя домена может предоставить много значимой информации пока DPI обрабатывается, и мы видим, что соединение блокируется сразу после отправки пакета приветствия клиента.
 Я уже пробовал многие способы для обхода этого и узнал, что, видимо, обрабатывается только первый кусок, когда мы отправляем пакет приветствия клиента, разделенный на куски. 
 Чтобы обойти это, SpoofDPI отправляет первый 1 байт запроса к серверу, 
 и затем уже отправляет все остальные.
 > SpoofDPI не расшифровывает Ваши HTTPS-запросы, так что нам не нужны SSL-сертификаты.

# Вдохновлено
[Green Tunnel](https://github.com/SadeghHayeri/GreenTunnel) от @SadeghHayeri  
[GoodbyeDPI](https://github.com/ValdikSS/GoodbyeDPI) от @ValdikSS