# Модель обвала песка
Пример нескольких состояний следующей модели: 
Имеется граф, в каждой вершине графа есть некоторое целое число песчинок, если количество песчинок в некоторой вершине превышает её степень, то в ней происходит "обвал": из этой вершины по одной песчинке переходит в каждую соседнюю с ней(тем самым, число песчинок в ней уменьшается на её степень, а в соседях увеличивается на 1). Также есть вершины, называемые стоками: если песок попадает в такую вершину, то из неё он не имеет возможности уйти. Можно доказать, что в графе с хотя бы одним стоком обвалы рано или поздно прекратятся, причём их результат не зависит от порядка, в котором они совершаются.

Здесь мы будем рассматривать простейший случай этой модели: граф - квадратная сетка(степень каждой вершины равна 4, вершины - узлы сетки), изначально в каждой вершине 0 песчинок. Мы будем "кидать" в начало координат некоторое большое число песчинок и смотреть, во что это в конце концов превратиться. Также сделаем то же самое, только с другими правилами обвала в вершине.
