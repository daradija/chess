# Design Notes
# GPU Implementation

The first thing we studied is implementing the chess game using GPU.
The data structure representing the board would have the indices of:
- search 8 8

On these indices, the piece would be stored.
And at a global level in the search, the color of the player whose turn it is to play.

Similar to a doubly linked list, and knowing that there are no more than 32 pieces on the board, we can use the search index and type, the latter being one of the types of chess pieces and their color.

- search type

On this pair of indices, we would store the X, Y position of the piece, if it has died, if it has been promoted, and if it has been castled.

- X, Y, dead?, promoted, castled.

![alt text](image.png)

