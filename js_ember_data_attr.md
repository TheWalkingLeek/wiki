Der die attr Methode setzt ein Attribut auf ein DS.Model.


```
name: DS.attr('string'),
admin: DS.attr('boolean')

```

Es können auch Optionen mitgereicht werden. Bsp. ein defaultValue, sollte der erhaltene Wert nil sein.


```
name: DS.attr('string', { defaultValue: 'Batman' })
```

  
**!!ACHTUNG!!** null als defaultValue funktioniert nicht. Sollte null also erlaubt sein, muss man die allowNull Option nutzen.

```
admin: DS.attr('boolean', { allowNull: true })
```