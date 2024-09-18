# Store - Uppgift

## Table of Contents
### [Side Quests](#side-quests)
### [Del.1](#del1)
### [Del.2](#del2)
### [Del.3](#del3)
### [Del.4](#del4)

<br>

## Side Quests:
- Töm cart efter checkout
- Sätt att se alla tillgängliga commands, t.ex. att `help` visar alla tillgängliga commands
- Command för att se `balance`
- Lägg till ett saldo till alla föremål: `amountInStock`
- Ge respons på om man skriver in fel command, föremål eller om man har för lite pengar
- Lägg till så att om man skriver en siffra efter föremålet så kan man köpa/ta-bort *n*-mängd föremål: `add glasses 5` lägger till 5 glasögon i kundvagnen och `remove glasses 5` tar-bort 5 glasögon
- Fixa så att input kan ta in strängar som inte bryr sig om versaler och gemener, t.ex. `AdD GlasSeS`  => `add glasses` 
- Lägg till ett command för att stänga av programmet
- Ändra

<br>

## Del.1
Skapa en konsollapplikation som skall agera som en affär. Affären ska ha minst tre varor med tre olika priser. När namnet eller en förkortning av namnet skrivs in i konsolen ska kostnaden av varan dras bort ifrån kundens saldo.

### Kriterier:
- Tre varor med tre priser
- Saldo som ändras när man köper en vara

### Länkar:
- [User Input - W3Schools](https://www.w3schools.com/cs/cs_user_input.php)
- [Switch Statements - W3Schools](https://www.w3schools.com/cs/cs_switch.php)
- [While Loop - W3Schools](https://www.w3schools.com/cs/cs_while_loop.php)

<br>

## Del.2
Uppdatera affären så att den nu har en kundkorg där man kan lägga till och ta bort varor. Skriv ut varor i kundkorgen, deras styckpris och totalpris i konsolen.

En kund ska kunna betala för det som finns i deras kundkorg varpå totalkostnaden ska dras ifrån kundens saldo. Om det inte finns tillräckligt mycket pengar på kontot ska kunden inte kunna betala för varorna.

### Kriterier:
- Kundkorg med funktionalitet för att lägga till, ta bort och betala.
- Kunna se vara, mängd, styckpris och totalkostnad.

**OBS** - Om det är för svårt att ta bort från kund korgen så skippa det tills vidare

### Länkar:
- [Arrays - W3Schools](https://www.w3schools.com/cs/cs_arrays.php)
  
<br>

## Del.3
Nu ska vi skapa några metoder för att återanvända funktionalitet

`DisplayItems()` : ska ta in en array/dictionary av alla föremål som en parameter, iterera igenom dem och skrivat ut namnet och värdet på alla föremål. 

Exempel:

```csharp
Console.WriteLine($"- {namn} : {pris}")
```

<br>

`AddToCart()` : ska ta in en ``cart`` och `name` samt `price` på ett föremål som parametrar. Om ett föremål med samma namn redan finns i din `cart` så ska kostnaden på föremålet i carten ökas med föremålets pris. D.v.s. om det finns en penna med värde 5kr i cart så ska värdet på penann i kart bli till 10 kr. Om föremålet inte redan finns i carten så lägg till den i carten.

När ett föremål lagts till eller fått ett uppdaterat värde så ska metoden returnera den uppdaterade carten

<br>

`RemoveFromCart()` : ska ta in en ``cart`` och `name` samt `price` på ett föremål som parametrar. Om ett föremål med samma namn som `name` från parametern så ska värdet på föremålet subtraheras med `price`. Om värdet på föremålet i cart är samma som `price` så ska föremålet tas bort ifrån `cart`. 

I det fall att det inte finns ett föremål med samma namn som `name` i carten så ska metoden returnera carten utan att ta bort någonting. Annars så ska metoden returnera den uppdaterade carten.

### Kriterier:

### Länkar: 
- [Methods - W3Schools](https://www.w3schools.com/cs/cs_methods.php)
- [Dictionary - TutorialsTeacher](https://www.tutorialsteacher.com/csharp/csharp-dictionary)

<br>

## Del.4
Skapa två klasser, `Cart` och `Item`. `Cart` ska innehålla ett property som är en lista med items och en som håller i summan för alla items. `Item` ska ha tre properties, Namn på en vara och vad den kostar.

### Kriterier:
#### Cart
- Lista med items
- Summa

#### Item
- Namn
- Kostnad

### Länkar:
- [Classes - W3Schools](https://www.w3schools.com/cs/cs_classes.php)