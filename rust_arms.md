# Rust Arms

## arm pattern

An arm pattern is what gets matched against. Interesting is, that you can also use conditionals in the pattern.

```
let mut v = vec![Foo { a: Baz }, Foo { a: Qux }, Foo { a: Dunnowhatsnext }];
    let pop_result = match v.pop() {
        Some(x) if x.a == Bar::Dunnowhatsnext => { println!("matched: {:?} so re-pop", x); v.pop() },
        Some(x) => Some(x),
        None => None
    };
```
