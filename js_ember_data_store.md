## createRecord Methode
Erstellt ein neues Ember Data Objekt des Models.

```
this.get('store').createRecord('person')
```
Kann auch Initialwerte bekommen welche in diesen Record geschrieben werden.


```
let coolePerson = { name: 'Meerjungfraumann' }
this.get('store').createRecord(coolePerson, 'person')
```
**Hier wird aber der Record an die Variable coolePerson gebunden!!**

**Hier genauso:**

```
let coolePerson = { name: 'Meerjungfraumann' }
let coolerRecord = this.get('store').createRecord(coolePerson, 'person')
```

**Um den Record im nachinein ohne die coolePerson Referenz noch bearbeiten zu können muss man so vorgehen:**

```
let coolerRecord = this.get('store').createRecord('person')
coolerRecord.set('name', 'Meerjungfraumann')
```