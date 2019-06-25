Sometimes, characters such as ä, ö or ü aren't being transferred the right way.
Use the characters unicode number and encode it in ruby.

```
character = "\u00C4"
puts character.encode('utf-8')
--> Ä
```
