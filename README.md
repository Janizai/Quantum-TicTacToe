# Tic Tac Toe with qubits
Python script that requires pygame and qiskit. Start a game by executing the python file [tictactoe.py](./tictactoe.py).

# The Game
In this version of Quantum Tic Tac Toe, each player can perform either
2 unitary moves or 1 measurement during their turn. Every 10 turns the
board is measured and collapsed to classical bits. 

The first to form a line of classical markings wins.

The circuit representation is printed out every turn. Also if a player tries to perform an invalid move, this is printed out as well, along with the reason why it's not allowed.

## Moves
The desired move is chosen by pressing the corresponding key and the
qubit is chosen by hovering over it with the mouse.
* q - Place a qubit with the current player's mark.
* h - Operate on the selected qubit with a Hadamard gate.
* x - Operate on the selected qubit with an X gate.
* m - Measures the selected qubit.
* s / spacebar - Ends the current player's turn.

## Rules
1. Players make 2 unitary operations or 1 projective operation on a box.
2. Unitary operations: initiate a qubit, X gate, and Hadamard gate.
3. Projective operator will collapse a qubit into a classical bit.
4. The player with 3 classical bits in a straight line wins.