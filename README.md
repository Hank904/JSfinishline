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
