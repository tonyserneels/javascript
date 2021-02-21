Begin vanaf de code uit het onderdeel 'Class - Omschrijven - Opdracht 1':

- Zorg ervoor dat er gebruik gemaakt wordt van een constructor-methode.
- Maak gebruik van parameters in de constructor-methode om de properties een waarde toe te kennen.
- Schrijf de code om zodat de properties gezet worden tijdens het aanmaken van de instantie
  (in plaats van de properties een waarde toe te kennen nadat er een instantie gemaakt is).

```js
class Student {
  voornaam;
  achternaam;

  constructor(voornaam, achternaam) {
    this.voornaam = voornaam;
    this.achternaam = achternaam;
  }
  volledigeNaam(){
    let volledigeNaam = '';

    if (this.voornaam){
      volledigeNaam += this.voornaam;
  }

  if (this.achternaam){
    if (volledigeNaam.length > 0){
      volledigeNaam += '';
    }
    volledigeNaam += this.achternaam
  }
  return volledigeNaam;
  }
}

let student = new Student("Tony", "Serneels");
console.log(student.volledigeNaam());
```
