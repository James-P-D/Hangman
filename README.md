# Hangman
Hangman game in SNOBOL

![Screenshot](https://github.com/James-P-D/Hangman/blob/main/screenshot.gif)

## Introduction

[Hangman](https://en.wikipedia.org/wiki/Hangman_(game)) is a game whereby the player has to guess the letters of a word. Each time the player fails to guess a letter correctly, a section of gallows is constructed, until the user either correctly guesses the word, or the gallows are complete and the player is dead.

## Technical Details

This program was written in [SNOBOL](https://en.wikipedia.org/wiki/SNOBOL) purely since it's a language that I've vaguely heard of, and wanted to investigate.

To run the script, you will need to download the interpreter from [Viktors Berstis' website](http://berstis.com/s4ref/snobol4.htm) and then install [DOSBOX](https://sourceforge.net/projects/dosbox/files/latest/download).  

From DOSBOX you will first need to mount the folder containing your SNOBOL code:

```
mount c C:\Users\jdorr\Desktop\Snobol
```

To run you code simply use:
```
SNOBOL4 HANGMAN.SNO /Q
```

You will then be prompted to choose one of the 10 words in the game's dictionary:

```
Welcome to Hangman!
Enter a number between 1 and 10
?2
______
```

You will then be prompted to guess the letters of the word. If you choose wisely, you will win the game:

```
Guess an uppercase letter
?B
B_____
Guess an uppercase letter
?N
B_N_N_
?A
Congratulations! You correctly guessed BANANA
```

If you choose poorly, you will lose:

```
_ANANA
?Q

Uh-oh!
+------+    
|/     |       
|      @    
|     \|/   
|      |    
|     / \   
|\          
+-----------

YOU ARE DEAD!
```