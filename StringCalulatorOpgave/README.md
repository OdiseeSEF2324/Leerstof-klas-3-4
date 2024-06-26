## Oefening String Calculator

### Opgave

Maak een IntelliJ project aan met de naam StringCalculator of herbruik deze.
Schrijf een methode `calculate` in de klasse `StringCalculator` die, op basis van een gescheiden reeks van getallen, de som van de getallen in de reeks optelt.
Deze methode heeft de volgende requirements
1. Een lege string resulteert in nul '' => 0
2. Een string met 1 getal resulteert in dat getal '1' => 1 '2' => 2
3. Een string met twee getallen gescheiden door een komma resulteren in de som '1,2' => 3 '10,20' => 30
4. Een string met twee getallen gescheiden door een enter/newline ("\n") resulteren in de som '1\n2' => 3
5. Een string met twee getallen gescheiden door een komma of een enter/newline ("\n") resulteren in de som '1\n2,3\n4' => 10
6. Een string met negatieve getallen resulteert in een exception met het bericht "Kan niet negatief zijn" '-1,2,-3' => 'Kan niet negatief zijn'
7. Getallen in de string groter dan 1000 worden genegeerd.

Implementeer de requirements achter elkaar en zorg steeds voor een test voor je begint met de volgende requirement.
Zorg ervoor dat er minstens 1 test is voor elke requirement en geef aan welke test welke requirement checkt.

Een aantal interessante lijnen code die je bij de oplossing kan gebruiken zijn:
```
        String s="a:b=c";
        s.split("[:=]");  //returns array {a,b,c}
        String n="5";
        Integer.parseInt(n); // returns integer 5
```