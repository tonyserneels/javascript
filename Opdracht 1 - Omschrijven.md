```js
// 1. Aanmaken van een class genaamd Student
class Student {
  // 2. Property voornaam
  voornaam;
  // 3. Property achternaam
  achternaam;

  // 4. Functie VolledigeNaam aangemaakt
  volledigeNaam() {
    let volledigeNaam = "";

    if (this.voornaam) {
      volledigeNaam += this.voornaam;
    }

    if (this.achternaam) {
      if (volledigeNaam.length > 0) {
        volledigeNaam += " ";
      }
      volledigeNaam += this.achternaam;
    }

    return volledigeNaam;
  }
}

/*
 * 5.
 Toekennen van een nieuwe instantie van de class Student aan de variabele genaamd student.
 De waarde is een instantie van de class.
 Een instantie is een object met de properties en functies die gedefnieerd staan in de class.
 Het type is Object.
 */
let student = new Student();
student.voornaam = "John";
student.achternaam = "Duck";
console.log(student.volledigeNaam());

let studentEnkelVoornaam = new Student();
studentEnkelVoornaam.voornaam = "John";
console.log(studentEnkelVoornaam.volledigeNaam());

let studentEnkelAchternaam = new Student();
studentEnkelAchternaam.achternaam = "Duck";
console.log(studentEnkelAchternaam.volledigeNaam());
```