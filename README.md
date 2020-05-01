# Отчёт о тестировании приложения "Money Transfer"

## Краткое описание

Проверка текущей суммы счета клиента переменная типа int (2_000_000_000 (два миллиарда рублей)) + сумма перевода переменная типа int (500_000_000) итоговое значение должно быть в переменная типа int

## Описание тестов
Проводилось функциональное тестирование проверка пополнение счета клиента
*  Набор тест кейсов:
	1) Создать новый проект с помощью inteleger idea
	2) Создать переменную balance тип int и присвоить ей значение (2_000_000_000)
	3) Создать переменную transfer тип int и присвоить ей значение (500_000_000)
	4) Создать переменную total тип int и присвоить ей значение суммы (balance + transfer)
	Ожидаемый результат сумма запишется корректно
	Фактический результат Число записано не корректно
	
	Скриншот:
	[Скриншот](https://ibb.co/RpKjYFM)

## Результаты

* % успешных тестов 0%/не успешных тестов 100%
* [Ссылки на баг-репорты](https://github.com/Oleg2394/Money-Transfer/issues/1#issue-610678124)

## Общие рекомендации
Перевести переменные:
balance
transfer
total
К типу переменной long

[Скриншот](https://ibb.co/bJ4mjBq)

Так как в переменной типа int не может хранится число больше чем 2_147_483_647;

Тестирование производилось в следующем окружении:
* <Windows 64-bit версия 1909>
* <Java 11.0.7>

