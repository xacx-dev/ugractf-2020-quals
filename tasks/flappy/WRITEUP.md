# Турбоптица: Write-up

Исполняемый файл выглядит как Windows-приложение, которое можно попробовать запустить. Однако, на деле игрока встретила бы лишь ошибка, различающаяся от версии к версии Windows. Дело в том, что наша игра написана под DOS, и для её запуска пригодится DOSBox.

Открывая приложение в эмуляторе или на 32-битной версии Windows, мы сталкиваемся с ошибкой «Wow your CPU is too fast for this game sorry». Нам намекают, что игру нужно запускать под определённой тактовой частотой. Установив правильную частоту в DOSBox, мы увидим игру, похожую на Flappy Bird — зелёная линия будет продвигаться вперёд, пока не столкнётся с препятствием.

Здесь можно было заняться реверс-инжинирингом, найти переменную, отвечающую за положение птицы, и выставить её дальше. Впрочем, в игру можно было сыграть по-настоящему. Управлением в игре являлась скорость процессора, которую можно контроллировать в DOSBox в реальном времени — изменение частоты поднимало и опускало птицу.

![Полное прохождение игры](images/walkthrough.gif)

Флаг: **ugra_moore_is_flapping_in_his_dreams_365bd0c7e01414baa47423338ec**.