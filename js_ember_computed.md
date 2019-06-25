Computed properties werden für Werte genutzt, welche sich während dem existieren in einer View verändern. Bsp. ein Chatverlauf. Das Computed Property funktioniert dann ähnlich wie ein observable und benachrichtigt alle Views, welche das Property nutzen, bei einer Änderung neu zu laden.

## Import:

```
import { computed } from '@ember/object';
```

## Definieren eines Properties:

```
amountOfEducations: computed('educations.@each', function() {
    return this.get('educations.length')
}),
```

## volatile
Die volatile Methode stoppt das computed Property, bei Updates der Value die View zu updaten. Dies kann genutzt werden, wenn zum Beispiel eine sortierte Liste beim Bearbeiten nicht aktualisiert werden soll.

```
amountOfEducations.volatile()

```