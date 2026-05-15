# Gomoku / 五子棋

A browser-based Gomoku game originally developed by Kai as a college Java programming project in 2009, and ported to a modern webpage version in 2026.

The project preserves the original AI idea from the Java version: a weighted pattern-based evaluator that scores important Gomoku shapes such as fours, threes, twos, split patterns, and defensive points.

## Play

Open the hosted webpage in a desktop or mobile browser and click **Start Game**.

The game supports:

- Human vs Computer
- Human vs Human
- Computer vs Computer
- Optional forbidden-move rules for Black
- English and Chinese UI
- Desktop mouse play
- Mobile tap-to-zoom play

## Features

### Core Gameplay

- 15×15 Gomoku board
- Black moves first
- Five consecutive stones wins
- Optional Black forbidden-move rule:
  - Double-three
  - Double-four
  - Overline
- Undo support
- Clear board / restart support
- Win, loss, and draw display on the board

### AI

The AI is based on the original college Java project’s pattern-weight system.

It evaluates board positions by assigning weights to important move candidates, including:

- Immediate five
- Open four
- Split four
- Open three
- Blocked three
- Open two
- Semi-open two
- Single-stone development
- Defensive blocking points

The goal is not to implement a modern professional Gomoku engine, but to preserve and improve the original project’s simple, readable, pattern-based AI style.

### UI

- Clean modern responsive layout
- English / Chinese localization
- Automatic language detection with manual language selector
- Board coordinates on all four sides
- Optional AI weight display
- Optional move step-number display
- Smooth hover preview stone on desktop
- Mobile-friendly tap-zoom placement:
  - First tap zooms into the board
  - Second tap inside the placement area places a stone
  - Second tap near the edge zooms out without placing

### Save Game

Games can be exported as an SGF file using the **Save Game** button.

The exported file includes:

- Board size
- Move sequence
- Player information
- Rule mode
- Game result, when available

## Project Background

This project began as a Java programming assignment in college in 2009. The original version used Java classes and a pattern-based AI evaluator. In 2026, the project was ported into a standalone webpage so it can be played easily on phones and computers without installing Java.

The current version keeps the spirit of the original project while adding:

- Modern web UI
- Mobile support
- Bilingual interface
- Forbidden-move option
- SGF export
- Improved interaction and presentation

## Rules

Standard Gomoku rules:

- The board is 15×15.
- Black plays first.
- Players alternate placing stones on empty intersections.
- The first player to make five consecutive stones horizontally, vertically, or diagonally wins.

When forbidden moves are enabled:

- Black may not play a double-three.
- Black may not play a double-four.
- Black may not make an overline.
- White is not restricted by forbidden-move rules.

## Files

This project is packaged as a single HTML file.

No build step is required.

To run locally:

1. Download the HTML file.
2. Open it in a modern web browser.

To host online:

1. Upload the HTML file to a public web host or GitHub Pages.
2. Open the page URL from a phone, tablet, or computer.

## Technologies

- HTML
- CSS
- JavaScript
- Canvas rendering

No external framework is required.

## About

Originally developed by Kai as a college Java programming project in 2009. Ported to the web in 2026.
