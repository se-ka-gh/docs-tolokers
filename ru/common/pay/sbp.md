# Система быстрых платежей

#### Особенности Системы быстрых платежей

Вывод средств через СБП отличается простотой и удобством, высокой скоростью проведения транзакций и низкими комиссиями.

{% note alert %}

Вывод средств через СБП доступен только для граждан РФ, подтвердивших статус [самозанятого](../self-employed/about.md) и указавших Толоку партнером в системе Мой Налог.

{% endnote %}


#### Условия

{% if platform=="web" %}

{% include [popup-info-sbp-conditions](../_includes/pay/popup-info/id-popup-info/sbp-conditions.md) %}

{% elsif platform=="android" or platform=="ios"  %}

#|
|| Где работает | РФ ||
|| Комиссия | 0,11% ||
|| Минимальная сумма вывода |

{% cut "от 0,01 до 1 $" %}

0,01 \$, если раз в неделю или реже. Последующие платежи в течение недели — 1 \$.

{% endcut %}

||
|| Способ вывода | Средства выводятся на счет в банке. Список доступных банков зависит от оператора услуги и может меняться.

{% note alert %}

Вывод средств через СБП доступен только для граждан РФ, подтвердивших статус [самозанятого](../self-employed/about.md) и указавших Толоку партнером в системе Мой Налог.

{% endnote %}

||
|#
{% endif %}

## Как вывести из Толоки {#withdraw-from-toloka}

{% note alert %}

Для корректного проведения операции ваш номер телефона в Яндекс ID должен совпадать с номером телефона в том банке, в который вы хотите вывести деньги.

{% endnote %}

{% if platform=="ios" %}
1. Перейдите в **{{ mobile_ios_profile }}**.
{% elsif platform=="web" or platform=="android" %}
1. Перейдите в [Мои деньги]({{ toloka-money }}).
{% endif %}
1. Выберите способ вывода **{{ ui_worker_money_page_transaction__SBP_SE }}**. В открывшейся форме будут указаны ваши данные, которые мы получили при верификации.
1. Выберите банк из списка. Если у вас есть карты в разных банках, и они подключены к Системе быстрых платежей, все эти банки окажутся в списке. Номер карты вводить не нужно.
{% if platform=="ios" or platform=="web" %}
1. Укажите сумму, которую вы хотите вывести. Комиссия за вывод средств составит 0,11% от суммы.
{% endif %}
1. Поставьте галочку согласия на обработку персональных данных. Это необходимо, чтобы мы могли отправить в банк всю информацию, необходимую для проведения платежа.
1. Нажмите {% if platform=="android" %}**{{ mobile_android_button_next }}**{% elsif platform=="ios" %}**{{ mobile_ios_button_next }}**{% elsif platform=="web" %}**{{ ui_worker_money__withdraw__submit }}**{% endif %}.
{% if platform=="android" %}
1. Укажите сумму, которую вы хотите вывести. Комиссия за вывод средств составит 0,11% от суммы.
1. Нажмите кнопку **{{ mobile_android_money_do_withdraw }}**.
{% endif %}
1. Если нужно, введите код из SMS для подтверждения.
1. Ваша заявка на вывод средств принята. Подождите пару минут и проверьте, поступили ли деньги.

{% include [check](../_includes/pay/about/check.md) %}



## Решение проблем {#troubleshooting}

#### У меня нет СБП среди способов вывода.

Чтобы вывести средства через СБП, вы должны подтвердить статус [самозанятого](../self-employed/about.md).


[![](../assets/buttons/contact-support.svg)](../troubleshooting/troubleshooting.md#money_withdrawal)

