# bluejj66
about me
function guessNumber() {
    const targetNumber = Math.floor(Math.random() * 10) + 1;
    let attempts = 0;
    
    while(true) {
        let userGuess = parseInt(prompt("Guess a number between 1-10:"));
        attempts++;
        
        if (userGuess === targetNumber) {
            alert(`Congratulations! You guessed in ${attempts} attempts`);
            break;
        } else if (userGuess < targetNumber) {
            alert("Too low, try again!");
        } else {
            alert("Too high, try again!");
        }
    }
}

guessNumber();
