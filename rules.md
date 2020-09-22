Version 0.3.0

This file is designed to outline the rules of the game, without the styling that might appear in a more polished document.

ONLY HUMAN is inspired by the [Dead Simple RPG](https://deadsimplerpg.wordpress.com/about/) games, particularly [Blaster](https://deadsimplerpg.wordpress.com/category/blaster-sf-rpg/).

# Basic Rules

ONLY HUMAN is a simple tabletop role playing game framework, for when you don't need a built in setting, an entire magic / technology system, and godlike progression. It requires a game master (GM) to control the world / non-player characters (NPCs) and to adjudicate the outcomes of player actions, and at least one player to control the player character(s) (PCs).

This section contains the basic rules for playing the game, as they pertain to the players. The GM will also likely use some of these rules, but their interactions are outlined further in the [GM Guide](#GM-Guide).

An actual implementation of this framework requires the details of armour, weapons, items, and roles. The [Still Human](#Still-Human) section of these rules provide an example of that.

Before playing each player and the GM should have access to at least one d20 (d20s are 20 sided dice), as well as some paper, pencils and erasers to record character details and notes. The GM should have an interesting story or scenario for the player(s) to encounter, and outlines of any special mechanics that they expect to use during the game.

## Character Creation

Before playing the game, the players each create a character. When doing so, players must allocate `12` points between the four **stats** that characters have: Dexterity (`DEX`), Intelligence (`INT`), Strength(`STR`), and Will (`WIL`). Each stat may be allocated at most `6` points.

Players must additionally allocate `16` points between **skills**. The GM may also provide you with the option to pick a **role**, which will confer an additional `4` points that must be allocated within particular set of **skills**. No skill can be allocated more than `4` points.

Each **skill** is associated with two **stats**. The list below details some examples of **skills**, but it is not exhaustive: you can add any number of other **skills** to the game pending only the agreement of the GM, and the association of the **skill** with a pair of **stats**.

- `DEX` + `DEX`: *Agility*, *Slight of hand*
- `DEX` + `INT`: *Ranged attacking*
- `DEX` + `STR`: *Speed*
- `DEX` + `WIL`: *Stealth*
- `INT` + `INT`: *Technology*, *Medicine*
- `INT` + `STR`: *Melee attacking*
- `INT` + `WIL`: *Investigation*, *Insight*
- `STR` + `STR`: *Athletics*
- `STR` + `WIL`: *Toughness*, *Intimidation*
- `WIL` + `WIL`: *Persuasion*

The points allocated to **stats** and **skills** are used to create modifiers that are explained in the [Tests](#Tests) section of these rules.

Keep in mind that these numbers should not completely describe your character. Think about their personality, what they want, what they need (but might not know they need), and how they know the other characters in the group. Have secrets for your character, but want them to be discovered.

## Tests

When a character tries something that has a risk of failure, and a chance of success, the GM must adjudicate the outcome. A common way to do so is to have the character take a **test**. A **test** must always be associated with a **skill**, which in turn must always be associated with two **stats**. The controlling player of the character in question, or the GM for NPCs, rolls a d20 and adds the character's **modifier** in the **skill**.

To find a character's **skill** **modifier** add together their points in the associated **stats** and then divide this by `2` rounding the result down (this is just the value of the **stat** if the **skill** is associated with the same **stat** twice), and then add their points in the associated **skill** to this value. When these rules reference a **skill** in a numerical context, they are referring to this **modifier**.

For every **test** taken the GM should choose a **difficulty** that corresponds to the challenge of the task at hand, with a higher **difficulty** indicating a harder to complete task. The [GM Guide](#GM-Guide) provides advice on [setting difficulties](#Setting-Difficulties).

If the result of the **test** is at least as high as the **difficulty** then the **test** is a success, otherwise it is a failure.

## Contests

**Contests** are a special kind of **test** for when two or more characters are simultaneously attempting tasks that come into conflict. In a **contest** the conflicting characters each take a **test** in the **skill** relevant to the task they are attempting. The character(s) with the highest result succeeds, and all the other characters (perhaps to varying degrees) fail. The GM adjudicates the outcome of any ties.

## Turns

When things get tense characters start taking turns. The turn order, and whether or not they overlap, is up to the GM. Everyone taking a turn represents about `10` seconds of time.

During a turn, characters may move, and once per turn (possibly during that movement) they may take an ​**action**. An **action** may take the form of **attacking**, **running**, **readying**, interacting substantially with an object, attempting to **stabilise** a character, or doing anything else that GM deems worthy of requiring an action.

Characters may talk at any point during turns, but the GM should ensure that they don’t communicate more than is reasonable in the amount of time that has elapsed.

## Moving

When characters make a move, they can move in a path of up to `10 + (2 × Speed)` metres in length. If a character is climbing, swimming, trying to move stealthily, wearing or carrying something bulky, or moving over difficult terrain, then they are considered to be **restricted**. The distance a character moves whilst **restricted** counts twice against their movement.

## Attacking

A character may spend their **action** making an attack, providing they know where they are attacking (if there is no target there the attack fails), the target of their attack is within range of the weapon they are using, and there is nothing physically preventing the attack (such as a wall). To make an attack characters make the relevant of either a _​Ranged attacking​_ or a _​Melee attacking​​_ **test**, adding their weapon modifier to their result. The **difficulty** for this **test** is `10 + target DEX`. Increase the **difficulty** by `2` for ranged attacks on targets within `2 metres`, and by `4` if the attacker can see less than half of the target.

If the attacker fails this **test** nothing further happens and the **action** is complete. Otherwise, the attack has an **impact** of the amount they exceeded their attack **test** by (possibly zero), minus the **absorption** of any armour the target is wearing. The target must then take a _Toughness_ **test**, with a **difficulty** of `15 + impact`. If the target fails this **test** they get **injured** and become **unstable**. If they fail by a margin of `10` or more they get **injured** twice, and if they fail by `15` or more they get **injured** three times.

## Running

If a character uses their action to **run** they may double the distance they are permitted to move in the current turn.

## Readying

If a character uses their action to **ready** they must specify a condition and an **action** that their character could make - in sufficient detail to satisfy the GM. If the specified condition occurs before they next take a turn, their character immediately takes the specified action.

## Injury

Characters have a **health state**, and are either **stable** or **unstable**. To begin with most characters are assumed to be **stable** in a normal **health state**.

If a character gets **injured** they drop to the next health state down the table. If they have been **unstable** in the same health state for more than half an hour, their player (or the GM for NPCs) rolls an unmodified d20. If the roll is an `11` or higher the character becomes **stable**, otherwise get **injured**

A successful _Medicine_ test of **difficulty** `11` will **stabilise** a character, but true recovery can require days, or perhaps specialised equipment (at the discretion of the GM).

| Health State | Effect |
| ------------ | ------ |
| Normal | The character is feeling fine. |
| Wounded | The character is hurt, they suffer a `-2` penalty to all **tests** |
| Seriously Wounded | The character is really hurt, they suffer a `-4` penalty to **tests** and are **restricted**. |
| Incapacitated | The character is unconscious (or effectively unconscious), they cannot voluntarily do anything and can easily be captured or killed. You no longer add this character's `DEX` to the **difficulty** of the **test** to attack them. |
| Dead | The character is dead, Jim. |

# Still Human

Still Human is a sci-fi implementation of the ONLY HUMAN framework, that is, it provides statistics for armour, weapons, other items, **roles**, and (through these) the vaguest hint of a setting for the GM to build upon.

Still Human is designed to run games for teams of highly trained or experienced characters that are sent on, or somehow end up entangled in, various missions in reasonably hard sci-fi near-ish future settings.

This should not be the only implementation, style, or setting that ONLY HUMAN is able to be played in. Hopefully this section serves to also provide an example of how this game can actually be implemented into something generally playable.

## Equipment

| Armour | Absorption | Description / Effects |
|:------ | ----------:|:--------------------- |
| Normal Clothes | `0` | Stylish _and_ practical |
| Space Suit | `2` | A surprisingly compact vacuum rated environmental suit. Two hot-swappable tanks (that passively re-fill in atmosphere) provide one hour of oxygen each. If the suit absorbs any damage it is torn, and must be repaired before it will be vacuum worthy. A character wearing a space suit is **restricted**. |
| Reinforced Space Suit | `3` | A military grade space suit. The same as a space suit, except it is only torn if its wearer is hit with an attack that results in an **impact** greater than `0`. |
| Combat Armour | `3` | Tactical body armour. |
| Combat Carapace | `4` | Heavy duty body armour. A character wearing combat carapace is **restricted**. |

| Weapon | Type | Range | Modifier |
|:------ |:---- | -----:| --------:|
| Combat Knife | Melee | `2 metres` | `+1` |
| Improvised Weapon | Melee | `2 metres` | `-1` |
| Shock Rod | Melee | `2 metres` | `+2` |
| Assault Rifle | Ranged | `400 metres` | `+3` |
| Auto Pistol | Ranged | `50 metres` | `+1` |
| Combat Knife | Ranged | `10 metres` | `+0` |
| Improvised Weapon | Ranged | `10 metres` | `-4` |

| Other Items | Description / Effects |
|:----------- |:--------------------- |
| Short Range Communicator | A small radio device. Provides encrypted communication with selected short range communicators configured to allow it within `20km`. |
| Long Range Communicator | A backpack sized radio device that provides encrypted communication to selected equipment configured to receive it within `40,000km`. |
| Pad | A smartphone sized, portable, touch screen computer. |
| Navigator | A small attachment to a pad that uses known maps, available satellite data, and computer vision to attempt to inform the user of their position at all times. |
| Scanner | A small attachment to a pad that allows various kinds of scanning. Where relevant, a scanner gives a `+2` modifier to _Investigation_ **tests**. |
| Medical Kit | A brief-case sized box containing various medical supplies. Where relevant, a medical kit gives a `+2` modifier to _Medicine_ **tests**. Additionally, the medical kit contains `5` stim-shots, that can be used to rouse an unconscious character to the seriously wounded **health state**, and a defibrillator that can be used to revive a dead character to the seriously wounded **health state** if they died in the last minute from causes that can be resolved by restarting their heart. The defibrillator has `5` uses per charge. Use of both the stim-shots and the defibrillator require a successful **stabilisation** **action**, if the **test** is failed they are still used, but have no effect. |
| Engineering Kit | A vacuum rated toolbox full of various equipment for dealing with the tech a space-faring engineer might expect to encounter. Where relevant, an engineering kit gives a `+2` modifier to _Technology_ **tests**. Additionally, the engineering kit contains `5` patches that can, as an **action**, be used to repair tears in space suits. |

## Roles

Still Human adds one additional **skill** to the game: _Piloting_, a `DEX` + `INT` **skill**. In addition to the benefits of **roles** outlined in the character creation section, with the agreement of the GM a character that selects one of the following roles may also take the corresponding piece(s) of equipment, and all characters may take Normal Clothes, a Space Suit, a Short Range Communicator, Pad, and their choice of a combat knife or an Auto Pistol.

| Role | Skills | Equipment |
|:---- |:------ |:--------- |
| Pilot | _Piloting_, _Investigation_ | Navigator |
| Communications | _Technology_, _Insight_, _Persuasion_ | Long Range Communicator |
| Security | _Ranged attacking_, _Melee attacking_, _Toughness_ | Reinforced Space Suit, Assault Rifle, Shock Rod |
| Engineering | _Slight of hand_, _Piloting_, _Technology_ | Engineering Kit |
| Medical | _Slight of hand_, _Medicine_ | Medical Kit |
| Science | _Technology_, _Investigation_ | Scanner |

## Requirements and Requisitioning

An alternative to roles is to come up with a list of required proficiencies for the group, e.g. "We need people experienced in piloting and investigation, and someone trained in both technology and slight of hand", and let the group work out how they will fill those niches together. Similarly, a pool of equipment can be provided, for the group to share out. This could lead to relations forming between the characters whilst they are being created.

# GM Guide

ONLY HUMAN is rather rules light. This is quite intentional, and is based on the idea that the fundamental core of an RPG is incredibly simple, and can benefit from being more exposed for GMs to tinker with. However, this power does also come with responsibility. Hence, this sections exists to provide various tips to try to help GMs out.

## Setting Difficulties

When setting **difficulties** generally keep in mind these difficulty levels:

| Difficulty             | **difficulty** |
|:---------------------- | --------------:|
| Very Easy              |              5 |
| Easy                   |             10 |
| Moderately Complicated |             15 |
| Difficult              |             20 |
| Very Difficult         |             25 |
| Practically Impossible |             30 |

Unless you are intentionally trying to hide the difficulty of the task, if a player attempts a task that is impossible to fail, or impossible to successfully complete, there is no need for a **test**. Simply narrate the outcome to the players.

## Adjudicating Complex Tasks

ONLY HUMAN does not provide specific rules for adjudicating everything a player may wish to try. So, when dealing with non-standard tasks, attempt to find a way to distil them down into one or more core difficulties (parts of the task with a risk of failure and a chance of success) that can be related to **skills** (whether on the given **skills** table or not).

Once you know what **skills** are involved, try to gauge the difficulty of these components of the task, work out if they happen in an order or at the same time, and work out what success or failure for individual parts or combinations of individual parts looks like. Finally, with these ideas in mind, have the character take **tests** based on the established skills and difficulties, in the established order, and provide the established outcomes.

In practice, this does not need to be dealt with remotely as formally, but that structure forms guidelines for one way to react to players attempting complicated tasks.

## Turns

ONLY HUMAN does not prescribe a method for determining the order of turns, whether there even is an order to turns, and whether or not turns can overlap. This should generally be decided on a case by cases basis, as there is no one system that is good for every situation. The order could be determined by _Speed_ **contests**, it could just evolve from the scene, characters could be divided into teams that alternate, or perhaps everyone could go at once. The characters can be sequenced through any method you like.

## Adding to the Game

Feel free to add items or rules to the game, it is intentionally kept simple for that reason - it requires story / setting based additions to come into its own. Keep in mind that it is expected for specific rules to override general rules, so don't be afraid of that. Perhaps you want a gun that fires so fast its wielder effectively shoots twice in one action, or an enemy that can take a lot more hits than a usual character. Don't worry if these things go against the core rules, GMing would be much less fun if the players knew how everything worked.

Adding equipment and roles (to effectively create your own implementation of ONLY HUMAN) is another great way to extend the game. Consider adding items or features that vary in more ways than the basic rules allow, such as a shotgun that can git everything in a cone up to `10 metres` with a `+4` or one target out to `30 metres` with a `+1`.

Additionally, when creating antagonists or enemies do not feel you need to stick to the options available to the player. You may want grunt alien enemies that drop dead on a single \textit{Toughness} \textbf{test} failure, or a villain antagonist so drugged up on stimulants that they are much harder to take down. You may want characters that have better or worse stats than the standard player character creation allows. Go for it.

## Character Equipment

Whilst there is no strict limit on how much equipment a character can carry, it is best to be realistic. If you think a PC is carrying too much, perhaps ask the player to label where everything is on their character's body. You could also apply strict carry weight limits, such as `40 + 10 × Athletics` kilograms of equipment. If you wanted to be even more granular you could specify that a character carrying more than `40 + 5 × Athletics` is **restricted**.

## Progression

It is possible to implement a rudimentary progression system in ONLY HUMAN. The simplest way would be to give players more points to allocate to **stats** and **skills**, and perhaps raising the cap on the maximum allocatable to each. If you plan on doing this, consider starting the characters initially with fewer points than the [character creation](#Character-Creation) section suggests, as increasing the available points too far beyond this point could leave min-maxed characters with very large **modifiers**.

Another simple progression mechanism, that is perhaps more inline with the ethos of ONLY HUMAN, would be to provide players with better equipment, and better connections in the setting of the game.
