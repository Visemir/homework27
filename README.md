1) Використовуючи Docker, необхідно підняти: nt

• Стек моніторингу (Prometheus, Grafana, AmertManager)

• Експортери, які необхідні для виконання завдання

![](https://github.com/Visemir/homework27/blob/main/docker.jpg)


2) Налаштувати моніторинг потрібно для:

• працюючих контейнерів

• системних метрик (CPU, Оперативна памʼять і тп)

3) Для відповідних експортерів, підключити дашборди, використовуючі готові із Grafana спільноти.

![](https://github.com/Visemir/homework27/blob/main/dashbord-docker.jpg)

![](https://github.com/Visemir/homework27/blob/main/dashbord-node.jpg)


5) Налаштувати [алерти](https://github.com/Visemir/homework27/blob/main/prometheus/alert_rules.yml), які будуть відправлятися до [Telegram](https://github.com/Visemir/homework27/blob/main/alertmanager/alertmanager.yml) коли:

- кількість вільного місця < 15%

- завантаженість CPU > 80%

- хоча б один із таргетів, з яких прометеус збирає метрики, не доступний

![](https://github.com/Visemir/homework27/blob/main/alerts-grafana.jpg)

![](https://github.com/Visemir/homework27/blob/main/telegram.jpg)
