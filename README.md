# Tinkoff Invest OpenAPI SDK для Python

Данный проект представляет собой инструментарий на языке Python для работы с OpenAPI Тинькофф Инвестиции, который можно
использовать для создания торговых роботов.

## Начало работы

Для установки SDK необходимо установить библиотеку с помощью pip
```bash
pip install -i https://test.pypi.org/simple/ --extra-index-url=https://pypi.org/simple/ tinkoff-invest-openapi-client
```

Или скачать код из репозитория и запустить скрипт setup.py
```bash
python setup.py install
```

Проверить работу можно скопировав и запустив код из папки examples 

### Где взять токен аутентификации?

В разделе инвестиций вашего [личного кабинета tinkoff](https://www.tinkoff.ru/invest/). Далее:

* Перейдите в настройки
* Проверьте, что функция "Подтверждение сделок кодом" отключена
* Выпустите токен для торговли на бирже и режима "песочницы" (sandbox)
* Скопируйте токен и сохраните, токен отображается только один раз, просмотреть его позже не получится, тем не менее вы
  можете выпускать неограниченное количество токенов

## Ссылки

Документацию непосредственно по OpenAPI можно найти по [ссылке](https://api-invest.tinkoff.ru/openapi/docs/).

[Основной репозиторий с документацией](https://github.com/TinkoffCreditSystems/invest-openapi/) - в нем вы можете задать вопрос в Issues и получать информацию о релизах в Releases.

Если возникают вопросы по данному SDK, нашёлся баг или есть предложения по улучшению, то можно задать его в Issues, либо в [telegram](https://t.me/awethon)

## Проблемы

#### SSL: CERTIFICATE_VERIFY_FAILED
Для MacOS решается выполнением команды
`open "/Applications/Python 3.7/Install Certificates.command"`
в терминале
