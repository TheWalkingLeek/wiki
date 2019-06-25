Rails Validierungen werden im Model gesetzt.

Sollte man die Presence eines Booleans überprüfen wollen, muss man folgendes bedenken:

```
false.blank? --> true

```

presence validation arbeitet mit blank? deshalb ist nur noch true erlaubt

```
validates :boolean_field, presence: true --> erlaubt nur noch true

validates :boolean_field, exclusion: { in: [nil] } --> erlaubt false & true
```
