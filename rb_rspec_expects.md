Stellt Erwartungen auf. Erwartet beispielsweise den Call einer angegebener Methode. 

```
expect(bob_attrs.count).to eq(11)
```
Kann auf Mocks genutzt werden um den Return Wert zu steuern. 

```
expect_any_instance_of(Odt::Fws).to receive(:export).exactly(1).times
```

Parametervorgaben setzen (e.g Methode x soll einen Call mit parameter y erhalten)

```
expect(bob).to receive(:bar).with("an argument I want")
```
Errors erwarten

```
expect { bob.fly }.to raise_error

```
**!!ACHTUNG!!** ist kein and_return Parameter gesetzt, wird die Methode so gestubbt, dass sie nil returned!

Weitere nützliche Matchers: https://relishapp.com/rspec/rspec-expectations/docs/built-in-matchers