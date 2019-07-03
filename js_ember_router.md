# js_ember_router

## Methods

### transitionTo

Die transitionTo Methode kann ein redirect zu einer anderen Route machen.
Dabei gibt es aber verschiedene Möglichkeiten und die Dokumentation ist da eher zurückhaltend.

1. `this.get('router').transitionTo('people.index')`
2. `this.get('router').transitionTo('people/18')`
3. `this.get('router').transitionTo('people.person', person)`
4. `this.get('router').transitionTo('people.person', person, { queryParams: { rated: true } })`

**Bei den QueryParams ist diese Verschachtelung sehr wichtig!**
