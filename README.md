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
