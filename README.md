<div align="center">
  <h1>SocketTicTacToeGUI</h1>
  <p><strong>Two-player networked tic-tac-toe with Python sockets, Tkinter windows, and game statistics.</strong></p>
  <p>
    <img alt="Python" src="https://img.shields.io/badge/Python-303840?style=flat-square" />
    <img alt="Tkinter" src="https://img.shields.io/badge/Tkinter-303840?style=flat-square" />
    <img alt="Sockets" src="https://img.shields.io/badge/Sockets-303840?style=flat-square" />
  </p>
  <p><a href="#overview">Overview</a> · <a href="#getting-started">Getting started</a> · <a href="#repository-map">Repository map</a></p>
</div>

---

## Overview

A two-player tic-tac-toe exercise using TCP sockets for communication and separate Tkinter windows for each player.

## What’s inside

- Host a game and connect a second player.
- Exchange player actions over a TCP connection.
- Track wins, losses, ties, and turns through a shared game-board class.

## Getting started

Use Python 3 with Tkinter installed. Start the server window first:

```sh
python player2.py
```

In another terminal, start the client:

```sh
python player1.py
```

For a local game, enter `127.0.0.1` and the same unused port in both windows. Start listening in Player 2 before connecting Player 1. The naming follows the original files: Player 2 hosts the server.

## Repository map

| Location | Purpose |
| --- | --- |
| [`player2.py`](./player2.py) | Server and Player 2 window |
| [`player1.py`](./player1.py) | Client and Player 1 window |
| [`gameboard.py`](./gameboard.py) | Board state, win detection, and statistics |

## Project status

Educational networking project. Socket operations are synchronous and the protocol is intended for local/trusted demonstrations, with no authentication or encrypted transport.
