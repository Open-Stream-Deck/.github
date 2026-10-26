<div align="center">

# Open Stream Deck

Открытая замена фирменному софту для макропанелей Ajazz и Mirabox.
Своя прошивка, своё приложение, свои плагины.

[Сайт](https://opensd.dev) · [Документация](https://wiki.opensd.dev) · [Скачать](https://github.com/Open-Stream-Deck/Open-Stream-Deck-App/releases/latest) · [SDK](https://wiki.opensd.dev/docs/sdk)

</div>

## Как это устроено

Дека  ->  прошивка OSD  ->  приложение  ->  плагины

На деку ставится наша прошивка, приложение управляет клавишами, страницами, профилями и виджетами, а плагины добавляют новые действия. Плагин занимает один файл `.opensd`, а писать его можно на Rust, JavaScript, TypeScript или любом языке, который собирается в WebAssembly.

## Репозитории

| Репозиторий | Что внутри |
| --- | --- |
| [Open-Stream-Deck-App](https://github.com/Open-Stream-Deck/Open-Stream-Deck-App) | Приложение для Windows, macOS и Linux. Само ставит прошивку на деку |
| [Firmware-AjazzAKP153R](https://github.com/Open-Stream-Deck/Firmware-AjazzAKP153R) | Прошивка для AJAZZ AKP153R: 15 клавиш, дисплей 480 x 854, поток около 3,8 МБ/с |
| [Firmware-Requests](https://github.com/Open-Stream-Deck/Firmware-Requests) | Готовые прошивки и запросы на поддержку новых моделей |
| [Open-Stream-Deck-SDK](https://github.com/Open-Stream-Deck/Open-Stream-Deck-SDK) | SDK и CLI для плагинов: [crates.io](https://crates.io/crates/opensd), [npm](https://www.npmjs.com/package/@opensd/cli) |
| [Open-Stream-Deck-Wiki](https://github.com/Open-Stream-Deck/Open-Stream-Deck-Wiki) | Исходники [wiki.opensd.dev](https://wiki.opensd.dev) |

## Поддерживаемые деки

Сейчас поддерживается AJAZZ AKP153R. Если у вас другая модель, оставьте запрос в [Firmware-Requests](https://github.com/Open-Stream-Deck/Firmware-Requests/issues).

## Участие

Баги и предложения пишите в issues нужного репозитория. Чтобы написать свой плагин, начните с [руководства по SDK](https://wiki.opensd.dev/docs/sdk).

## Лицензии

Приложение и прошивка распространяются под [Open Stream Deck Noncommercial License 1.0](https://github.com/Open-Stream-Deck/Open-Stream-Deck-App/blob/main/LICENSE). Их можно бесплатно использовать, изучать, менять и распространять, но только в некоммерческих целях и с указанием автора (whxtelxs). Продавать код, продавать деки с прошивкой и строить на этом платные сервисы можно только по отдельной лицензии, запросы пишите на git@opensd.dev.

SDK и Firmware-Requests выпущены под MIT или Apache 2.0 на ваш выбор, вики под MIT. Плагин на SDK можно лицензировать как угодно, в том числе продавать.
