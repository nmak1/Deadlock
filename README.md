# Задача №1. Deadlock

Для решения данной задачи добавлено

```
  val t1 =  thread {
        synchronized(resourceB) {
            consumerA.lockFirstAndTrySecond(resourceA, resourceB)
        }
    }
```

    val t2 =  thread {
       synchronized(resourceA) {
            consumerB.lockFirstAndTrySecond(resourceB, resourceA)
        }
    }
