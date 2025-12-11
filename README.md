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
