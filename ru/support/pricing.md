---
editable: false
---

# Правила тарификации для технической поддержки



{% include [currency-choice](../_includes/pricing/currency-choice.md) %}

Стоимость обслуживания зависит от выбранного тарифного плана. Сетка возможностей всех тарифных планов приведена в разделе [{#T}](overview.md). 

Выбранный тарифный план распространяется на платежный аккаунт и [может быть изменен](overview#change-service-plan) только владельцем платежного аккаунта.

Базовый тарифный план предоставляется всем пользователям {{ yandex-cloud }} бесплатно. Для остальных тарифных планов цена вычисляется с учетом потребления ресурсов за текущий отчетный период (календарный месяц). Чтобы рассчитать стоимость использования, воспользуйтесь [нашим калькулятором](https://cloud.yandex.ru/prices#calculator) или ознакомьтесь со способами расчета в разделах ниже.


{% note info %}

Все цены указаны с НДС. Стоимость технической поддержки рассчитывается после вычета ранее выданных грантов из стоимости потребленных ресурсов.

{% endnote %}

## Базовый {#base}

Базовый тарифный план предоставляется всем пользователям {{ yandex-cloud }} бесплатно. Тариф подходит для домашних и исследовательских проектов.

## Стандарт {#standard}

Тариф <q>Стандарт</q> по сравнению с базовым тарифом позволяет запрашивать у технической поддержки общие рекомендации по архитектуре вашего решения в {{ yandex-cloud }}. Тариф подходит для разработки и пилотирования проектов.

### Стоимость тарифного плана {#standard-price}


{% include [rub.md](../_pricing/support/rub-standard.md) %}




### Пример расчета стоимости {#standard-example}

Вы начали платное потребление 1 марта и подключили поддержку по тарифному плану Стандарт. Ежедневно с вашего лицевого счета будет списываться доля фиксированной стоимости:

>900 ₽ / 31 = 29,0300 ₽

В расчетах:

* 900 ₽ — фиксированная стоимость поддержки за месяц.
* 31 — число дней в марте.

Если к концу отчетного периода вы потратили на ресурсы {{ yandex-cloud }} 60 000 ₽ или меньше, дополнительных начислений не будет. Стоимость поддержки составит 900 ₽.

Если к концу отчетного периода вы потратили на ресурсы {{ yandex-cloud }} больше 60 000 ₽, то с момента превышения порога в 60 000 ₽ ежедневно с вашего лицевого счета будут списываться доли и фиксированной, и дополнительной стоимости.

  Например, вы потратили 60 000 ₽ с 1 по 21 марта, а затем с 22 марта до конца месяца тратили по 1000 ₽ в день.

  Итоговая стоимость составит:

  >900 ₽ + ((60 000 ₽ + 10 × 1000 ₽) − 60 000 ₽) × 12% = 900 ₽ + 10 000 ₽ × 0,12 = 2100 ₽

  В расчетах:

  * 900 ₽ — фиксированная стоимость поддержки за месяц.
  * 60 000 ₽ — сумма потребления с 1 по 21 марта.
  * 10 — количество дней с 22 марта до конца месяца.
  * 1000 ₽ — ежедневная сумма потребления с 22 марта до конца месяца.


## Бизнес {#business}

Тариф <q>Бизнес</q> подходит для бизнес-проектов и по сравнению с базовым тарифом позволяет:

* запрашивать у технической поддержки общие рекомендации по архитектуре вашего решения в {{ yandex-cloud }};
* получать консультации и рекомендации по настройке стороннего ПО, а также по решению проблем совместимости с {{ yandex-cloud }};
* получать рекомендации по устранению проблем с операционными системами и их компонентами.

### Стоимость тарифного плана {#business-price}


{% include [rub.md](../_pricing/support/rub-business.md) %}




### Пример расчета стоимости {#business-example}

Вы начали платное потребление 1 марта и подключили поддержку по тарифному плану Бизнес. Ежедневно с вашего лицевого счета будет списываться доля фиксированной стоимости:

>6000 ₽ / 31 = 193,5500 ₽

В расчетах:

* 6000 ₽ — фиксированная стоимость поддержки за месяц.
* 31 — число дней в марте.

Если к концу отчетного периода вы потратили на ресурсы {{ yandex-cloud }} 60 000 ₽ или меньше, дополнительных начислений не будет. Стоимость поддержки составит 6000 ₽.

Если к концу отчетного периода вы потратили на ресурсы {{ yandex-cloud }} больше 60 000 ₽, но меньше 200 000 ₽, с момента превышения порога в 60 000 ₽ ежедневно с вашего лицевого счета будут списываться доли и фиксированной, и дополнительной стоимости.

  Например, вы потратили 60 000 ₽ с 1 по 21 марта, а затем с 22 марта до конца месяца тратили по 1000 ₽ в день.

  Итоговая стоимость составит:

  >6000 ₽ + ((60 000 ₽ + 10 × 1000 ₽) − 60 000 ₽) × 7% = 6000 ₽ + 10 000 ₽ × 0,07 = 6700 ₽

  В расчетах:

  * 6000 ₽ — фиксированная стоимость поддержки за месяц.
  * 60 000 ₽ — сумма потребления с 1 по 21 марта.
  * 10 — количество дней c 22 марта до конца месяца.
  * 1000 ₽ — ежедневная сумма потребления с 22 марта до конца месяца.

Если к концу отчетного периода вы потратили на ресурсы {{ yandex-cloud }} больше 200 000 ₽, с момента превышения порога в 60 000 ₽ ежедневно с вашего лицевого счета будут списываться доли и фиксированной, и дополнительной стоимости. До 200 000 ₽ доля дополнительной стоимости — 7% от суммы, которую вы потратили за день, после — 5%.

  Например, вы потратили 60 000 ₽ с 1 по 21 марта. Затем с 22 марта по 26 тратили по 28 000 ₽ в день, а с 27 до конца месяца — по 10 000 ₽.

  В этом случае расчет дополнительной стоимости поддержки до превышения порога в 200 000 ₽ будет таким:

  >(200 000 ₽ − 60 000 ₽) × 7% = 140 000 ₽ × 0,07 = 9800 ₽

  В расчетах 60 000 ₽ — сумма потребления с 1 по 21 марта.

  Расчет дополнительной стоимости поддержки после превышения порога в 200 000 ₽ будет таким:

  >((200 000 ₽ + 5 × 10 000 ₽) — 200 000 ₽) × 5% =  50 000 ₽ × 0,05 = 2500 ₽

  В расчетах:

  * 200 000 ₽ — сумма потребления с 1 по 26 марта.
  * 5 — количество дней с 27 марта до конца месяца.
  * 10 000 ₽ — ежедневная сумма потребления с 27 марта до конца месяца.

  Итоговая стоимость составит:

  >6000 ₽ + 9800 ₽ + 2500 ₽ = 18 300 ₽

  В расчетах:

  * 6000 ₽ — фиксированная стоимость поддержки за месяц.
  * 9800 ₽ — дополнительная стоимость поддержки до превышения порога в 200 000 ₽.
  * 2500 ₽ — дополнительная стоимость поддержки после превышения порога в 200 000 ₽.

## Премиум {#premium}

Тариф <q>Премиум</q> включает в себя все услуги остальных тарифных планов и может быть дополнен, чтобы лучшим образом отвечать вашим потребностям. 

Чтобы получить оценку стоимости тарифного плана Премиум, пожалуйста, обратитесь к вашему менеджеру в {{ yandex-cloud }} или в [службу поддержки]({{link-console-support}}).

