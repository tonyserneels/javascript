```js
// Poging 1

class auto {
  merk;
  type;

  constructor(paramter1, parameter2){
  this.merk = parameter1;
  this.type = paramter2;
  }
  auto() {
    return '${this.merk} ${this.type}';
  }
}

let ferrari = new atuo("Ferrari","F50");
console.log(ferrari.auto());

// Poging 2

class auto{
  merk;
  type;

  constructor(merk, type){
    this.merk = merk;
    this.type = type;
  }
}
let ferrari = new auto('Ferrari', 'F50');
console.log(ferrari.merk, ferrari.type);

let lambo = new auto('Lamborghini', 'Countach');
console.log(lambo.merk, lambo.type);

let peugeot = new auto('Peugeot', '207');
console.log(peugeot.merk, peugeot.type);