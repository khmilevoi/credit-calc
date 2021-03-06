# Тестовое Задание
## Кредитный калькулятор

### Требования к стеку технологий
- TypeScript, React, axios, moment.js

### Ресурсы
[API для условий калькулятора](https://api.test.l-l.cloud/v2/conditions)
Пример ответа:
```json
{
  "amount": {
    "min": 500,
    "max": 10000,
    "limit": 3000
  },
  "term": {
    "min": 1,
    "max": 30
  },
  "interestRate": 0.0198
}
```

### Требования к функционалу
Необходимо сделать калькулятор с 2 параметрами (сумма и срок кредита).
Для каждого параметра необходимо предусмотреть редактирование посредством:
- поле для ввода (numeric input)
- пользовательский ползунок (range slider)
  
Калькулятор должен автоматически рассчитывать сумму и дату возврата.  
Сумма кредита должна изменяться шагом в 10 (т.е. ввести сумму 1005 грн. - невозможно).
 
Формулы:
- для расчета суммы возврата: `сумма кредита + сумма кредита * процентная ставка * срок кредита`
- для расчета срока кредита: `текущая дата + срок кредита`


### Примеры выполнения
- [lovilave.com.ua](https://lovilave.com.ua/)
- [credit-pro.com.ua](https://credit-pro.com.ua/)


### Требования к сдаче работы
- в виде GitHub репозитория с инструкцией к запуску

*Можно, но не обязательно: развернутый проект с использованием Github Actions и Github Pages*
