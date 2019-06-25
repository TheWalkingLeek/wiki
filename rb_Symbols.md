Symbols enthalten, wie Strings, Zeichenfolgen. Der Unterschied liegt darin, dass Symbols immer global sind und dadurch 2 Symbols mit demselben Inhalt auch den selben Hash enthalten.

Zu beachten dabei ist, dass man Symbols nicht für Nutzereingaben oder Ähnliches nutzt. Denn Symbols werden nicht vom Garbage Collector gelöscht und bleiben daher immer in der Memory.

Dadurch sind sie aber sehr nützlich für z.B. Hashes.


```
var = :symbol
```

