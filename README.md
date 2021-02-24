# Factorial
Compute a factorial of a number

const readline = require('readline').createInterface({
    input: process.stdin,
    output: process.stdout
  })
  
  readline.question(`Enter a number to compute factorial: `, (number) => {

    let fact = 1;
    for (let i = 1; i <= number; i++){
        fact = fact * i;
    }
    console.log("Factorial " + number + " = " + fact);
    readline.close();
  });
