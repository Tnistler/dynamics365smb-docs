# Отчеты по расчетам с клиентами (Россия)

Функция отчетов о расчетах с клиентами позволяет создавать оборотную ведомость финансовых операций клиента для финансовых операций финансовых счетов с типом источника Клиент. Предоставляются также следующие отчеты:

- Клиенты оборотная ведомость по ГК (отчет 12450)
- Клиент Бухг. Карточка (отчет 12441)
- Оборотная ведомость по клиентам (отчет 12439)
- Оборот по учетной группе клиентов (отчет 12440)
- Анализ Операций Клиента (отчет 12442)
- Клиент - Акт Выверки Упрощенный (отчет 14910)

## Клиенты оборотная ведомость по ГК(отчет 12450)

Отчет **Клиенты оборотная ведомость по ГК** используется для анализа оборотной ведомости, а также для анализа сальдо счета клиента. Отчет обычно печатается ежемесячно, но может быть напечатан за любой выбранный период.

Экспресс-вкладка **Параметры** содержит поля, приведенные в следующей таблице.

| Поле                                      | Описанием                                                    |
| ----------------------------------------- | ------------------------------------------------------------ |
| **Точность округления**                   | Выберите это поле, чтобы выбрать нужную точность округления, например: 0,001; 0,01; 1 или 1000. |
| **Заменять нулевые значения на пропуски** | Выберите это поле, чтобы заменять нулевые значения пробелами при печати. |
| **Пропускать нулевые строки**             | Выберите это поле, чтобы исключить строки с нулевыми значениями. |
| **Печать по договорам**                   | Если выбран, все суммы в отчетах будут рассчитываться и отображаться в разделах по договорам. |

## Клиент Бухг. Карточка (отчет 12441)

В отчете **Бухг. карточка клиента** предоставляются следующие сведения обо всех операциях клиента за определенный период:

- Начальное Сальдо
- Дата Учета
- Документ Но.
- Описанием
- Оборот Дебет
- Оборот Кредит
- Тип документа
- Конечное Сальдо

Отчет обычно печатается ежемесячно и на дату инвентаризации, но может быть напечатан за любой выбранный период.

Следующая процедура показывает, как получить доступ к отчету **Бухг. карточка клиента**.

1. Перейдите в **Клиенты оборотная ведомость по ГК**, выберите действие **Отчет**, затем выберите действие **Бухг. карточка клиента**.

На экспресс-вкладке **Параметры** можно установить флажок **Новая страница для клиента**, чтобы информация по каждому клиенту была напечатана на отдельном листе.

## Оборотная ведомость по клиентам (отчет 12439)

Отчет **Оборотная ведомость по клиентам** используется для печати данных об операциях клиента за определенный период. Печатаемые данные включают:

- Код
- Описание
- Начальное Сальдо (дебет или кредит на начало периода)
- Оборот (дебет или кредит)
- Конечное Сальдо (дебет или кредит на конец периода)

Для доступа к отчету:

Выберите значок ![Поиск страницы или отчета](https://github.com/DianaMalina/dynamics365smb-docs/blob/live/business-central/LocalFunctionality/Russia/1.png), введите **Оборотная ведомость по клиентам**, а затем выберите связанную ссылку.

Экспресс-вкладка **Параметры** содержит поля, приведенные в следующей таблице. 

| Поле                                           | Описанием                                                    |
| :--------------------------------------------- | :----------------------------------------------------------- |
| **Точность округления**                        | Выберите это поле, чтобы выбрать нужную точность округления, например: 0,001; 0,01; 1 или 1000. |
| **Заменять нулевые значения на пропуски**      | Выберите это поле, чтобы заменять нулевые значения пробелами при печати. |
| **Пропускать счета без оборотов**              | Выберите это поле, чтобы исключить строки, не имеющие оборота за указанный период. |
| **Пропускать счета с нулевым конечным сальдо** | Выберите это поле, чтобы исключить строки с нулевым конечным сальдо на конец периода. |
| **Пропускать нулевые строки**                  | Выберите это поле, чтобы исключить строки с нулевыми значениями. |

## Оборот по учетной группе клиентов (отчет 12440)

Отчет **Оборотная ведомость по учетной группе клиента** используется для печати сведений об операциях клиентов, которые собираются для учетных групп клиентов. Печатаемые данные включают:

- Код учетной группы клиента
- Название учетной группы клиента
- Начальное Сальдо (дебет или кредит)
- Оборот (дебет или кредит)
- Конечное Сальдо (дебет или кредит)

Для доступа к отчету:

Выберите значок ![Поиск страницы или отчета](https://github.com/DianaMalina/dynamics365smb-docs/blob/live/business-central/LocalFunctionality/Russia/1.png), введите **Оборот по учетной группе клиентов**, а затем выберите связанную ссылку.

На экспресс-вкладке **Параметры** имеется возможность указать те же параметры форматирования, что и на экспресс-вкладке **Параметры** отчета **Оборотная ведомость по клиентам**.

## Анализ Операций Клиента (отчет 12442)

В отчете **Анализ операций клиента** указываются обязательства клиента на начало и конец периода, анализ операции и выплата счета. Печатаемые данные включают:

- Дата Учета
- Документ Но.
- Документ Название
- Тип (оплата, счет)
- Сумма
- Сумма Закрытия
- Дата Оплаты

В этом отчете отображаются все операции клиента за определенный период. Анализ данного отчета позволяет определить взаимозависимость счета и оплаты, а также показывает закрытые операции, счета для оплаты, частично выплаченные счета и суммы предоплаты клиентов.

Для доступа к отчету:

Выберите значок ![Поиск страницы или отчета](https://github.com/DianaMalina/dynamics365smb-docs/blob/live/business-central/LocalFunctionality/Russia/1.png), введите **Анализ операций клиента**, а затем выберите связанную ссылку.

На экспресс-вкладке **Параметры** имеется возможность указать параметры форматирования, приведенные в следующей таблице.

| Параметр                       | Описанием                                                    |
| ------------------------------ | ------------------------------------------------------------ |
| **Дата начала**                | Введите дату начала периода.                                 |
| **Дата окончания**             | Введите дату окончания периода.                              |
| **Валюта Отчета**              | Введите валюту для использования в отчете. Можно выбрать следующие типы:   -   Местная валюта -   Валюта транзакции |
| **Новая страница для Клиента** | Выберите это поле, чтобы напечатать данные для каждого клиента на отдельной странице. |

## Клиент - Акт Выверки Упрощенный (отчет 14910)

В отчете **Клиент - акт выверки** указываются платежи и обязательства клиента. Он используется для сверки взаимных оплат контрагентов.

Для доступа к отчету:

Выберите значок ![Поиск страницы или отчета](https://github.com/DianaMalina/dynamics365smb-docs/blob/live/business-central/LocalFunctionality/Russia/1.png), введите **Клиент - акт выверки упрощенный**, а затем выберите связанную ссылку.

Возможные уровни подробностей:

- Полностью
- Частично
- Нет

### Все подробности

Если выбран уровень Все подробности, отчет печатает следующие данные для каждого документа за текущий и предыдущий периоды:

- Номер документа и номера связанных с ним документов.
- Сальдо для каждого документа (дебет или кредит)
- Дата Документа
- Описанием

### Частичные подробности

Если выбран уровень частичных подробностей, отчет отображает сальдо для каждого документа за текущий и предыдущий периоды, но не отображает связи со счетами, кредит-нотами и оплатами.

### Нет

Если выбрано значение Нет, отчет отображает для каждого клиента начальное сальдо, оборот за период, а также сальдо на конец периода. Он показывает также сумму обязательств клиента.

На экспресс-вкладке **Клиент** страницы запроса определите номер или диапазон номеров клиентов, в зависимости от того, нужно ли печатать отчет для одного или для нескольких клиентов.

На экспресс-вкладке **Параметры** имеется возможность указать параметры форматирования, приведенные в следующей таблице.

| Параметр                   | Описанием                                                    |
| -------------------------- | ------------------------------------------------------------ |
| **Дата начала**            | Введите дату начала периода.                                 |
| **Дата Окончания Периода** | Введите дату окончания периода.                              |
| **Код валюты**             | Введите валюту для использования в отчете. Имеется возможность выбрать любую валюту из списка валют. |
| **Подробно**               | Выберите один из следующих вариантов:   -   **Все**; -   **Частично**; -   **Нет** |

## См. также

[Отчеты по платежам (Россия)](https://github.com/DianaMalina/dynamics365smb-docs/blob/live/business-central/LocalFunctionality/Russia/russian-payables-reports.md)

[Практическое руководство. Настройка договоров с клиентами и поставщиками](https://github.com/DianaMalina/dynamics365smb-docs/blob/live/business-central/LocalFunctionality/Russia/how-to-set-up-customer-and-vendor-agreements.md)
