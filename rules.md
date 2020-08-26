# ONLY HUMAN

Version 0.3.0

This file is designed to outline the rules of the game, without the styling that might appear in a more polished document.

ONLY HUMAN is inspired by the [Dead Simple RPG](https://deadsimplerpg.wordpress.com/about/) games.

## Basic Rules

ONLY HUMAN is a simple tabletop role playing game framework, for when you don't need a built in setting, an entire magic / technology system, and godlike progression. It requires a game master (GM) to control the world / non-player characters (NPCs), and at least one player to control the player character(s) (PCs).

This section contains the basic rules for playing the game, as they pertain to the players. The GM will also likely use some of these rules, but their interactions are outlined further in the [GM Guide](#GM-Guide).

An actual implementation of this framework requires the details of armour, weapons, items, and roles. The [Still Human](#Still-Human) section of these rules provide an example of that.

Before playing each player and the GM should have access to at least one d20 (d20s are 20 sided dice), as well as some paper, pencils and erasers to record character details and notes. The GM should have an interesting story or scenario for the player(s) to encounter, and outlines of any mechanics that they expect to use during the game.

### Character Creation

Before playing the game, the players each create a character. When doing so, players must allocate `12` points between the four **stats** that characters have: Dexterity (`DEX`), Intelligence (`INT`), Strength(`STR`), and Spirit (`SPT`). Each stat may be allocated at most `6` points.

Players must additionally allocate `16` points between **skills**. The GM may also provide you with the option to pick a **role**, which will confer an additional `4` points that must be allocated to a particular set of **skills**. No skill can be allocated more than `4` points.

Each **skill** is associated with two **stats**. The list below details some examples of **skills**, but it is not exhaustive: you can add any number of other **skills** to the game pending only the agreement of the GM, and the association of the **skill** with a pair of **stats**.

- `DEX` + `DEX`: *Agility*, *Slight of hand*
- `DEX` + `INT`: *Ranged attacking*
- `DEX` + `STR`: *Speed*
- `DEX` + `SPT`: *Stealth*
- `INT` + `INT`: *Technology*, *Medicine*
- `INT` + `STR`: *Melee attacking*
- `INT` + `SPT`: *Investigation*, *Insight*
- `STR` + `STR`: *Athletics*
- `STR` + `SPT`: *Toughness*, *Intimidation*
- `SPT` + `SPT`: *Persuasion*

The points allocated to **stats** and **skills** are used to create modifiers that are explained in the [Tests](#Tests) section of these rules.

Keep in mind that these numbers should not completely describe your character. Think about their personality, what they want, what they need (but might not know they need), and how they know the other characters in the group. Have secrets for your character, but want them to be discovered.

### Playing the Game

#### Tests

When a character tries something that has a risk of failure, and a chance of success, the GM must adjudicate the outcome. A common way to do so is to have the character take a **test**. A **test** must always be associated with a **skill**, which in turn must always be associated with two **stats**. The controlling player of the character in question, or the GM for NPCs, rolls a d20 and adds the character's **modifier** in the **skill**.

To find a character's **skill** **modifier** take the average of their points in the associated **stats** (which is just the value of the **stat** if the **skill** is associated with the same **stat** twice), rounding down, and then add their points in the associated skill. When these rules reference a **skill** in a numerical context, they are referring to this **modifier**.

For every **test** taken the GM should choose a **difficulty** that corresponds to the challenge of the task at hand, with a higher **difficulty** indicating a harder to complete task. The [GM Guide](#GM-Guide) provides advice on [setting difficulties](#Setting-Difficulties).

If the result of the **test** is at least as high as the **difficulty** then the **test** is a success, otherwise it is a failure.

#### Contests

**Contests** are a special kind of **test** for when two or more characters are simultaneously attempting tasks that come into conflict. In a **contest** the conflicting characters each take a **test** in the **skill** relevant to the task they are attempting. The character(s) with the highest result succeeds, and all the other characters (perhaps to varying degrees) fail. The GM adjudicates the outcome of any ties.

#### Turns

When things get tense characters start taking turns. The turn order, and whether or not they overlap, is up to the GM. Everyone taking a turn represents about `10` seconds of time.

During a turn, characters may move, and once per turn (possibly during that movement) they may take an ​**action**. An **action** may take the form of **attacking**, **running**, **readying**, interacting substantially with an object, attempting to **stabilise** a character, or doing anything else that GM deems worthy of requiring an action.

Characters may talk at any point during turns, but the GM should to ensure that they don’t communicate more than is reasonable in the amount of time that has elapsed.

#### Moving

When characters make a move, they can move in a path of up to `10 + (2 × Speed)` metres in length. If a character is climbing, swimming, trying to move stealthily, wearing or carrying something bulky, or moving over difficult terrain, then they are considered to be **restricted**. The distance a character moves whilst **restricted** counts twice against their movement.

#### Attacking

A character may spend their **action** making an attack, providing the target of their attack is within range of the weapon they are using, and there is nothing physically preventing the attack (such as a wall). If a character cannot see their target, they must declare where they are attacking, if there is nothing there their attack fails, but otherwise it continues as normal. To make an attack characters make the relevant of either a _​Ranged attacking​_ or a _​Melee attacking​​_ **test**, adding their weapon modifier to their result. The **difficulty** for this **test** is `10 + target DEX + cover`, where `cover` is `3` if half or more of the target is obscured from the attacker and `6` if more than three quarters of the target is obscured from the attacker.

If the attacker fails this **test** nothing further happens and the **action** is complete. Otherwise, the attack has an **impact** of the amount they exceeded their attack **test** by (possibly zero), minus the **absorption** of any armour the target is wearing. The target must then take a _Toughness_ **test**, with a **difficulty** of `15 + impact`. If the target fails this **test** they are **injured** and become **unstable**. If they fail by a margin of `10` or more they are **injured** twice, and if they fail by `15` or more they are injured three times.

#### Running

If a character uses their action to **run** they may double their movement for the turn.

#### Readying

If a character uses their action to **ready** they must specify a condition and an **action** that their character could make - in sufficient detail to satisfy the GM. If the specified condition occurs before they next take a turn, their character immediately takes the specified action.

#### Injury

Characters have a **health state**, and are either **stable** or **unstable**. If a character is **injured** or they have been **unstable** in the same health state for more than half an hour, they drop to the next health state down the table. To begin with most characters are assumed to be **stable** in a normal **health state**. A successful _Medicine_ test of **difficulty** `15` will **stabilise** a character, but true recovery can require days, or perhaps specialised equipment (at the discretion of the GM).

| Health State | Effect |
| ------------ | ------ |
| Normal | The character is feeling fine. |
| Wounded | The character is hurt, they suffer a `-2` penalty to all **tests** |
| Seriously Wounded | The character is really hurt, they suffer a `-4` penalty to **tests** and are always considered **restricted**. |
| Incapacitated | The character is unconscious (or effectively unconscious), they cannot voluntarily do anything and can easily be captured or killed. You no longer add this character's `DEX` to the **difficulty** of the **test** to attack them. |
| Dead | The character is dead, Jim. |

## Still Human

Still Human is a sci-fi implementation of the ONLY HUMAN framework, that is, it provides statistics for armour, weapons, other items, **roles**, and (through these) the vaguest hint of setting for the GM to build upon.

Still Human is designed to run games for teams of highly trained or experienced characters that are sent on, or somehow end up entangled in, various missions in reasonably hard sci-fi near-ish future settings.

This should not be the only implementation, style, or setting that ONLY HUMAN is able to be played in. Hopefully this section serves to also provide an example of how this game can actually be implemented into something generally playable, in any context.

### Equipment

| Armour | Absorption | Description / Effects |
|:------ | ----------:|:--------------------- |
| Normal Clothes | 0 | Stylish _and_ practical |
| Space Suit | 2 | A surprisingly compact vacuum rated environmental suit. Two hot-swappable tanks (that passively re-fill in atmosphere) together one hour of oxygen each. If the suit absorbs any damage it is torn, and must be repaired before it will be vacuum worthy. A character wearing a space suit is **restricted**. |
| Reinforced Space Suit | 3 | A military grade space suit. The same as a space suit, except it is only torn if its wearer is hit with an attack and it cannot absorb all the **impact**. |
| Combat Armour | 3 | Tactical body armour. |
| Combat Carapace | 4 | Heavy duty body armour. A character wearing combat carapace is **restricted**. |

| Weapon | Type | Range | Modifier |
|:------ |:---- | -----:| --------:|
| Combat Knife | Melee | 2m | +1 |
| Improvised Weapon | Melee | 2m | -1 |
| Shock Rod | Melee | 2m | +2 |
| Assault Rifle | Ranged | 400m | +3 |
| Auto Pistol | Ranged | 50m | +1 |
| Combat Knife | Ranged | 10m | +0 |
| Improvised Weapon | Ranged | 10m | -4 |

| Other Items | Description / Effects |
|:----------- |:--------------------- |
| Short Range Communicator | A small radio device. Provides encrypted communication with selected short range communicators configured to allow it within 20km. |
| Long Range Communicator | A backpack sized radio device that provides encrypted communication to any equipment configured to receive it within 40,000km. |
| Pad | A smartphone sized, portable, touch screen computer. |
| Navigator | A small attachment to a pad that uses known maps, available satellite data, and computer vision to attempt to inform the user of their position at all times. |
| Scanner | A small attachment to a pad that allows various kinds of scanning. Where relevant, a scanner gives a `+2` modifier to _Investigation_ **tests**. |
| Medical Kit | A brief-case sized box containing various medical supplies. Where relevant, a medical kit gives a `+2` modifier to _Medicine_ **tests**. Additionally, the medical kit contains 5 stim-shots, that can be used to rouse an unconscious character to the seriously wounded **health state**, and a defibrillator that can be used to revive a dead character to the seriously wounded **health state** if they died in the last minute from causes that can be resolved by restarting their heart. |
| Engineering Kit | A vacuum rated toolbox full of various equipment for dealing with the tech a space-faring engineer might expect to encounter. Where relevant, an engineering kit gives a `+2` modifier to _Technology_ **tests**. Additionally, the engineering kit contains 5 patches that can be used to repair tears in space suits. |

### Roles

Still Human adds one additional **skill** to the game: _Piloting_, a `DEX` + `INT` **skill**. In addition to the benefits of **roles** outlined in the character creation section, with the agreement of the GM a character that selects one of the following roles may also take the corresponding piece(s) of equipment, and all characters may take Normal Clothes, a Space Suit, a Short Range Communicator, and a Pad.

| Role | Skills | Equipment |
|:---- |:------ |:--------- |
| Pilot | _Piloting_, _Investigation_ | Navigator |
| Communications | _Technology_, _Insight_, _Persuasion_ | Long Range Communicator |
| Security | _Ranged attacking_, _Melee attacking_, _Toughness_ | Reinforced Space Suit, Assault Rifle, Shock Rod |
| Engineering | _Slight of hand_, _Piloting_, _Technology_ | Engineering Kit |
| Medical | _Slight of hand_, _Medicine_ | Medical Kit |
| Science | _Technology_, _Investigation_ | Scanner |

## GM Guide

### Setting Difficulties

When setting **difficulties** generally keep in mind these difficulty levels:

| Difficulty             | **difficulty** |
|:---------------------- | --------------:|
| Very Easy              |              5 |
| Easy                   |             10 |
| Moderately Complicated |             15 |
| Difficult              |             20 |
| Very Difficult         |             25 |
| Practically Impossible |             30 |

### Adjudicating Complex Tasks

### Adding to the Game

## Definitions

Some words or phrases in the above rules are written in bold. This means that they have a particular definition within the game that is more specific than their general English definition. Whilst they are explained the first time they appear, their meaning is detailed again here for ease of reference.

- **Stat**: Definition
- **Skill**: Definition
- **Role**: Definition
- **Modifier**: Definition
- **Difficulty**: Definition
- **Test**: Definition
- **Restricted**: Definition
- **Action**: Definition
- **Attacking**: Definition
- **Running**: Definition
- **Readying**: Definition
- **Impact**: Definition
- **Absorption**: Definition
- **Injured**: Definition
- **Health State**: Definition
- **Unstable**: Definition
- **Stable**: Definition
