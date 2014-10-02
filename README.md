public class Player{
        // Assigned upon player creation. Decides whether player is X or O on TicTacToeBoard.
        boolean isX = false;

        public int getMove(){
                int hi = 9001;
                return hi;
        }

        // Invoked upon the winning player as decided by boolean returned by TicTacToeBoard.update.
        public String winner(){
                String playerString = "";
                if(isX){
                        playerString = "X";
                } else{
                        playerString = "O";
                }
                String winning = "Game Over! Player" + playerString + "wins!";
                return winning;
        }

        // Invoked upon a player if board is filled and no winner is declared.
        public String tie(){
                String tie = "Game Over! Tie!";
                return tie;
        }

        // Set isX
        public void setX(boolean isX){
                this.isX = isX;
        }

        // Get isX
        public boolean getX(){
                boolean returnX = isX;
                return returnX;
        }
}
