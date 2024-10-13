# Java Chess Game

## Project Overview

This Java-based chess game implements a fully functional two-player chess system with a graphical user interface. The project comprises two main classes: `ChessGame` and `Piece`, which work together to create an interactive chess playing experience.

## Features

1. **Graphical User Interface**: The game uses Java Swing to create a visual chessboard with piece images.
2. **Complete Chess Rules**: Implements all standard chess moves, including:
   - Basic moves for all pieces (Pawn, Rook, Knight, Bishop, Queen, King)
   - Special moves:
     - Castling (Kingside and Queenside)
     - En Passant capture for pawns
     - Pawn promotion
3. **Move Validation**: Ensures all moves adhere to chess rules, including:
   - Piece-specific move patterns
   - Preventing moves that would put the player's own king in check
   - Handling pinned pieces
4. **Check and Checkmate Detection**: Identifies when a king is in check and detects checkmate scenarios.
5. **Stalemate Detection**: Recognizes when the game ends in a draw due to stalemate.
6. **Turn-based Gameplay**: Alternates turns between white and black players.
7. **Move Highlighting**: Shows valid moves for the selected piece.
8. **Pawn Promotion**: Allows pawns that reach the opposite end of the board to be promoted.

## Class Structure

### ChessGame Class
- Manages the overall game state
- Initializes the game board and pieces
- Handles user input (mouse events)
- Implements game logic (turn management, endgame conditions)
- Renders the game board and pieces

### Piece Class
- Represents individual chess pieces
- Implements move generation for each piece type
- Handles move validation
- Manages special moves (castling, en passant)

## Game Controls

- Click and drag pieces to move them.
- Valid moves are highlighted in yellow when a piece is selected.
- The game automatically switches turns after each valid move.
- Pawn promotion is handled automatically when a pawn reaches the opposite end of the board.

## Technical Details

- **Image Handling**: The game uses a sprite sheet (`chess.png`) to render chess pieces.
- **Move Validation**: Implements complex algorithms to ensure all moves are legal, including checking for pins and checks.
- **AI**: The current version does not include an AI opponent. It's designed for two human players.

## Future Enhancements

1. Implement an AI opponent using algorithms like Minimax with Alpha-Beta pruning.
2. Add a move history feature to allow undoing moves.
3. Implement a save/load game feature.
4. Add network functionality for online multiplayer.
5. Improve the UI with additional features like a timer, captured pieces display, etc.

## Dependencies

- Java Development Kit (JDK) 8 or higher
- Java Swing library (included in standard JDK)

## Contributing

Contributions to improve the game or add new features are welcome. Please fork the repository and submit a pull request with your changes.

