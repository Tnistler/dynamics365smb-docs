# Практическое руководство. Настройка секций налогового регистра

Можно создать новую секцию налогового регистра или выбрать секцию налогового регистра, которая будет использоваться в организации в текущем налоговом периоде. Можно выбрать секцию налогового регистра, действовавшую в одном из предыдущих налоговых периодов и просмотреть налоговую информацию за любой из периодов. Имеется возможность копирования налоговых регистров из одной секции налоговых регистров в другую. Это позволяет настраивать налоговые регистры и отлаживать алгоритм сбора информации в налоговые регистры.

Ниже приводится процедура настройки секций налогового регистра.

## Настройка налогового регистра

1. Выберите значок ![Поиск страницы или отчета](https://github.com/DianaMalina/dynamics365smb-docs/blob/live/business-central/LocalFunctionality/Russia/1.png), введите **Налоговые регистры**, а затем выберите связанную ссылку.

2. В окне **Секции налоговые регистров**, выберите действие **Создать**.

3. На экспресс-вкладке **Общее** введите значения в поля, описанные в следующей таблице.

   | Поле               | Описанием                                                    |
   | ------------------ | ------------------------------------------------------------ |
   | **Код**            | Отображается код имеющейся версии налогового регистра для определенного налогового периода.   Создайте код для новой секции налогового регистра, если необходимо. |
   | **Описание**       | Введите описание секции налогового регистра.                 |
   | **Статус**         | Это поле может содержать одно из следующих значений:   -   **Заблокировано** -   **Открытые** -   **Отчеты** -   **Закрыто**   Статус **Блокировка** устанавливается по умолчанию при создании новой секции. Он указывает, что новая секция налогового регистра создана и что регистр не содержит данных.   Чтобы продолжить настройку, измените статус на **Открыт вручную**. При использовании этого статуса во время расчета и перерасчета налогового регистра нельзя проверить доступность данных предыдущего и следующего налоговых периодов. Непрерывность создания налоговых регистров в текущем периоде не контролируется. Этот статус позволяет включить отладку точности расчета налогового регистра.   При статусе **Отчеты** непрерывность создания налоговых данных контролируется. Это рабочий режим модуля Налоговый учет. При использовании этого статуса должна изменяться только конечная дата.   Статус **Закрыто** указывает, что налоговый период закрыт. Этот статус может быть установлен после того, как будут созданы все налоговые регистры для налогового периода. |
   | **Дата начала**    | Введите дату начала для секции налогового регистра.          |
   | **Дата окончания** | Введите дату окончания для секции налогового регистра.       |

4. На экспрес-вкладке **Измерения** введите коды измерений для фильтрации информации, выбранной для налоговых регистров. Коды измерений могут быть изменены только в том случае, если в поле **Статус** установлено значение **Открыто**.

5. На экспресс-вкладке **Сальдо** введите сроки для обязательств дебиторов и кредиторов, используемые в соответствии с текущим налоговым периодом. Например, Дебетовое сальдо - точка 1 = 45Д, Дебетовое сальдо - точка 2 = -90Д.

6. На экспресс-вкладке **Система** выберите код действующей нормы для текущей версии налогового регистра в поле **Код нормы юрисдикции**. Выберите номер формы **17209** в поле **Форма ID**.

   Нажмите кнопку **ОК**.

7. В окне **Секции налоговые регистров**, выберите действие **Регистры**.

8. В окне **Налог. регистр названия** можно добавить в список новые регистры. Для создания нового налогового регистра выполните одно из следующих действий:

   1. Установите курсор в пустую строку в конце списка регистров и введите данные нового регистра.
   2. Установите курсор на регистр, после которого должен быть создан новый регистр. Нажмите клавишу F3 и введите данные нового регистра.

9. Введите значения в поля, описанные в следующей таблице.

   | Поле                   | Описанием                                                    |
   | ---------------------- | ------------------------------------------------------------ |
   | **Номер**              | Введите номер налогового регистра.                           |
   | **Описание**           | Введите наименование налогового регистра.                    |
   | **Метод Формирования** | Выберите тип налогового регистра.   Можно выбрать один из следующих вариантов:   -   Расчет (накопление) -   Операции (создание на основе учтенных финансовых операций) |
   | **Таблица ID**         | Выберите 17208 для налогового регистра с методом формирования "Расчет".   Для налогового регистра с методом формирования "Операции" в зависимости от исходной операции регистра выберите одно из следующих значений: **17209**, **17210**, **17211**, **17212**, **17213**, **17214**. |

Сопоставление исходных операций регистра и кодов таблицы приводится в следующей таблице.

| Значение  | Описанием                                                    |
| --------- | ------------------------------------------------------------ |
| **17209** | Для регистров, созданных на основе операций Главной книги    |
| **17210** | Для регистров, созданных на основе операций клиента и поставщика |
| **17211** | Для регистров, созданных на основе операций с основными средствами и нематериальными активами |
| **17212** | Для регистров, созданных на основе операций товара           |
| **17213** | Для регистров, созданных на основе расходов будущих периодов |
| **17214** | Для регистров, созданных на основе книги операций по зарплате |

Если создается новая версия налогового регистра, окно со списком регистров будет пустым. В этом окне можно вручную ввести все налоговые регистры, которые должны использоваться, или выбрать действие **Копирование секции** в окне **Секция расчета налогового регистра**, и скопировать список регистров с настройками из любой секции налоговых регистров.

В окне **Копирование секции налоговых регистров** введите секцию, из которой требуется скопировать регистр.

Ниже приводится процедура удаления налогового регистра из списка регистров.

## Удаление налогового регистра из списка регистров.

1. Выберите действие **Регистры**, затем выберите **Изменить**, чтобы выбрать карточку регистра.
2. Нажмите кнопку **ОК**.
3. Выберите действие **Удалить**, чтобы удалить регистр из списка регистров.

## См. также

[Налоговый учет](https://github.com/DianaMalina/dynamics365smb-docs/blob/live/business-central/LocalFunctionality/Russia/tax-accounting.md)

[Налоговые регистры](https://github.com/DianaMalina/dynamics365smb-docs/blob/live/business-central/LocalFunctionality/Russia/tax-registers.md)

[Практическое руководство. Создание налоговых регистров](https://github.com/DianaMalina/dynamics365smb-docs/blob/live/business-central/LocalFunctionality/Russia/how-to-create-tax-registers.md)

[Сбор сведений о налоге на прибыль для налоговой декларации](https://github.com/DianaMalina/dynamics365smb-docs/blob/live/business-central/LocalFunctionality/Russia/collecting-profit-tax-information-for-tax-declaration.md)

