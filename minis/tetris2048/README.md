# A Tetris 2048 Clone
Written using React framework.  

I haven't spent much time on polishing the game, like moving the tiles smoothly pixel by pixel, or adding effects to the merging of the tiles.  

My intent was to implement a simple game in React which has a game loop that utilizes `window.requestAnimationFrame` and a `Game` component that updates according to the ticks of this loop.  

## Short summary of the components
`Tile` component is a stateless component that takes care of rendering a tile. A tile is a 106px by 106px square which shows a number in the relevant style.  

`Board` component is also a stateless component that generates the `Tile` components and determines their position on the screen.  

`Game` component is the main entry component which takes care of the game logic. It handles the creation of the tiles, movement of the tiles based on keyboard events triggered by the user, merging of the tiles, and determining the game status.  

`Overlay` component renders an overlay on top of the board, so that the user is informed about the game status and ables the user to restart the game. It is stateless component and triggers the `restartGame` defined in `Game` component.  
