p3.neokobe.com
==============

by David Killeffer <rayden7@gmail.com> for CSCI-E 75, Fall 2012, Harvard University Extension School

My submission is a JavaScript implementation of the classic children's card game, War.
This is a very simple game.  A standard 52-card deck is shuffled and split between two
players, each player initially receiving getting 26 cards.  The object of the game is
to win all of the cards.

The rules for the game are explained in detail here:

http://www.pagat.com/war/war.html

This implementation uses jQuery, Underscrore.js Handlebars.js, and a modified JavaScript
Card/Stack library (for modeling a Card and a Stack of Cards).

The Underscore.js library is used to simplify array traversal.

The Handlebars.js library is used to declare HTML templates that are used for the actual cards.
Basic templates are defined that correspond to card ranks, but are irrespective of suit.  When
the index.html page is loaded and cards are randomly assigned to the player and opponent, the
Handlebars.js script "templates" are used to define card objects.  For details on how the
templates are used, see war-cards.js and look in the cardCreateNode() method.
