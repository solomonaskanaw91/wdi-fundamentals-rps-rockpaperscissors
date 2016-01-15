'use strict';

function getInput() {
    console.log("Please choose either 'rock', 'paper', or 'scissors'.")
    return prompt();
}
function randomPlay() {
    var randomNumber = Math.random();
    if (randomNumber < 0.33) {
        return "rock";
    } else if (randomNumber < 0.66) {
        return "paper";
    } else {
        return "scissors";
    }
}


var winner = "";
var playerMove = "";
var computerMove = "";


function getPlayerMove(move) {

    return move || getInput();
}

function getComputerMove(move) {

    return move || RandomPlay();
}

function getWinner(playerMove,computerMove) {
    var winner;
if (playerMove ==="rock") {

  if (computerMove === "rock") {

	winner = "tie";
 }
 else if (computerMove === "paper") {
	winner = "computer";
 }

 else {
    winner = "player";
  }
}

else if (playerMove === "scissors") {
     if (computerMove === "scissors") {
	    winner = "tie";
	}

else if (computerMove === "rock") {
     winner="computer";
 }
 else {
     winner = "player";
 }
}
else {
     if (computerMove === "paper") {
        winner = "tie";
  }
 else if (computerMove === "scissors") {
       winner = "computer";
}
 else {
     winner = "player";
	}
}

    return winner;
}

function playToFive() {
    console.log("Let's play Rock, Paper, Scissors");
    var playerWins = 0;
    var computerWins = 0;
 while (playerWins < 5 && computerWins < 5) {
	playerMove = getPlayerMove();
	computerMove = getComputerMove();
	winner = getWinner(playerMove,computerMove);

   if (winner === "player") {
	console.log("Player chose" + playerMove + " and computer chose" + computerMove + ". Player wins this battle, not the war.");
	playerWins++;
}
    else if (winner === "computer") {
	console.log("Player chose" + playerMove + "and computer chose" + computerMove + ". Computer wins this battle, not the war.");
	computerWins++;
}
    else if (winner === "tie"){
	console.log("It's a tie!");
}
    console.log("The score is now" + playerWins + "to" + computerWins + ".");
}
    return [playerWins, computerWins];
}
