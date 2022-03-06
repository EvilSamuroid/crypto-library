# Инструкция по созданию фермы аккаунтов без прокси на бесплатном антидетект-браузере SWITCH
- Это оригинальная статья.
---

## Преимущества SWITCH перед Google Chrome
Создание фермы на бесплатном антидетект-браузер SWITCH имеет несколько преимуществ, которые делают держание фермы в профилях обычного Google Chrome бессмысленным.

-> [Все о покупке аккаунтов для фермы](Абузы%20и%20мультиакинг.md).

##### Удобство хранения и способа запуска аккаунтов
Держание фермы аккаунтов в виде профилей Google Chrome имеет следующий недостаток: основные рабочие профиля смешиваются с профилями фермами, что неудобно. К тому же в Google Chrome не показывается, какие профили уже запущены, a массовый запуск немного трудозатратнее, чем в антидетект-браузере, где можно просто проклацать кнопки запуска.

##### Клонирование профилей
Клонирование профилей Google Chrome сложнее, чем в антидетект-браузере. Это производится посредством копирования папки с профилем, которая по каким-то копируется безмерно долго. 

В антидедект-браузере клонирование происходит всего несколько секунд с помощью нажатия одной кнопки.

##### Функции антидетект-браузера, как приятный бонус
Хоть мы и не задействуем возможности антидетект-браузера на полную (использование прокси и подмена отпечатков), никто не запрещает использовать их в будущем и вывести ферму на новый уровень.

##### Сохранение профилей
Очень удобно, что мы можем импортировать наши профили и экспортировать их в любой момент для работы на другом компьютере.



## Установка SWITCH
- Регистрируемся на [официальном сайте разработчика mybot.su](http://mybot.su/register.php):
![](_attachments/fc5670ddbd9af6536f0f206515745ea7.png)
- [Скачиваем SWITCH с официального сайта](http://mybot.su/switch):
![](_attachments/4d5d7f6c3c35e7c9a743b2086b7ffe0c.png)
- Устанавливаем на компьютер и логинимся.

Программа распространается бесплатно и имеет закрытый код, а я не могу ручаться за ее безопасность. Берегите свои данные!



## Настройка профиля-заготовки
Нам нужно сделать эталонный профиль, который мы далее будем клонировать и заполнять данными фермы.

### Создаем профиль
Создаем профиль. В полях, относящихся к антидетект-настройкам, ставим нормальный режим, ведь наc не интересуют эти функции и мы не используем прокси:
![](_attachments/28eebc338d8cfdda94c0d6c5aaf37247.png)

Запускаем профиль. Можно указать имя пользователя профиля, совпадающее с названием профиля в списке профилей антидетект-браузера:
![](_attachments/7709a3dd061cb9a5ef2469710bcf8d25.png)

### Закладки
Закрепляем нужные закладки:
    - [Chainlist](https://chainlist.org/)
	- [Discord](https://discord.com/channels/@me)
	- [Twitter](https://twitter.com/home)
	- [Почта Маил](https://account.mail.ru/login)
	- [Почта Рамблер](https://mail.rambler.ru/)	
![](_attachments/4ef1c32cae3db5285580c13d09b25113.png)


### Расширения
Устанавливаем нужные расширения:
![](_attachments/5df94295a8fab8dbd8587d22e3bcaa3d.png)
    - [Metamask](https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn)
    - [Phantom wallet](https://chrome.google.com/webstore/detail/phantom/bfnaelmomeimhlpmgjnjophhpkkoljpa)
    - [Dark Reader](https://chrome.google.com/webstore/detail/dark-reader/eimadpbcbfnmbkopoojfekhnkhdbieeh) (темная тема)
    - [uBlock Origin](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm) (блокировка рекламы)
    - [DuckDuckGo](https://chrome.google.com/webstore/detail/duckduckgo-privacy-essent/bkdgflcldnnnapblkhphbgpggdiikppg)
    - [Google Переводчик](https://chrome.google.com/webstore/detail/google-translate/aapbdbdomjkkjkaonfhkkikfgjllcleb)
	
#### Антикапча
Антикапча поможет нам каждый раз не решать сотню капч вручную при открытии сотни профилей:
    - В первую очередь [регистрируемся на сайте](https://anti-captcha.com/clients/entrance/login) и вносим средства для оплаты решения капч.
	- Скачиваем [ZIP-расширение с официального сайта](https://antcpt.com/rus/download/google-chrome-options/manual-zip.html):
	![](_attachments/77da0ffa6095108b09f82265c0ac8a6e.png)
	- Распаковываем архив в папку:
	![](_attachments/64acfdafa5537196a3881ff94bd57e35.png)
	- Переходим в управление расширениями:
	![](_attachments/d903da8aae232c7dcb2fc6b375081047.png)
	- Включаем режим разработчика и загружаем распакованное расширение:
	![](_attachments/5a493da3d4c292e68979f5b48e20dd3e.png)
	- Переходим в [аккаунт AntiCaptcha -> settings -> API setup](https://anti-captcha.com/clients/settings/apisetup) и копируем API-ключ:
    ![](_attachments/9766339935934ae405f42a65af8efbc7.png)
	- Переходим в настройки расширения AntiCaptcha и вставляем в полу скопированный ключ, нажимаем сохранить:
	![](_attachments/8fe0eb09ef9142e676ec6d9449649309.png)


## Создание фермы
- Остается только клонировать профиль-заготовку, задать ему номер, зайти в него и войти в нужные аккаунты и кошельки:
![](_attachments/a1b273da7c047ae64f3cb5e3ff1e0b18.png)

- Заранее добавляем в метамаск нужные сети с помощью [chainlist](https://chainlist.org/):
    - Binance Smart Chain
    - Polygon
![](_attachments/774275c01f97da13e18c4f2c48c0d5a1.png)
- Заранее добавляем в метамаск нужные токены с помощью [coinmarketcap](https://coinmarketcap.com/):
    - [busd](https://coinmarketcap.com/currencies/binance-usd/)
    - [usdt](https://coinmarketcap.com/currencies/tether/)
    - [usdc](https://coinmarketcap.com/currencies/usd-coin/)
![](_attachments/6e85f173051c8905b0afbd8b72f4d5c7.png)