class virtualPet {
    constructor(name) {
        this.name = name;
    }
    eat(food) {
        if (food === "dih") {
            console.log(`I hate gingers`);  
        } else {
            console.log(`We don't have victorys anymore`);
        }
        
    }
}

const pet = new virtualPet("dih");
pet.eat("dih");


class UserInfo {
    constructor (password) {
        this.password = password;
    }
}
class Passwords extends UserInfo {}
const password1 = new UserInfo("paygorn67");
const password2 = new UserInfo("dihcheese");
const password3 = new UserInfo("Icantgoon69!");
console.log(password1);
console.log(password2);
console.log(password3);


class Gamelevel {
  constructor(level) {
    this.level = level;
  }

  levelDisplay() {
    console.log(`You are level ${this.level}`);
  }
}

class Player1 extends Gamelevel {}
class Player2 extends Gamelevel {}

const status1 = new Player1(45);
const status2 = new Player2(90);

status1.levelDisplay(); 
status2.levelDisplay();


class Login {
    google() {
        console.log(`Logging in with google.`);
    }
}
class SignIn extends Login {
    facebook() {
        super.google();
        console.log(`Loggin in with Facebook.`);
    }
}
const a = new SignIn();
a.facebook();


class Human {
    constructor(weapon) {
        this.weapon = weapon;
        this.health = 100;
    }
    reciveDamage() {
        this.life = this.health - 10;
    }
    attack() {
        console.log(`Swings ${this.weapon}!`);
    }
}
class Warrior extends Human {
    constructor(weapon, warCry) {
        super(weapon);
        this.warCry = warCry;
    }
    recieveDamage() {
        this.health - 5;
    }
    attack() {
        super.attack();
        console.log(this.warCry);
    }
}
const human = new Human("axe...The human said this");
human.attack();
const warrior = new Warrior("sword", "Barritus!");
warrior.attack();
const donald = new Warrior("dih", "I hate gingers!...and dislexyia");
donald.attack();
