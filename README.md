Uppgifter i JS

# Variabler

Variabler är en grund i JavaScript (och i alla andra programmeringsspråk) och det finns 3 olika sorter:
* let
* const (constant)
* var

De vanligaste att använda är _let_ och _const_ och i stort sett ingen använder _var_ längre i modern JavaScript. 

Man använder variabler för att 'spara' ett värde som man vill använda. Du kan spara vad du vill till en variabel, vare sig det är en siffra, en string, en array eller något annat. Skillnaden mellan _let_ och _const_ är att man kan **ändra** vad innehållet på en _let_ är, men inte på en _const_. Du definerar en variabel såhär:

## let
```
// Vi döper variabeln till variableOne och ger den värdet 0
let variableOne = 0

// Vi gör en till variabel som heter variableTwo men ger den inget värde den här gången
let variableTwo

// Eftersom variableTwo är en 'let' så kan vi ändra värdet på den när vi vill och hur vi vill. Här sätter vi den alltså till 2
variableTwo = 2

// Eftersom variableOne också är en 'let' kan vi också ändra dess värde till vad vi vill, även om vi redan satt att den ska ha värdet 0 där uppe där vi skapade den
variableOne = 1

// Om vi loggar (console.log) båda variabler nu kommer det skrivas ut 1 och 2 i konsolen:
console.log(variableOne) // Loggar 1
console.log(variableTwo) // Loggar 2

// Vi kan även sätta värdet på en variabel med en annan variabel:

variableOne = variableTwo // Det är alltid variabeln på vänstersidan som tar värdet av den på högersidan. variableOne tar alltså värdet av variableTwo här, dvs 2

console.log(variableOne) // Loggar 2
console.log(variableTwo) // Loggar också 2
```

## const 
```
// Vi döper variabeln till constVariableOne och ger den värdet 'hello'
const constVariableOne = 'hello'

// Vi gör en till variabel som heter constVariableTwo och ger den värdet 1
const constVariableTwo = 1

// Eftersom const är konstant kan vi inte ändra på den, oavsett vad vi gör. constVariableOne kommer alltid att vara 'hello'. Vi kan alltså inte göra:
constVariableOne = 'oogabooga' // Detta ger ett fel när vi försöker använda den här javascripten

// Eftersom vi inte kan ändra på värdet av variabeln kan vi alltså heller inte skapa en const utan värde (som vi kan med let)
const constVariableThree // Ger också ett fel

// Om vi loggar båda variabler nu kommer de visa det vi satte dom till från början:

console.log(constVariableOne) // Loggar hello
console.log(constVariableTwo) // Loggar 1
```

Båda variabeltyper är bra på sina olika sätt. Man kan använda dom för att t.ex. spara saker man inte orkar skriva om flera gånger:

```
const rollButton = document.getElementById('roll-button')

// Nu kan man skriva såhär
rollButton.addEventListener('click', () => console.log('hello))

// Istället för att skriva såhär
document.getElementById('roll-button').addEventListener('click', () => console.log('hello'))
```

eller för att spara saker som användaren trycker in på din hemsida, eller för att få spara värdet du får från en funktion (t.ex. Math.random()), bl.a. Man använder mycket variabler hela tiden i JavaScript och ändrar på värdet av dom ofta.

## Uppgifter:

Några uppgifter om variabler. När jag skriver "skapa en let/const" så kan du döpa den till vad du vill.

1. Skapa en let-variabel och ge den värdet _'hello'_.
2. Skapa en let-variabel utan att ge den ett värde (startvärde). Ändra sedan värdet på variabeln till _'hello'_ på raden under.
3. Skapa två let-variabler och ge den ena värdet 5 och den andra 10. Sätt värdet på den första variabeln (5) till värdet av den andra (10) genom att använda =-tecknet.
4. Skapa en const-variabel och ge den värdet _'hello'_. Logga värdet med en console.log().
5. Skapa två const-variabler och ge den ena värdet 10 och den andra 20. Skapa sen en tredje const-variabel som är summan av de två första variablerna adderade med varandra (variabel + variabel)
6. Med samma två const-variabler som ovan (10 och 20), skapa en tredje let-variabel som är variabel två (20) minus variabel ett (10). Logga sedan värdet på den tredje variabeln. Ändra sedan värdet på den tredje variabeln (på en ny rad, dvs att du inte ändrar raden där du definierar variabel tre) till 0 och logga det igen.
7. 
