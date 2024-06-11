# Scrabble Toolbox
Best move analysis for Scrabble

## Understanding the basic of scrabble
This toolbox will walk you through understanding the basic rules of Scrabble to play and master the game. You can also build and test your own Scrabble strategy.

## Use the default strategy
Use the default stategy to find the best move given a Scrabble board and your tile rack:

```matlab
% 1. Instantiation the default strategy
strategy = DefaultStrategy

% 2. Define the board
strategy.board = [
    ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ' ;
    ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ' ;
    ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ' ;
    ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ' ;
    ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ' ;
    ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', 't', ' ', ' ', ' ', ' ', ' ', ' ' ;
    ' ', ' ', ' ', ' ', ' ', ' ', 'h', 'a', 'r', 'e', ' ', ' ', ' ', ' ', ' ' ;
    ' ', ' ', ' ', ' ', 'p', 'h', 'a', 's', 'e', ' ', ' ', ' ', ' ', ' ', ' ' ;
    ' ', 'r', 'a', 'd', 'i', 'o', ' ', ' ', 'm', ' ', ' ', ' ', ' ', ' ', ' ' ;
    ' ', ' ', ' ', ' ', ' ', 'l', ' ', ' ', 'o', ' ', ' ', ' ', ' ', ' ', ' ' ;
    ' ', ' ', ' ', ' ', ' ', 'd', ' ', ' ', 'r', ' ', ' ', ' ', ' ', ' ', ' ' ;
    ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ' ;
    ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ' ;
    ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ' ;
    ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ' ;
]

% 3. Define the tile rack
strategy.tiles = ['a', 't', 'x', 'o', '?', 'e', 'l']

% 4. Get best move
strategy.getBestMove()
```

## Building a Scrabble strategy
Use the following steps to generate a scrabble strategy:

```matlab
% 1. Create a strategy object
strategy = Strategy

% 2. Assign the strategy
strategy.basis = 'Target plays that make multiple words and triple word scores'
```
