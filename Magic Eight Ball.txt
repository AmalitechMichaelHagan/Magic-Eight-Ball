let userName = '';
let userQuestion = '';
let eightBall = '';
let randomNumber = Math.floor(Math.random()*8);

userName ? console.log(`Hello, ${userName}!`) : console.log('Hello!');

console.log('Your Question is: ' + userQuestion);

//Switch statement that selects a random response based on the randomNumber variable
switch(randomNumber){
case 0: eightBall = 'It is certain';break;
case 1: eightBall = 'It is decidedly so';break;
case 2: eightBall = 'Reply hazy try again';break;
case 3: eightBall = 'Cannot predict now';break;
case 4: eightBall = 'Do not count on it';break;
case 5: eightBall = 'My sources say no';break;
case 6: eightBall = 'Outlook not so good';break;

default : eightBall = 'Signs point to yes';break;

}

//Logs the eightball message or displays an empty question prompt depending on the state of the userQuestion variable
userQuestion ? console.log(eightBall) : console.log('Hmmm, It appears you haven\'t put out a question yet. Let\'s try again.');
