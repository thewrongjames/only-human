# Only Human

## Introduction

Only Human is a simple tabletop RPG system for when you don't need / want the characters to have super human abilities. It is inspired by the [Dead Simple RPG](https://deadsimplerpg.wordpress.com/about/) game [Blaster](https://deadsimplerpg.wordpress.com/category/blaster-sf-rpg/) because I found it interesting, as well as D&D 5th Edition particularly and Pathfinder 2nd Edition, those are what I play the most of.

When I first saw the one page version of Blaster (3.5, I think), I was amazed at the idea that you could create a one page RPG that was more than just an (admittedly usually good) joke. It turns out that when you don't commit to providing an entire magic system, detailed progression, or setting, the solid foundations of an RPG system appear to be able to be rather light.

Fundamentally, what is needed for a role playing game is just a framework within which to adjudicate actions - a system of quantifying how good characters are expected to be at certain things, and whether or not (or the degree to which) they succeed at individual attempts of these things. Only Human tries to provide this.

At the moment these rules contain Only Human, which is a sort of base framework for game systems in which the players are not superheroes, and Still Human, which is a particular implementation of that framework in a near-future sci-fi setting.

## Structure

At the moment there are a couple of parts to this repo. The primary "end-user" facing component is `only-human.tex`, this is the LaTeX file that compiles into the rules pdf designed for players and GMs to read. If you wish to generate the rules file yourself you can see [the "Compiling" section below](#compiling), however, the easiest way to get those rules is from the [releases page](https://github.com/thewrongjames/only-human/releases).

In order to separate the rules from their layout, we also have the `design` folder. This contains `design/rules.md`, which should be the full rules free from any restrictions of layout. These will likely be more verbose than what you find in the generated PDF, so you can feel free to consult it if you find anything ambiguous. Or not. I'm not going to tell you that one is the source of truth. It's your game, not mine, pick whichever you like more.

The `design` folder also contains documents detailing design principles of various aspects of the game, so we have explicit notions of what we are going for, to aid in design.

## Compiling

I recommend compiling the rules with `xelatex`, and you will need the font Economica installed.
