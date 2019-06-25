Enums werden in der Migration und der Datenbank als Integer definiert.

Im Model definiert man die Werte dann so:

```
enum company_type: %i[mine candidate external other]
```

**{enum}_before_type_cast:**

```
c = Company.find_by(company_type: 'mine')
c.company_type_before_type_cast
=> 0
```

**{record}.{enum_value}?:**

```
c = Company.find_by(company_type: 'mine')
c.mine?
=> true
```