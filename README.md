# ДЗ 02 -- Мультимножество

**Дедлайн**: 09.12.2019 12:00:00 (100%), 16.12.2019 12:00:00 (50%).

### Условие
Требуется реализовать мультимножество на базе самобалансирующегося дерева (на выбор: AVL, красно-черное, декартово, 2-3, splay).

Примеры запросов, которые должно поддерживать мультимножество:
> $ val multiSet = MultiSet(4, 8, 15, 16, 23, 42, 42)
>
> [4 -> 1, 8 -> 1, 15 -> 1, 16 -> 1, 23 -> 1, 42 -> 2]
>
> $ multiset(42)
>
> 2
>
> $ multiSet & MultiSet(42)
>
> [42 -> 3]
>
> $ multiSet | MultiSet(108)
>
> [4 -> 1, 8 -> 1, 15 -> 1, 16 -> 1, 23 -> 1, 42 -> 2, 108 -> 1]

### Требования:
* Реализация основных операции над коллекциями;
* реализацяи операций пересечения (`&`) и объединения (`|`) коллекций; 
* поддержка функций высшего порядка, for-comprehension;
* реализация не должна использовать библиотеки коллекций: `Java`/`Scala`/`Guava` и т.д. (Это относится именно к реализации, в тестах использовать можно.)
* покрытие тестами: `JUnit 3/4/5` или [`ScalaTest`](https://www.scalatest.org/);
* использование [`sbt`](https://www.scala-sbt.org/) в качестве системы сборки;
* отсутствие дубликации кода.