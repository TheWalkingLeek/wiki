Blocks in Ruby können sowohl in Procs, als auch in Lambdas erstellt werden.

Allerdings sind Lambdas auch Proc Objekte!

## Unterschiede
* Lambdas überprüfen die Anzahl Parameter
* return wird anders genutzt. Falls return in einem Proc aufgerufen wird, bezieht sich dieses return auf die Methode. Bei Lambdas auf den Block