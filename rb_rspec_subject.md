Ein Wert welcher gesetzt werden kann und im aktuellen Scope verfügbar ist.

```
subject { [1, 2, 3] }
describe "has some elements" do
    it "which are the prescribed elements" do
      expect(subject).to eq([1, 2, 3])
    end
  end
```
