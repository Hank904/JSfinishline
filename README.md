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


class userInfo {
    constructor (email, username, password) {
    }
}
const user1 = new userInfo("dih@gmail.com", "hank11", "Icantgoon");
const user2 = new userInfo("donald@gmail.com", "donald", "paygorn");
console.log(user1);
console.log(user2);
