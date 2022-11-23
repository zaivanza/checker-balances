# checker-balances

скрипт проверяет баланс монет почти во всех сетях. исключение : arbitrum nova и те сети, где нет верифнутых контрактов. основные сети есть, все в порядке. не смотрит баланс в пулах, в протоколах и стейкинге. то есть чекер только тех монет, которые доступны на балансе. 

1. в файл ass.txt добавляем адреса или приватники кошельков, и так и так сработает.
2. в массив data добавляем те монеты, которые хочешь спарсить. сейчас добавлены стейблы и некоторые нужные мне монеты. 

инструкция по добавлению новых монет :
1. заходим coinmarketcap, выбираем монету, заходим в scan. например ты выбрал DAI в сети ethereum : https://etherscan.io/token/0x6b175474e89094c44da98b954eedeac495271d0f
2. нам нужно 4 значения : decimals, symbol, address и abi.
- decimals : https://pastenow.ru/9e144874ed8f82e52a9ac0d48b672cb5
- address : нажимаем на contract (выше decimals), копируем это : https://pastenow.ru/d528e413a088802c1396e6aaf4dffcda
- abi : нажимаем contract (https://pastenow.ru/4bfb542ec81cb5b5fa5dbafdbea884e7), листаем страницу code вниз и копируем значение Contract ABI : https://pastenow.ru/482134091dd7f9c06f12513c1b843aa8

эти значения вписываем в массив data в файле main.py.

с вами был админ паблика https://t.me/hodlmodeth, отправитель редких гемов в [ chat ] = http://t.me/chathodlmodeth и главный, но не самый умный кодер чата [ code ] = https://t.me/code_hodlmodeth. все вопросы по кодингу туда.
