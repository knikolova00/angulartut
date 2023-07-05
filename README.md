# Tic Tac Toe Game with Angular
This game was created using a great tutorial provided by Fireship - https://www.youtube.com/watch?v=G0bBLvWXBvc.

## Remarks
The tutorial is already three years old and there are some changes required to make the game work.

1. The Angular Console plugin used in the video is now called 'Nx Console'. I had trouble using the 'generate'
command (used for generating UI components) in version '18.4.0', downgrading to the previous version solved the issue. 
2. Nebular is not compatible with Angular 16, there is an issue raised for that (https://github.com/akveo/nebular/issues/3192) but it has not been fixed as of the time I am writing this. It seems like downgrading Angular would solve this problem, however if not possible you would have to use an alternative library or write some custom styling.
3. It occured to me that when there is a tie, no message is diplayed to indicate that. I added some logic to the ```calculateWinner()``` function to check if there is no winner and all squares are filled. Now the game also displays 'Draw!' when the game has finished but no one has one. 