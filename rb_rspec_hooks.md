Hooks welche zu einem gewissen Zeitpunkt während des Testdurchlaufes ausgeführt werden. Die Namen sind ziemlich selbsterklärend (so wie alles in rspec).

Hooks sind im aktuellen Scope aktiv.

```
before(:each) do 
      puts "Runs before each Test" 
   end 
   
   after(:each) do 
      puts "Runs after each Test" 
   end 
   
   before(:all) do 
      puts "Runs before all Test" 
   end 
   
   after(:all) do 
      puts "Runs after all Test"
   end
```
