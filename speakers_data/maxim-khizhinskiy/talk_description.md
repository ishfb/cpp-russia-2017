﻿Итераторы и конкурентные map/set - на первый взгляд, несовместимые понятия. 
В мире lock-free, где содержимое мапы динамично меняется, пройтись по всем элементам контейнера и не упасть, казалось бы, невозможно.
Или все же возможно?.. Какими свойствами должен обладать конкурентный контейнер, чтобы быть итерабельным?

В этом докладе я постараюсь ответить на этот вопрос, а также рассмотрю процесс создания итерабельного списка.
По пути мы споткнемся о несколько подводных камней и постараемся их преодолеть.

Для всех, кому интересно, как lock-free выглядит изнутри.