# hangman
hangman is a weird game

## What's all this about?
This project was inspired by a [Jan Misali video](https://www.youtube.com/watch?v=le5uGqHKll8). I wanted to explore some interesting ideas that could go along with hangman, in particular, what the optimal algorithm might look like. Game tree search is well known to give the best result in a finite adversarial turn-based game.

## Notes
* As addressed in the video, hangman isn't exactly adversarial. And more importantly, it's not even turn-based. So we have to apply some heuristic instead of assuming the opponent makes the "best move". I take the average over the number of possible solutions given a particular guess, which seems to work well enough.
    * I could take the maximum to get something that works more like a traditional tree search. I might try doing that, since it would allow alpha-beta pruning + heuristic action ordering --> faster runtime.
* I spent about 12 hours on this project and barely slept. :(