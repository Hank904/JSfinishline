let blinkOn = false;
let blinkerInterval =  setInterval(() => {
    if (blinkOn) {
        console.log(`Blinker off`);
        blinkerOn = false;
    } else {
        console.log(`Blinker on`);
        blinkerOn = true;
    }
}, 500);
setTimeout(() => {
    clearInterval(blinkerInterval);
    console.log(`STOP!`);
}, 2500);

let countdown = 3;
const countdownInterval = setInterval(() => {
    if (countdown > 0) {
        console.log(countdown);
    }
    countdown--;
    if (countdown < 0) {
        clearInterval(countdownInterval);
        console.log("GO");
    }
}, 1000);

function callback() {
    console.log(`Oh i hate gingers`);
}
function calldih(){
    console.log(`Fuck gingers`);
}
console.log(`OOOOOOh`);
console.log(`oohhhh`);
setTimeout(callback, 1000);
setTimeout(calldih, 2000);

const greet = (name, callback) => {
    console.log(`Hello, ${name}!`);
    callback();
}

const sayGoodbye = () => {
    console.log(`Goodbye!`);
}
greet(`teresa`, sayGoodbye);

const promiseDemo = new Promise(function(){});

const orderCake = () => {
    return new Promise(function(resolve, reject) {
        if (dessertStock.cake > 0) {
            resolve(`cake available! Order processing.`);
        } else {
            reject(`Out of stock. Sorry baby.`);
        }
    });
}

function handleSuccess(successValue) {
    console.log(successValue);
}

function handleFailure(failureValue) {
    console.log(failureValue)
}
const makeOrder = orderCake();
makeOrder.then(handleSuccess).catch(handleFailure);
