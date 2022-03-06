# Как ловить неуловимые дропы c AtomicHub через atomicdropsx
  - [Статья с картинками](http://vk.com/@cheapchill-lovim-paki-bez-kapchi) 
  - [Видео](https://youtu.be/hIxZXdsB_Ic)
  - Это оригинальная статья.
---
  
## Проверяем, есть ли на дропе капча
Мы не можем брать дропы с капчей через этот сервис, поэтому пользуемся следующими способами проверки наличия капчи:
- У дропов по вайтлисту или с приватным ключом (значение key=... в адресной строке) никогда нет капчи.
- Переводим время и смотрим, есть ли капча.
- На странице сейла: правая кнопка мыши -> показать код -> network -> обновить страницу -> смотрим, есть ли файл keys:
          Если есть, то: делаем попытку взять дроп через (пункт 6: *Клаймим дроп*) atomicdropsx -> Contract -> Actions -> [claimdrop](https://wax.bloks.io/account/atomicdropsx?loadContract=true&tab=Actions&table=drops&account=atomicdropsx&scope=atomicdropsx&limit=100&lower_bound=54387&upper_bound=54387&action=claimdrop) и смотрим на ошибку:
		  Если вылезла ошибка *Drops that require auth need to be claimed with specialized actions*, то на дропе присутствует капча или вайтлист.

## Пополняем баланс atomicdropsx
Дроп берется с баланса привязанного к нашему адресу кошелька atomicdropsx. Пополняем этот кошелек:
1. Идём на [atomicdropsx](https://wax.bloks.io/account/atomicdropsx?loadContract=true&tab=Actions&account=atomicdropsx&scope=atomicdropsx&limit=100&table=drops&action=claimdrop) и логинимся через WAX кошелёк.
2. Отсылаем с того же кошелька нужное кол-во WAX на кошелек *atomicdropsx*, а там, где *memo*, вписываем *deposit*.

## Проверяем баланс
atomicdropsx -> Contract -> Tables -> [balances](https://wax.bloks.io/account/atomicdropsx?loadContract=true&tab=Tables&account=atomicdropsx&scope=atomicdropsx&limit=100&table=balances&action=claimdrop): в поля *Lower Bound* и *Upper Bound* вписываем свой WAX адрес и делаем *Refresh*.

## Получаем всю информацию о дропе
1. Переходим на страницу дропа и копируем *id дропа*.
2. atomicdropsx -> Contract -> Tables -> [drops](https://wax.bloks.io/account/atomicdropsx?loadContract=true&tab=Tables&account=atomicdropsx&scope=atomicdropsx&limit=100&table=drops&action=claimdrop).
3. В поля *Lower Bound* и *Upper Bound* вписываем *id дропа* и делаем *Refresh*.

## Убираем окно подтверждения у дропа
atomicdropsx -> Contract -> Actions -> [assertdrop](https://wax.bloks.io/account/atomicdropsx?loadContract=true&tab=Actions&table=drops&account=atomicdropsx&scope=atomicdropsx&limit=100&lower_bound=54387&upper_bound=54387&action=assertdrop)    Заполняем соответствующие поля информацией о дропе и нажимаем Submit Transaction:
— ***drop_id***
— ***assets_to_mint_to_assert***  
то, что в квадратных скобках, включая сами скобки.
— ***listing_price_to_assert***     
Цена следующего формата:
            x.xxxxxxxx WAX
            х.хх USD
— ***settlement_symbol_to_assert***
8,WAX

## Клаймим дроп
atomicdropsx -> Contract -> Actions -> [claimdrop](https://wax.bloks.io/account/atomicdropsx?loadContract=true&tab=Actions&table=drops&account=atomicdropsx&scope=atomicdropsx&limit=100&lower_bound=54387&upper_bound=54387&action=claimdrop) (*claimdropwl*, если дроп по вайтлисту)
Заполняем соответствующие поля информацией о дропе, полученной на прошлом шаге, и нажимаем *Submit Transaction*:
— ***claimer*** 
адрес WAX, с которого совершён вход.
— ***drop_id***
— ***claim_amount*** 
кол-во NFT.
— ***intended_delphi_median*** 
Если у дропа фиксированная цена в WAX: 0
Если в USD: постоянно меняется, поэтому смотрим тут delphioracle -> Tables -> [datapoints](https://wax.bloks.io/account/delphioracle?loadContract=true&tab=Tables&table=datapoints&account=delphioracle&scope=waxpusd&limit=1): значение *median*.
— ***referrer***  
*atomichub*
— ***country***  
*Rus*

## Выводим деньги
atomicdropsx -> Contract -> Actions -> [withdraw](https://wax.bloks.io/account/atomicdropsx?loadContract=true&tab=Actions&account=atomicdropsx&scope=atomicdropsx&limit=100&table=balances)    
Заполняем соответствующие поля и нажимаем Submit:
— ***owner*** 
Адрес WAX.
— ***token_to_withdraw***
Кол-во токенов следующего формата: *x.xxxxxxxx WAX*.