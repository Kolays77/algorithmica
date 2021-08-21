---
title: Теория вероятностей
---

В вузах теорию вероятностей очень долго аксиоматизируют перед тем, как перейти к чему-то полезному. Сейчас продемонстрируем, зачем.

[Парадокс Бертрана](https://ru.wikipedia.org/wiki/%D0%9F%D0%B0%D1%80%D0%B0%D0%B4%D0%BE%D0%BA%D1%81_%D0%91%D0%B5%D1%80%D1%82%D1%80%D0%B0%D0%BD%D0%B0_(%D0%B2%D0%B5%D1%80%D0%BE%D1%8F%D1%82%D0%BD%D0%BE%D1%81%D1%82%D1%8C%29):

> Рассмотрим равносторонний треугольник, вписанный в окружность. Наудачу выбирается хорда окружности. Какова вероятность того, что выбранная хорда длиннее стороны треугольника?

Оказывается, можно придумать как минимум три способа решать задачу, которые все выглядят адекватно, но при этом дают разные ответы.

1. Наудачу выберем две точки на окружности и проведём через них хорду. Чтобы посчитать искомую вероятность, представим, что треугольник повёрнут так, что одна из его вершин совпадает с концом хорды. Заметим, что если другой конец хорды лежит на дуге между двумя другими вершинами треугольника, то длина хорды больше стороны треугольника. Длина рассмотренной дуги равна трети длины окружности, значит искомая вероятность равна $\frac13$.

2. Зафиксируем радиус окружности, наудачу выберем точку на радиусе. Построим хорду, перпендикулярную зафиксированному радиусу, проходящую через выбранную точку. Для нахождения искомой вероятности, представим, что треугольник повёрнут так, что одна из его сторон перпендикулярна зафиксированному радиусу. Хорда длиннее стороны треугольника, если её центр ближе к центру, чем точка пересечения треугольника с зафиксированным радиусом. Сторона треугольника делит пополам радиус, следовательно вероятность выбрать хорду длиннее стороны треугольника $\frac12$.

3. Выберем наудачу произвольную точку внутри круга и построим хорду с центром в выбранной точке. Хорда длиннее стороны равностороннего треугольника, если выбранная точка находится внутри круга, вписанного в треугольник. Площадь вписанного круга есть $\frac14$ от площади большего, значит исходная вероятность равна $\frac14$.

Как мы увидели, от формального определения «случайной хорды» непосредственно зависит ответ. Каждый раз, когда в истории математики появляется подобный приводящий к протеворечиям парадокс, математики паникуют и начинают всё формализовывать и аксиоматизировать. Так появилась теория вероятностей.

## Аксиоматика

*Случайной переменной* или *случайной величиной* называется переменная, принимающая различые значения случайно. Сама по себе, случайная переменная только описывает возможные состояния; она должна быть связана с *вероятностным распределением*, которые указывает, насколько вероятно каждое из состояний.

Например, можно ввести случайную переменную, соответствующую исходу броска шестигранного кубика — она принимает значения из *вероятностного пространства* $\Omega = \{1, 2, 3, 4, 5, 6\}$, причём с равной вероятностью: $p(x=i) = \frac{1}{6}$.

### Непрерывные распределения

Случайные переменные могут быть не только дискретными, но и непрерывными. Например, мы можем ввести величину: случайное число от 0 до 1.

Плотность вероятности.

### Ожидание и дисперсия



### Нормальное распределение



### Парадокс дней рождений



### Условные вероятности



### Теория информации



### 

Случайные переменные могут быть дискретными или непрерывными. Дискретные переменные имеют конечное (броски кубика) или счётное количество состояний, а непрерывные переменные принимают значения на континууме.

Функцию X : \Omega \to R будем называть случайной величиной. Она сопостав-

ляет каждому элементарному исходу x \in \Omega какое-то число.

Например, мы можем ввести случайную переменную для исходов броска шестигранного кубика.

Случайные переменные могут быть дискретными или непрерывными. Дискретные переменные имеют конечное или счётное количество состояний. Непрерывные переменные принимают действительные значения.

Вероятностным пространством $\Omega$ называют какое-то множество элементарных исходов. Это, в общем-то, любое множество: например, $\{1, 2, 3, 4, 5, 6\}$ - исходы на кубике, или $\{(x, y) | 1 \leq x, y \leq 6\}$ - исходы на двух последовательно брошенных кубиках.

Событием $A$ в этом пространстве называется некоторое подмножество вероятностного пространства $\Omega$, например, пустое, или само $\Omega$, или $\{1, 2, 6\}$ --- подмножество $\{1, 2, 3, 4, 5, 6\}$.

События можно пересекать, объединять, дополнять --- они же подмножества.

На некоторых событиях (в том числе элементарных исходах) определена функция $P$, которую называют вероятностью. Она удовлетворяет следующим условиям:

1) $P(A \cup B) = P(A) + P(B)$, если они не пересекаются ($A \cap B = \emptyset$)

2) $P(\Omega) = 1$

Чаще всего (если ничего не указывает на обратное) на элементарных исходах вероятности равны --- это называется равномерным распределением.

Во всех этих задачах первого раздела в решениях нужно первым делом описать вероятностное пространство.

% \subsection{Места в электричке}
% % TODO куда-то передвинуть
% Андрей, Серёжа и Лёша едут в электричке из Долгопрудного. Отсеки по 6 человек, по 12 в вагоне, вагонов 9. Они хотели бы найти места, где они могут сесть втроем. Они заглянули в вагон и увидели там 7 свободных мест. Они хотят узнать, имеет ли смысл ходить по поезду в поиске свободного места. Помогите им, посчитав матожидание числа вагонов (вероятность найти место?), которые им нужно пройти.

\subsection{Монетка}
% TODO: какое-то из чисел нужно пофиксить так, чтобы ответ был 1/2
Андрей и Серёжа играют в игру. Они подбрасывают монетку $N$ раз. Если орлов выпало $K$ и больше, то побеждает Андрей. В противном случае побеждает Серёжа (ничья не предусмотрена). С какой вероятностью победит Серёжа?

a) N = 3, K = 2

b) N = 99, K = 50

c) N = 100, K = 50

\subsection{Рисуйте круги Эйлера}
Каждый школьник на сборах изучает хотя бы один из трех языков: Java, Python и C++. Вероятности, что случайно выбранный школьник изучает соответственно Java, Python и C++ равны $0.4$, $0.5$ и $0.6$. Вероятность, что школьник изучает Java и Python, равна $0.2$. Вероятность, что школьник изучает Python и C++, равна $0.3$. Вероятность, что школьник изучает C++ и Java, равна $0.2$. 

Найдите вероятность, что школьник изучает все три языка программирования. Найдите вероятность того, что школьник изучает только C++.

\subsection{Разбиение числа 10*}
Петя случайным образом разбивает число 10 на сумму трех слагаемых (целые, больше нуля). Опишите вероятностное пространство и вычислите вероятность того, что среди слагаемых будет число 4. Порядок слагаемых в разложении важен.

\subsection{Ладьи*}
На шахматной доске размера $n \times n$ случайно размещают $n$ ладей. Найдите вероятность следующих событий:

a) $A = \{$ладьи не бьют друг друга$\}$

b) $B = \{$ладьи не бьют друг друга, и на главной диагонали нет никаких фигур$\}$

\subsection{Подсчёт голосов*}
Докажите, что вероятность того, что на выборах с участием двух кандидатов, в которых первый набрал $p$ голосов, а второй набрал $q \leq p$, первый будет опережать второго в течение всего времени подсчета, равна $\frac{p-q}{p+q}$.
\newpage
\section{Геометрическая вероятность}

В этих задачах используется красивый прием --- вероятность равна отношению каких-нибудь площадей.

\subsection{Точка в прямоугольнике}
Случайная точка $A$ имеет равномерное распределение в прямоугольнике со сторонами $1$ и $2$. Найдите вероятность следующих событий:

a) расстояние от точки $A$ до любой стороны прямоугольника не превосходит $0.1$

b) расстояние от точки $A$ до ближайшей большей стороны прямоугольнике меньше, чем до ближайшей меньшей стороны.

\subsection{Два числа}
$X$ и $Y$ равномерно распределены на отрезке $[0, 1]$. Какая вероятность того, что $X^2 + Y^2 \leq 1$?

\subsection{Петя и Вася*}
Петя и Вася договорились встретиться с 12:00 до 13:00, но не договорились в какое время, поэтому каждый из них решил прийти в случайное время, подождать 10 минут и уйти. С какой вероятностью они встретятся?

\subsection{Два числа*} Найти вероятность того, что из трех наудачу взятых отрезков длиной не более, чем 1, можно составить треугольник.
\newpage
\section{Условная вероятность и независимость}

По определению, вероятность $A$ при условии $B$ равна $P(A | B) = \frac{P(A \cap B)}{P(B)}$. Это называется условной вероятностью, и в бытовом смысле это вероятность события $A$, если мы уже знаем, что событие $B$ точно произошло (мы как бы сужаем вероятностное пространство до $B$, отсюда и формула).

По определению, $A \perp B$ ($A$ независимо с $B$), если $P(A \cap B) = P(A) P(B)$. Это совпадает с бытовым понятием независимости событий. Если монетку кидают несколько раз, то считается, что эти броски независимы.

\subsection{Лампы}
Помещение освещается фонарем с тремя лампами. Вероятность перегорания одной лампы в течение года равна $0.3$. Найдите вероятность того, что в течение года хотя бы одна лампа не перегорит.

\subsection{Формула Байеса и формула полной вероятности}
a) Докажете формулу Байеса:
$$P(A|B) = \frac{P(B|A)P(A)}{P(B)}$$

По смыслу это очень крутая формула --- обычно ты знаешь вероятность событий при каких-то условиях, а вот вероятности выполнения этих условий неочевидны. С помощью этих формул можно посчитать вероятность условий при условии выполнения этих событий.

b) Докажите формулу полной вероятности:
$$P(A) = P(A|B_1)P(B_1) + ... + P(A|B_n)P(B_n)$$
при условии
$$\Omega = B_1 \cup ... \cup B_n (B_i \cap B_j = \emptyset)$$

Это важная и интуитивно понятная формула --- событие просто разбивается на непересекающиеся подслучаи, считаются вероятности событий в этих случаях, и усредняется с весами, равными вероятностям этих случаев.

\subsection{Задача на формулу Байеса, либо формулу полной вероятности}
Из 30 стрелков 12 попадает в цель с вероятностью 0,6, 8 - с вероятностью 0,5 и 10 – с вероятностью 0,7. Наудачу выбранный стрелок произвел выстрел, поразив цель. К какой из этих трех групп вероятнее всего принадлежал этот стрелок? Найдите вероятность его принадлежности к этой группе (при условии, что он действительно попал).

% Я не понял ничего про эту задачу
% \subsection{Экзитпол*}
% Вы опрашиваете людей на выходе из избирательного участка, кто за кого проголосовал. Всего есть два кандидата — А и Б. Вы опросили 100 людей, из которых 55 проголосовали за А. С какой вероятностью кандидат А победит?

\subsection{Контпримеры*}
Привести примеры, показывающие, что равенства

$$P(B|A) + P(B|\overline A) = 1$$

$$P(B|A) + P(\overline B|\overline A) = 1$$

неверны.

\subsection{Еще контрпример*}
События $A_1$, ..., $A_k$ по определению независимы в совокупности, если для любого их подмножества $A_{i_1}$, ..., $A_{i_t}$ верно равенство $P(A_{i_1}, ..., A_{i_t}) = P(A_{i_1}) \times ... \times P(A_{i_t})$).

Приведите пример трех попарно независимых событий, которы, тем не менее, в совокупности зависимы.

\subsection{Попарно независимые события*}
Пусть $A$, $B$, $C$ – попарно независимые равновероятные события, причем $A \cap B \cap C = \emptyset$. Найдите максимально возможное значение $P(A)$.
\newpage
\section{Случайная величина и функция распределения}

Функцию $X: \Omega \rightarrow\mathbb{R}$ будем называть случайной величиной. Она сопоставляет каждому элементарному исходу какое-то число. Тогда можно определить и $P(X \in A)$ - вероятность, что случайная величина $X$ лежит в каком-то подмножестве действительных чисел $A$, потому что $X \in A$ — это событие в вероятностом пространстве $\Omega$.

Функцией распределения называют $F_X(x) = P(X \leq x)$.

Плотностью распределения называют либо $\rho_X(k) = P(X = k)$ (в дискретном случае), либо $\rho_X(x) = F_X(x)'$ --- производную функции распределения.

\subsection{Функции распределения}
Найдите и нарисуйте функции распределения и плотности следующих случайных величин:

a) $X = 1$

b) $X =
\begin{cases} 
    0, & p \\
    1, & 1-p 
\end{cases}
$

c) $X \sim U[0, 1]$ ($X$ равномерно распределена на отрезке $[0, 1]$)

\subsection{Геометрическое распределение}
Петя кидает монету, с вероятностью $p$ выпадает орел и он прекращает кидать ее, с вероятностью $1-p$ выпадает решка и он кидает ее еще раз. Пусть $X$ - это количество бросков. Найдите $\rho_X(x)$ и $F_X(x)$.

% \subsection{Пуассон}
% % Это лучше рассказать просто так
% Мост может выдержать до $k$ машин. Чтобы проехать по нему, требуется 1 час. В каждую очень малую единицу времени заезжает машина с вероятностью $\lambda$. Найдите вероятность того, что мост рухнет в промежуток времени $t$, то есть по нему за это время проедет более $k$ машин.
\newpage
\section{Мат. ожидание и дисперсия}
Мат. ожиданием случайной величины $X$, которая принимает значения $a_0$, $a_1$, ... называют 
$$E[X] = a_0 P(X = a_0) + a_1 P(X = a_1) + ...  = \sum_{x} x p_X(x) $$

Если X принимает несчетное число значение (например, равномерное распределение на отрезке $[0, 1]$), то мат. ожидание определяется как интеграл фукнции $x$ умножить на плотность (достаточно понимать, что интеграл - это площадь под графиком этой функции):
$$E[X] = \int\limits_{-\infty}^{\infty} x \rho (x) dx$$

Дисперсия определяется как $D[X] = E[(X-E[X])^2]$ --- средний квадрат отклонения случайной величины от ее мат. ожидания.

В бытовом смысле мат. ожидание --- это среднее значение случайное величины, а именно если взять несколько независимых одинаково распределенных случайных величин, то их среднее действительно будет стремиться к мат. ожиданию (например на физике делают несколько опытов и усредняют ответ именно для этого).

В бытовом смысле дисперсия --- это насколько случайная величина шумная.

Самая главная вещь в теории вероятностей: мат. ожидание линейно:

\begin{align*}
E[X+Y] & = \sum_{x, y} (x+y) p(x, y)
\\     & = \sum_{x, y} x p(x, y) + \sum_{x, y} y p(x, y)
\\     & = \sum_x x p(x) \sum_y p(y) + \sum_y y p(y) \sum_x p(x)
\\     & = \sum_x x p(x) + \sum_y y p(y)
\\     & =  E[X] + E[Y] 
\end{align*}

Если $X \perp Y$ (это значит, что все события вида $X \in A$ независимы всем событиям вида $Y \in B$), то еще и произведение можно снимать:

$$ E[X \cdot Y] = E[X] \cdot E[Y] $$

% Дисперсия суммы, произведения, домноженя на константу?

\subsection{Простые примеры}

Найдите мат. ожидания и дисперсии следующих случайных величин:

a) $X = 1$

b) $X =
\begin{cases} 
    0, & p \\
    1, & 1-p 
\end{cases}
$

c) $X \sim U[0, 1]$ ($X$ равномерно распределена на отрезке $[0, 1]$)

d) Случайная величина из задачи 4.2 (геометрическое распределение) [10-11 классам надо честно найти, 8-9 классам можно погуглить чему равна сумма ряда, так как для его нахождения нужно уметь дифференцировать]

\subsection{Простая формула для дисперсии}
Докажите, что $$D[X] = E[X^2] - E[X]^2$$

\subsection{Разбиение на индикаторы}
Кинули кубик $N$ раз, найдите мат. ожидание числа выпавших шестерок.

Подсказка: случайную величину $X[$количество выпавших шестерок$]$ можно представить как $$X = I_1 + ... + I_N$$
где $I_k =
\begin{cases} 
    1, & $на k-м кубике выпало $ 6 \\
    0, & $иначе$ 
\end{cases}
$
Подсказка 2: используйте после этого линейность мат. ожидания

\subsection{Случайный граф*}
Взяли $N$ вершин и каждую пару разных вершин соединили с вероятностью $0.5$. Найдите

a) мат. ожидание числа ребер

b) мат. ожидание числа треугольников

\subsection{Случайный граф - 2*}
Взяли $N$ вершин и каждую пару разных вершин соединили с вероятностью $0.5$. Найдите

a) дисперсию числа ребер

b) дисперсию числа треугольников

\newpage
\section{Нормальное распределение}
% ты знаешь доказательство «на пальцах»?
% доказательство чего? ЦПТ
% может не надо? может в следующий раз?
% Ну, хоть как-то убедить в правильности
% Там, про выборы и соцопросы рассказать
% мне кажется, это можно упомянуть и не доказывать

% кстати, зацени http://sereja.me/a/pollard

%Метод Монте-карло и его относительная ошибка.

Есть замечательное нормальное распределение $N(a, \sigma^2)$ --- это распределение со страшной плотностью $$\rho(x) = \frac{1}{\sigma\sqrt{2\pi}}e^{-{\frac{(x-a)^2}{2\sigma^2}}}$$ 
Причем его мат. ожидание равно $a$, а дисперсия равна $\sigma^2$.

Оно замечательно тем, что если взять много независимых случайных величин одного любого распределения $X$, то распределение их среднего арифметического примерно равно $N(E[X], \frac{D[X]}{N})$. Этот факт (более строгий, конечно) называется Центральной Предельной Теоремой.

\subsection{Кубики}
Нарисуйте, как распределена (график плотности, или просто значения плотности) сумма значений на N игральных кубиках при

a) N = 1

b) N = 2

c) N = 3

d*) N = 5

e*) N = 100 

Подсказка: для 5 и 100 можно написать программу и нарисовать гистгорамму.

\subsection{Сумма нормальных величин}
Известно, что сумма двух нормально распределенных случайных величин --- тоже нормально распределенная случайная величина. Пусть $X \sim N(0, 1), Y \sim N(5, 4)$, найдите параметры (мат. ожидание и дисперсию) у случайной величины $2X + Y$.
\newpage
\section{Оценка времени работы алгоритмов и не только}

Про рандомизированные алгоритмы мы очень часто говорили фразу "в среднем работает за O(n)". Это означает, что количество операций --- это случайная величина, и её мат. ожидание --- O(n).

\subsection{Quicksort}
Докажите, что Quicksort со случайным выбором опорного элемента на любой фиксированной перестановке работает в среднем за $O(n\log{n})$ сравнений.

Подсказка 1: разбейте количество сравнений на простые случайные величины и используйте линейность мат. ожидания.

Подсказка 2: докажите лемму --- два числа $x_i$ и $x_j$ сравниваются только в том случае, если опорным элементом среди всех элементов между ними (в упорядоченном массиве) первым опорным элементом был выбран один из этих двух.

\subsection{Высота случайного бинарного дерева*}
Найдите мат. ожидание глубины вершины случайного бинарного дерева (например, декартово дерево таким является), а именно такого дерева, у которого приоритеты вершин распределены одинаково, и по приоритетам дерево является кучей.

Подсказка: Докажите лемму --- для любых $i\neq k$ , $x_i$ является предком $x_k$ тогда и только тогда, когда $x_i$ имеет наибольший приоритет среди $x_{min(i, k)}$, $x_{min(i, k) + 1} ... x_{max(i, k)} $.

\subsection{Эратосфен*}
Предполагая, что вероятность того, что число $k$ простое, равно $\frac{1}{\ln k}$, покажите, что обычное решето Эратосфена работает за $O(n \log \log n)$.

% \subsection{Гипотеза Гольдбаха}
% Предполагая, что простые числа распределены как в прошлой задаче, «докажите» гипотезу Гольдбаха.

\subsection{Разрушение дерева*}
Дано корневое дерево. Каждую итерацию выбирается вершина (равновероятно из всех оставшихся), и удаляется всё поддерево, соответствующее этой вершине. Найти, сколько ходов в среднем будет продолжаться этот процесс, то есть матожидание номера итерации, на которой будет удалён корень дерева.

\subsection{Альтернативное декартово дерево}
Пусть при мердже двух деревьев мы делаем подвешивание не за вершину с большим приоритетом, а следующим образом:

\begin{itemize}
  \item За левое с вероятностью $\frac{L}{L+R}$.
  \item За правое с вероятностью $\frac{R}{L+R}$.
\end{itemize}

где $L$ и $R$ это размеры соответствующих деревьев.

Покажите, что каждая вершина всё так же равновероятно будет корнем дерева.

% \section{Случайные процессы}

% \subsection{От нуля до единицы*}

% Дан следующий код:

% % что-то не работает, как исправить?
% \begin{lstlisting}[language=Python]
% x = 0
% while x < 1:
%     x += random()
% \end{lstlisting}

% Требуется посчитать матожидание x.

% (random в питоне возвращает случайное действительное число от 0 до 1.)

% \subsection{Пьяница}
% Пьяница стоит на краю обрыва (обрыв слева). С вероятностью $p$ он идёт на один шаг вправо, с вероятностью $p-1$ — на один шаг влево. Посчитайте вероятность того, что пьяница когда-либо упадёт.

% \subsection{Казино*}
% Вы стартуете с $A$ долларов и играете в азартную игру, постоянно делая ставку один доллар, которая дает вам два доллара с вероятностью $p < \frac{1}{2}$. Для оплаты смены в лагере Юнивёрсум вы хотите в какой-то момент получить $B > A$ долларов, и как только это произойдет, вы играть прекратите. Найдите вероятность, что вы уйдете с деньгами. Вы либо уходите с $B$ долларами, либо разоряетесь. Возможно, вам придётся играть бесконечно.

## Плотность распределения

Пусть есть некоторая случайная величина $X$. *Плотностью распределения* $X$ называется функция $p(x)$, отражающая относительную вероятность наступления события $X=x$ (то есть относительно всех остальных возможных событий). Например, для случайной величины с конечным множеством элементарных исходов $\Omega$ $p(x)=P(X=x)$ (где $P(A)$ - вероятность наступления события $A$). Обычно функция плотности вероятности предполагается нормированной на единицу (то есть площадь под графиком равна 1). *Функцией распределения* случайной численной величины $F(x)$ называется вероятность попадания $X$ в луч $(-\infty;\,x]$ (или $\int_{-\infty}^{x}p(x)\,dx$). 

## Матожидание

Предположим, у нас есть случайная численная величина $X$ с функцией плотности $p(x)$. Тогда математическое ожидание случайной величины равно сумме $P(A) \cdot A$ для всех возможных исходов $A$. TODO

## Дисперсия

Какие два числа лучше всего описывают распределение?

## Нормальное распределение

Центральная предельная теорема названа так пафосно вполне обоснованно.

Она говорит, что нам достаточно про каждое слагаемое знать всего два числа — ожидание и дисперсию.

$$ f(x) = \frac{1}{2\sqrt{\pi}} e^{-\frac{(x-\mu)^2}{\sigma^2}} $$

Доказать это очень трудно. Даже со ссылками на мощные теоремы оно займёт не одну страницу. Обычно доказательство рассказывают в середине второго курса.

Трудно даже доказать, что это распределение, т. е. что.

## Применения

Пусть в некоторой стране есть два кандидата в президенты, назовём их Путин и Навальный.

Мы спросили у 1000 случайных избирателей бинарный вопрос, и 510 из них сказали, что будут голосовать за Путина. С какой вероятностью он победит? Теорема говорит, что число голосов, как 

## Линейные рекурренты

Чтобы решать следующие задачи, нам нужно будет использовать следующий факт:

...

Доказательство мы не приведем.

В частности, таким образом получается формула для чисел Фибоначчи.

$$ f_n = \ldots $$

Кто бы мог подумать, что все эти иррациональности и степени сократятся и вообще дадут целое число?..

## Классика

Парадокс дней рождения.

Это на самом деле очень часто используемый результат. Так можно считать вероятность коллизии хэшей, а также он используется во многих теоретико-числовых алгоритмах, в которых используется предположения (весьма справедливые) о распределении простых чисел.

Пьяница. Человек стоит на краю обрава и идёт в его сторону с вероятностью p. С какой вероятностью он когда-либо в него упадёт?

TODO: история про эстетическое удовольствие, азарт и смысл посещения казино.
Казино. Мы приходим в казино с 1000\$ и следующим образом проводим там время: ставим по 1\$, пока не обанкротимся или не выиграем 1100\$. Какая вероятность того, что мы уйдём с деньгами?

## Парадокс дней рождений

> В группе, состоящей из 23 или более человек, вероятность совпадения дней рождения хотя бы у двух людей превышает 50%.

Более общее утверждение: в мультимножество нужно добавить $\Theta(\sqrt{n})$ случайных чисел от 1 до n, чтобы какие-то два совпали.

**Первое доказательство** (для любителей матана). Пусть $f(n, d)$ это вероятность того, что в группе из $n$ человек ни у кого не совпали дни рождения.
Будем считать, что дни рождения распределены независимо и равномерно в промежутке от $1$ до $d$.

$$
f(n, d) = (1-\frac{1}{d}) \times (1-\frac{2}{d}) \times ... \times (1-\frac{n-1}{d})
$$

Попытаемся оценить $f$:

$$
\begin{aligned}
    e^x & = 1 + x + \frac{x^2}{2!} + \ldots & \text{(ряд Тейлора для экспоненты)} \\
    & \simeq 1 + x & \text{(аппроксимация для $|x| \ll 1$)} \\
    e^{-\frac{n}{d}} & \simeq 1 - \frac{n}{d} & \text{(подставим $\frac{n}{d} \ll 1$)} \\
    f(n, d) & \simeq e^{-\frac{1}{d}} \times e^{-\frac{2}{d}} \times \ldots \times e^{-\frac{n-1}{d}} & \\
    & = e^{-\frac{n(n-1)}{2d}} & \\
    & \simeq e^{-\frac{n^2}{2d}} & \\
\end{aligned}
$$

Из последнего выражения более-менее понятно, что вероятность $\frac{1}{2}$ достигается при $n \approx \sqrt{d}$ и в этой точке изменяется очень быстро.

**Второе доказательство** (для любителей теорвера). Введем $\frac{n(n-1)}{2}$ индикаторов — по одному для каждой пары людей $(i, j)$ — каждый будет равен единице, если дни рождения совпали. Ожидание и вероятность каждого индикатора равна $\frac{1}{d}$.

Обозначим за $X$ число совпавших дней рождений. Его ожидание равно сумме ожиданий этих индикаторов, то есть $\frac{n (n-1)}{2} \cdot \frac{1}{d}$.

Отсюда понятно, что если $d = \Theta(n^2)$, то ожидание равно константе, а если $d$ асимптотически больше или меньше, то $X$ стремится нулю или бесконечности соответственно.

*Примечание*: формально, из этого явно не следует, что вероятности тоже стремятся к 0 и 1.

### Бонус: «мета-задача»

Дана произвольная строка, по которой известным только авторам задачи способом генерируется ответ yes/no. В задаче 100 тестов. У вас есть 20 попыток отослать решение. В качестве фидбэка вам доступны вердикты на каждом тесте. Вердиктов всего два: OK (ответ совпал) и WA. Попытки поделить на ноль, выделить терабайт памяти и подобное тоже считаются как WA.

«Решите» задачу.

## Принцип максимального правдоподобия

## Энтропия

Энтропией называется минимальное число бит, которым теоретически возможно сжать сообщение. Эта величина важна, потому что на практике если её можно посчитать, то сжатие с соответствующей кратностью реально достижимо.

Шумный канал.

Пусть у вас есть 1тб данных и два китайских терабайтника, на каждый из которых можно записать столько данных, но каждый бит имеет вероятность 10% записаться на противоположный. Требуется сохранить данные с первого раза без потерь. Совсем без потерь.

Причём это делается почти впритык.

# Теорвер для алгоритмистов

Вы, наконец, узнаете, почему ДД работает за логарифм, почему быстрая сортировка быстрая, какой модуль нужно выбирать для хэшей, сколько сэмплов нужно выбирать для монте-карло и т. д.

Следующие строчки позволят нам генерировать распределения и рисовать графики, не обращайте внимание.

# Аксиоматика

В вузах теорвер очень долго аксиоматизируют перед тем, как перейти к чему-то полезному. Сейчас поясним, зачем.

[Парадокс Бертрана](https://ru.wikipedia.org/wiki/%D0%9F%D0%B0%D1%80%D0%B0%D0%B4%D0%BE%D0%BA%D1%81_%D0%91%D0%B5%D1%80%D1%82%D1%80%D0%B0%D0%BD%D0%B0_(%D0%B2%D0%B5%D1%80%D0%BE%D1%8F%D1%82%D0%BD%D0%BE%D1%81%D1%82%D1%8C%29):

> Рассмотрим равносторонний треугольник, вписанный в окружность. Наудачу выбирается хорда окружности. Какова вероятность того, что выбранная хорда длиннее стороны треугольника?

Оказывается, можно придумать хотя бы три способа решать задачу, которые выглядят адекватно, но все дают разные ответы.

2. Наудачу выберем две точки на окружности и проведём через них хорду. Чтобы посчитать искомую вероятность, представим, что треугольник повёрнут так, что одна из его вершин совпадает с концом хорды. Заметим, что если другой конец хорды лежит на дуге между двумя другими вершинами треугольника, то длина хорды больше стороны треугольника. Длина рассмотренной дуги равна трети длины окружности, значит искомая вероятность равна $\frac13$.

3. Зафиксируем радиус окружности, наудачу выберем точку на радиусе. Построим хорду, перпендикулярную зафиксированному радиусу, проходящую через выбранную точку. Для нахождения искомой вероятности, представим, что треугольник повёрнут так, что одна из его сторон перпендикулярна зафиксированному радиусу. Хорда длиннее стороны треугольника, если её центр ближе к центру, чем точка пересечения треугольника с зафиксированным радиусом. Сторона треугольника делит пополам радиус, следовательно вероятность выбрать хорду длиннее стороны треугольника $\frac12$.

4. Выберем наудачу произвольную точку внутри круга и построим хорду с центром в выбранной точке. Хорда длиннее стороны равностороннего треугольника, если выбранная точка находится внутри круга, вписанного в треугольник. Площадь вписанного круга есть $\frac14$ от площади большего, значит исходная вероятность равна $\frac14$.

Как мы увидели, от формального определения «случайной хорды» непосредственно зависит ответ.

Каждый раз, когда в истории математики появляется подобный приводящий к протеворечиям парадокс, математики паникуют и начинают всё формализовывать и аксиоматизировать. Так появилась теория вероятностей (внимание: не «ти», а «тей»).

Перейдем к самим определениям:

Функцию $X : \Omega \to R$ будем называть случайной величиной. Она сопостав-
ляет каждому элементарному исходу какое-то число.

## Распределения

**Геометрическое распределение**.

## Парадокс дней рождений

Пусть $f(n, d)$ это вероятность того, что в группе из $n$ человек ни у кого не совпали дни рождения.
Будем считать, что дни рождения распределены независимо и равномерно в промежутке от $1$ до $d$.

$$f(n, d) = (1-\frac{1}{d}) \times (1-\frac{2}{d}) \times ... \times (1-\frac{n-1}{d})$$

Попытаемся оценить $f$:

$$
\begin{align}
  \begin{aligned}
    e^x & = 1 + x + \frac{x^2}{2!} + \ldots & \text{(ряд Тейлора для экспоненты)} \\
    & \simeq 1 + x & \text{(аппроксимация для $|x| \ll 1$)} \\
    e^{-\frac{n}{d}} & \simeq 1 - \frac{n}{d} & \text{(подставим $\frac{n}{d} \ll 1$)} \\
    f(n, d) & \simeq e^{-\frac{1}{d}} \times e^{-\frac{2}{d}} \times \ldots \times e^{-\frac{n-1}{d}} & \\
    & = e^{-\frac{n(n-1)}{2d}} & \\
    & \simeq e^{-\frac{n^2}{2d}} & \\
  \end{aligned}
\end{align}
$$

# Матожидание

Математическим ожиданием случайной величины $X$, которая принимает значения $x_1, x_2, \ldots$ называется

$$ E[X] = \sum_{x \in S} p_S(x) \cdot x $$

Самое главное для нас свойство — ожидание линейно:

$$
\begin{align*}
E[X+Y] & = \sum_{x, y} (x+y) p(x, y)
\\     & = \sum_{x, y} x p(x, y) + \sum_{x, y} y p(x, y)
\\     & = \sum_x x p(x) \sum_y p(y) + \sum_y y p(y) \sum_x p(x)
\\     & = \sum_x x p(x) + \sum_y y p(y)
\\     & =  E[X] + E[Y] 
\end{align*}
$$

Акцентируем внимание: $X$ и $Y$ вообще не важно какие. Возможно, они связаны как-то очень сложно, но это не важно. Как мы потом, увидем, это свойство очень упрощает вычисление матожиданий каких-то очень сложных шняг.

Также, в частности его можно домножать на константу.

Теперь можно перейти к практическим задачам.

## Геометрическое распределение

> Петя кидает монету, с вероятностью $p$ выпадает орел и он прекращает кидать ее, с вероятностью $1-p$ выпадает решка и он кидает ее еще раз. Пусть $X$ - это количество бросков. Найдите $\rho_X(x)$ и $F_X(x)$.

## Неподвижные точки в перестановке

Когда автор пришел на первое занятие по английскому в МФТИ, препод устроила следующую игру на знакомство: разделила всех студентов на две команды. В каждой команде про своих членов загадываются факты: кто-то мечтал стать акробатом, кто-то смотрит анимэ и всё в таком духе. Команде соперников сообщались только эти факты, и им нужно было отгадать, кому какой принадлежит. Побеждает команда, которая отгадала больше фактов о соперниках. Нас было 11 — простое число, никак не делящееся на равные команды, и поэтому в одной команде было 5 человек, а в другой 6. Автору стало интересно: если отбросить все психологические аспекты и делать все рандомно, у какой команды вероятность победить выше?

Следует заметить, что все-таки ожидание правильно отгаданных вопросов не очень помогает выяснить, у какой команды есть преимущество и какое.

## Высота декартова дерева

**Высота дерева**. Высота в среднем логарифмическая. Любознательные могут ознакомиться с типа доказательством, но это не обязательно.

Глубина вершины — это количество родителей (прим. К. О.). Введем *индикатор*. $E[h] = \sum \frac{1}{k} \approx \log n $.

## Асимптотика quicksort-а

Тут на самом деле будет примерно так же, как с ДД. Нас интересует суммарное число сравнений. Просуммируем для каждой пары элементов вероятность, что они будут сравнены.

Как для пары определить эту вероятность? Посмотрим на все элементы между ними, будь они в отсортированном массиве.

Внезапно возникает гармонический ряд, ну а дальше мы знаем.

# Дисперсия

Дисперсия — это количественная метрика. Это не что-то абстрактное, как могли рассказать в школе на теорвере, а формально определенная величина, имеющая кучу всяких полезных свойств.

Дисперсия определяется как средний квадрат отклонения случайной величины от ее матожидания:

$$ D[X] = E[(X − E[X])^2] $$

Её проще считать по другой формуле, разложив квадрат внутри ожидания:

$$
\begin{align}
D[X] &= E[(X − E[X])^2]
\\   &= E[X^2 - 2 \cdot X \cdot E[X] + E[X]^2]
\\   &= E[X^2] - E [\underbrace{2 \cdot E[X]}_{const} \cdot X ] + E[E[X]^2]
\\   &= E[X^2] - 2 E[X]^2 + E[X]^2
\\   &= E[X^2] - E[X]^2
\end{align}
$$

Эту формулу мы будем использовать для вывода разных свойств.

У дисперсии очень много крутых свойств.

$$ D[k X] = E[k^2 X^2] - E[k X]^2 = k^2 (E[X^2] - E[X]^2) = k^2 D[X] $$

Предполагаем, что $X$ и $Y$ независимы.

$$
\begin{align}
D[X + Y] &= E[(X+Y)^2] - E[X+Y]^2
\\       &= E[X^2 + X Y + Y^2] - (E[X] + E[Y])^2
\\       &= E[X^2] + E[Y^2] - E[X]^2 - E[Y]^2
\\       &= D[X] + D[Y]
\end{align}
$$

Важное отличие от свойств матожидания: дисперсию так просто можно считать только для независимых величин.

## Закон больших чисел

Закон больших чисел — принцип, который описывает результат выполнения одного и того же эксперимента много раз. Согласно закону, среднее значение конечной выборки из фиксированного распределения близко к математическому ожиданию этого распределения.

У матожидания (константы) стандартное обозначение $\mu$ (мю), а у дисперсии $\sigma$ (сигма).

$$ M_n = \frac{X_1 + \ldots + X_n}{n} $$

$$ E[M_n] = \frac1n E[X_1 + \ldots + X_n] = \mu $$

Это немного очевидное равенство. Теперь нас интересует, насколько точно оно в реальности достигается:

$$ D[M_n] = \frac{1}{n^2} D[X_1 + \ldots + X_n] = \frac{\sigma}{n} $$

С одной стороны, оно домножается на $\frac{1}[n^2}$ из-за усреднения, с другой — на $n$ из-за суммирования.

## Нормальное распределение

Когда вы в каких-нибудь библиотеках для анализа данных просите показать какой-то summary, то чаще всего вы увидите два числа: матожидание и дисперсию.

Центральная предельная теорема названа так пафосно вполне обоснованно.

Она говорит, что нам достаточно про каждое слагаемое знать всего два числа — ожидание и дисперсию.

$$ f(x) = \frac{1}{2\sqrt{\pi}} e^{-\frac{(x-\mu)^2}{\sigma^2}} $$

Доказать это очень трудно. Даже со ссылками на мощные теоремы оно займёт не одну страницу. Обычно доказательство рассказывают в середине второго курса.

Трудно даже доказать, что это распределение, т. е. что $\int_{-\inf}^\inf f(x) dx = 1$.

## Метод Монте-Карло

Алгоритмы вида «давайте посчитаем значения в разных случайных точках и усредним» называются методами монте-карло.

Пусть у нас есть единичный квадрат и несколько сотен кружков. Нам нужно посчитать долю области квадрата, которая не покрывается ни одним из кругов, с точностью до 1%.

Можно просто делать так: тыкать в 10000 случайных точек и проверять для каждой, является ли она «хорошей», а затем вывести $\frac{\text{хорошие}}{\text{хорошие} + \text{плохие}}$ в качестве ответа.

Сдать можно сюда.

## Хэш-таблицы

Вообще, хэш — это такая функция, которая сопоставляет элементу какой-то другой элемент. С точки зрения криптоанализа, она должна быть трудно обратимой, а с точки зрения алгоритмиста — генерирующей равномерные игреки.

Можно делать так если мы планируем хранить $n$ элементов, то нужно завести $\Theta(n)$ ячеек, каждая из которых будет на самом деле односвязным списокм.

Это будет работать, потому что из-за рандома в среднем в каждой ячейке будет по одному элементу. Но константа у такого решения большая.

Стандартная хэш-таблица из STL по непонятным автору причинам работает очень медленно. Во многих задачах она является самой нагруженной структурой. Её можно написать в 3-5 раз быстрее.