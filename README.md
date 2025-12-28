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
