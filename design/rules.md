This file exists to document the rules in a setting not constrained by layout, it will hence likely be more explicit than the final document.

# Only Human

Only Human is a simple framework for tabletop role playing games, for when you don't want the characters to be super-human. It requires a game master (GM) to control the world and the non-player characters (NPCs) and to adjudicate the outcomes of player actions, and at least one player to control the player character(s) (PCs).

Only Human does not provide a setting or any of the rules associated with that, but this document also provides an implementation of the framework called [Still Human](#still-human), detailed later in this document. Still Human is fleshed out enough to be actually played as a game, but you can of course add to it, or to create other implementations of the framework.

This section contains the basic rules for playing the game, as they pertain to the players. The GM will also use some of these rules, but there are more details provided for them in [GM Guide](#GM-Guide). Additionally, every term that appears in **bold** is a keyword. Whilst they are explained when they are first used, definitions are also provided in the [Keywords](#keywords) section.

Before playing, each player and the GM should have access to at least one d20 (d20s are 20 sided dice), as well as some paper, pencils and erasers to record character details and notes. The GM should have an interesting story or scenario for the player(s) to encounter, and outlines of any special mechanics that they expect to use during the game.

## Character Creation

Before playing the game, the players each create a character. To do so the players must pick a **role**, and assign points to the character's **stats** and **skills**. **Roles** are part of implementations of Only Human, so you can find some examples in the Still Human section below. Whatever the implementation, a role will have associated **skills**, and will also confer starting equipment. Your GM will tell you what your options are.

In Only Human, characters have four **stats** that represent their innate strengths and weaknesses. These are `DEX` (dexterity), `INT` (intelligence), `STR` (strength), and `WIL` (will, as in will power) In this document **stats** will always be presented in `THIS` format. They also have **skills** which represent specific training they have received in particular fields. In this document **skills** will always be presented in _This_ format. Together these quantify how competent a character is at any task they may attempt. You should record the values assigned to these **stats** and **skills** in a physical or digital document for reference whilst playing the game. We call this document your **character sheet**.

Whilst the numerical aspects of character creation take up most of this section, your character should be much more than just numbers. Work with the GM to plan details such as their personality, what they want, what they need (but might not know they need), their friends, their family, how they know the other characters in the group and how any of this can tie into the adventure. Your character will of course also need a name. Have secrets for your character, but want them to be discovered. Note this all down on your **character sheet**.

To create a character, you must allocate **points** to the characters **stats** and **skills**. You must allocate `4` **points** between the character's **stats**, giving at most `2` **points** to any particular **stat**. For example, you could put two points into `DEX`, one point into `INT`, no points into `STR` and one point into `WIL`. A **stat** having more points indicates your character is more innately talented in that area. Record the number of points you have assigned to each **stat** on your character sheet.

For **skills**, you must allocate `6` **points** to any of the **skills** associated with your **role**, and an additional `12` **points** freely to any **skill** (including those associated with your **role**). Whatever the source of the points, you may allocate at most `6` **points** to any particular **skill**. Similarly to **stats**, having more points in a **skill** indicates that your character has had more practice or training in that area.

There is no fixed list of **skills**, in principle anything can be a **skill**, at the discretion of the GM. The **skills** listed below provided an example of how specific or broad any added **skills** should be. If a character has not assigned any **points** to a particular **skill**, they are simply regarded as having `0` **points** in that **skill**. Every **skill** must be associated with a pair of **stats**, but they may be associated with the same **stats** twice.

Below are lists of **skills**, following their associated **stats**. An * (an asterix) indicates that the **skill** is a **defensive skill**, and a † (a dagger) indicates that the **skill** is an **offensive skill**. Exactly what this means will be discussed later, in the [Attacking](#attacking) section. For now, simply ensure that group each of these groups of skills together on your **character sheet**.

All the **skills** in this first list are required for the core operation of the game. These should be detailed on every character's **character sheet**, even if that character did not assign **points** to some of them, for ease of reference. A particular implementation of Only Human may add more core **skills** (which may be **offsenvie skills**, **defensive skills**, or neither), or split these skills into multiple more specific skills.

- `DEX` + `DEX`: _Evasion_*
- `DEX` + `INT`: _Ranged Attacking_†
- `DEX` + `STR`: _Speed_
- `DEX` + `WIL`: -
- `INT` + `INT`: _Medicine_
- `INT` + `STR`: _Melee Blocking_*
- `INT` + `WIL`: -
- `STR` + `STR`: _Melee Attacking_†
- `STR` + `WIL`: _Endurance_
- `WIL` + `WIL`: -

The **skills** on this second list are simply examples of common things characters may be skilled in, though some of them of course depend on the setting. These skills, and any others not listed here or above don't need to be included on the **character sheets** of characters that have not allocated any points to them.


- `DEX` + `DEX`: _Slight of Hand_
- `DEX` + `INT`: _Driving_, _Piloting_, _Riding_
- `DEX` + `STR`: -
- `DEX` + `WIL`: _Stealth_
- `INT` + `INT`: _Investigation_, _Science_
- `INT` + `STR`: -
- `INT` + `WIL`: _Insight_, _Performance_
- `STR` + `STR`: _Athletics_
- `STR` + `WIL`: _Intimidation_
- `WIL` + `WIL`: _Animal Handling_, _Persuasion_

There are two important numbers associated with each of your character's **skills**, the **skill's** **modifier**, and the **skill's** **DC**. Each represent the same thing: how competent overall your character is with the **skill**. However they are used in different ways, a **modifier** is for when you are taking an action, and a **DC** is for when someone is taking an action against you. Both are explained in more detail in the [Tests](#tests) section below.

A **skill's** **modifier** is calculated by taking the number of points the character has allocated to each of the **stats** associated with the **skill** and adding those two numbers to the number of points the character has allocated to the **stat** itself. If a **skill** is associated with the same **stat** twice, the points in that one **stat** are skill added twice. A character's **DC** in a particular **skill** is simply their **modifier** in that **skill** plus `10`. You should note both these numbers down alongside their respective **skills** on your **character sheet**.

For example, a player have have allocated `1` point to their character's `DEX` **stat**, `2` points to their character's `INT` **stat**, `5` points to their character's `Ranged Attacking` **skill**, and `3` points to their character's `Slight of Hand` **skill**. Their character would then have a _Ranged Attacking_ **modifier** of `1 (DEX) + 2 (INT) + 5 (Ranged Attacking) = 8` and a _Ranged Attacking **DC** of `7 + 10 = 17`. Further, their character would have a _Slight of Hand_ **modifier** of `1 (DEX) + 1 (DEX) + 3 (Slight of Hand) = 5` and a _Slight of Hand_ **modifier** of `5 + 10 = 15`.

## Tests

Whenever a character does something, the GM adjudicates and narrates the outcome. If the character's (attempted) action has a risk of meaningful failure, and a chance of success, the adjudication is usually done by having the character take a **test**. A **test** must always be associated with a **skill**. As a player, you should not ask the GM if you can take a **test**, you should simply tell them what your character is doing, and they will tell you whether you need to take a **test**, and what **skill** it should be in. However, as there is not limit to the number of **skills** in Only Human, once a test is called for you should feel free to recommend an alternate, perhaps more relevant, **skill**.

To take a test, the controlling player of the character in question, or the GM for NPCs, rolls a d20 and adds the character's **modifier** in the relevant **skill**.

TODO:
- Major success and major failure on 10 above or 10 below.

## Turns

When things get tense, whether that is because a fight has broken out in the tavern, or because there is a leak in an airlock with seconds to patch, characters start taking turns.

### Moving

### Interacting

### Attacking

- TODO:
  - Attacker rolls against some kind of evasion to hit, maybe the defender can pick what they are using, depending on whether it is a melee or ranged attack.
    - Hit is severity 1, critical hit is severity 2.
    - Armour provides different defence options, but perhaps only against certain kinds of attacks, or certain damage types (or maybe the damage resistance applies to the next roll?).
  - Defender rolls some kind of resistance.
    - Critical failure increases the severity by 1, success decreases by 1, critical success decreases by 2.
    - Maybe the DC is determined by the weapon.
    - Maybe different weapons have different DCs for whether the hit is a critical or not (i.e. a critical knife wound may be much harder to resist than a normal one, and maybe for some weapons they are no different)
  - If the resulting severity is 1 or more, the defender's health state decreases by that amount and they become unstable.

### Readying

## Injury

# Still Human

Still Human is an implementation of the Only Human framework. It is designed to run games for teams of trained or experienced characters that are sent on, or somehow end up entangled in, various missions in reasonably hard sci-fi near-ish future settings, though that could perhaps be adapted.

## Roles

# GM Guide

## Running the Game

### Setting DCs

| Difficulty             | **DC** | Explanation |
| :--------------------- | ------:|:----------- |
| Very Easy              |    `5` | Even a normal person will probably succeed. |
| Easy                   |   `10` | A normal person is slightly more likely than not to succeed, an expert cannot fail. |
| Moderate               |   `15` | A normal person will probably fail, an expert will probably succeed. |
| Very Difficult         |   `20` | A normal person only has a slim chance of success, an expert is slightly more likely than not to succeed. |
| Incredibly Difficult   |   `25` | Even an expert will probably fail. |
| Practically Impossible |   `30` | Even an expert only has a slim chance of success. Any higher is impossible |

### Deciding Who Rolls

### Adjudicating Complex Tasks

### Turns

## Making Adventures

### Making NPCs

### Making Monsters

## Adding to the Game

### Making an "Implementation"

### Progression

# Keywords

- **Character sheet**:

- **DC**:

- **Defensive Skill**:

- **Modifier**: A **modifier** is a number representing how capable a character is with a given **skill**. The **modifier** for a **skill** is calculated by adding the **points** the character has in each **stat** associated with the **skill** (note that if it is associated with the same **stat** twice, the **points** in that **stat** are still added twice) to the **points** the character has in that **skill**.

- **Offensive Skill**:

- **Points**: During character creation a player assigns a certain number of points to a character's **stats** and **skills**. These are used to determine a character's **skill** **modifiers**.

- **Roll**:

- **Skill**: A **skill** is a particular thing that certain characters can be better or worse at. A **skill** is always associated with two **stats**, though it can be associated with the same **stat** twice.

- **Stat**:

- **Test**: A **test** is a d20 roll a player or the GM makes to determine the outcome of an action that a character takes. A **test** is always associated with a particular **skill**. The outcome of a **test** is the result of the d20 roll plus the character's **modifier** in the relevant **skill**.