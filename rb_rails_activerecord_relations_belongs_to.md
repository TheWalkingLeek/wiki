Belongs_to bezeichnet eine 1:x Beziehung.

```
class Book < ApplicationRecord
   belongs_to :author
end
```
**Rails 5:** Die Beziehung, bzw der Foreign key ist ab Rails 5 standartmässig **Not Null.** Um diesen wieder nullable zu machen braucht man den Parameter **optional:true**