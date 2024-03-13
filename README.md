## Исследование и применение различных алгоритмов кластеризации для сегментации типов давижений человека и анализа изображений.

Асташов И.В., 2024.

Проект выполнен в рамках курса «Машинное обучение» магистерской программы НИУ ВШЭ [«Машинное обучение и высоконагруженные системы»](https://www.hse.ru/ma/mlds/).


## Цель и задачи

**Цель**: Исследовать различные методы кластеризации для сегментации типов движений человека и анализа изображений для выделения семантических компонент.

**Задачи:**

1. Стандартизировать табличные данные активностей человека.
2. Провести понижение размерности данных с использованием метода главных компонент **(PCA)**.
3. Визуализировать данные в проекции на первые две главные компоненты.
4. Провести анализ результатов кластеризации данных с использованием следующих алгоритмов: **KMeans, Agglomerative Clustering, DBSCAN, HDBSCAN и Spectral Clustering**.
5. Подобрать оптимальные гиперпараметры для каждого алгоритма и оценить их качество с использованием метрик **Silhouette Score, Adjusted Rand Index (ARI), Adjusted Mutual Information (AMI) и V-measure**.
6. Разделить предложенные изображения на семантические компоненты с использованием **спектральной кластеризации** и **KMeans**, подобрав оптимальные гиперпараметры для каждого метода.
7. Сравнить качество сегментации и проанализировать полученные результаты.


## Анализ результатов кластеризации движений человека

Проведена кластеризация данных активности человека с использованием нескольких алгоритмов. Лучшие результаты по метрикам качества продемонстрировала спектральная кластеризация, хотя этот метод требовал наибольшего времени обучения. Agglomerative Clustering оказался самым быстрым алгоритмом, его качество кластеризации оказалось несколько хуже.

## Сегментация изображений

Проведена сегментация изображения с использованием спектральной кластеризации и KMeans. Для каждого метода были подобраны оптимальные гиперпараметры. Спектральная кластеризация продемонстрировала лучшее качество сегментации по сравнению с KMeans.