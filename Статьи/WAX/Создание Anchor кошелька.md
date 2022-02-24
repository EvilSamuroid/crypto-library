# Создание кошелька WAX на Anchor
- [видео](https://www.youtube.com/watch?v=fOrnipgcoOU), 
- [статья с картинками](https://telegra.ph/Kak-sozdat-koshelyok-Anchor-bez-telefona-05-19)

Для создания требуется уже существующий WAX аккаунт и 0.4 WAX.

Алгоритм создания кошелька:
1. wax.bloks.io -> wallet -> utilities -> [keys](https://wax.bloks.io/wallet/utilities/keys)    Генерируем публичный и приватный ключи и сохраняем.
2. wax.bloks.io -> wallet -> utilities -> [format keys](https://wax.bloks.io/wallet/utilities/format-keys)    
Форматируем ключи и сохраняем.
3. wax.bloks.io -> wallet -> [create-account](https://wax.bloks.io/wallet/create-account)
4. Создаём аккаунт:
— ***New account to create***
имя аккаунта, строго 12 символов
— ***New Accounts Public Owner Key***
отформатированный публичный ключ
— ***New Accounts Public Active Key***
снова отформатированный публичный ключ
— ***NET to Stake for New Account*** (in WAX)
— ***CPU to Stake for New Account*** (in WAX)
— ***RAM to buy for New Account*** (in Bytes)
5. Скачиваем кошелёк Anchor ([Windows](https://greymass.com/en/anchor/download), [IOS](https://greymass.com/en/anchor/download), [Android](https://play.google.com/store/apps/details?id=com.greymass.anchor&hl=en_US&gl=US))
6. Придумываем пароль (вводится будет часто).
7. Anchor Wallet -> WAX Wallet -> import an existing account -> import a private key
    Импортируем отформатированный приватный ключ