# Todo List

This list is not necessarily a guarantee, but it contains a list of features and updates I plan to add. 
Things may be added to this list as I think of them, and removed if they are added or I change my mind.

## Engine updates and New Features
* Cleanup pokered-gbc code (optimizations)
* Add support for larger tileset images, like Polished Crystal
* Add support for setting XY Flip/Palette Attributes as part of block data?
* Real-Time Clock, with Day and Night
* More modern Berry System, allowing you to plant and grow new ones instead of the Gen 2-like current system
* Expand Pokédex beyond 255 (mimic ShantyTown's "expand-dex" branch)
* Allow for more than one proper region, so Johto can happen
* Individual menu sprites for all Pokémon
* Pokégear/Pokénav equivalent
* Rematches with Trainers and Gym Leaders, no annoying phone calls
* Bag has multiple pockets and more storage space
* Held items
* Special split into two stats
* New available move pool, with a lot more thought put into it this time
* Weather effects in-battle
* Abilities (can enable or disable during intro)
* Natures (can enable or disable during intro)
* Infinite-Use TMs
* New Pokéball types
* Dive areas
* Battle Tower
* Battle Factory
* Battle Tent
* Pokémon World Tournement
* Player customization options
* Rewritten Trainer AI
* Secret Bases
* Surfing Pikachu minigame (ported from Pokeyellow)
* Ruins of Alph puzzles (waiting for PR from ShantyTown)
* Bug Catching Contest
* Possibly add Forms
* Use IVs and EVs instead of DVs and Stat EXP, old DVs become a mini Personality ID
* Gain EXP on catching a Pokémon


## Bugfixes from Vanilla RB
* Leech Seed/Toxic shared damage counter
* Toxic becomes normal poison if you swap
* OHKO moves based on speed
* Crits ignore stat-ups from both Pokémon
* Agility negates speed-loss before boosting
* Using Counter on moves used against your Substitute
* Using Counter against OHKO moves to instakill
* Trapping moves prevent opponent doing anything
* Whirlwind and Roar do not work in trainer battles
* Rest does not undo stat changes from status afflictions you had, such as Burn
* Rage issues
* Mimic and Disable choosing moves at random
* Multi-hit moves deal same damage for each blow
* Make Pokéball break with zero shakes instead of "You missed the Pokémon!"
* Stat-up too high making your stat roll over to ultra low values
* Substitute not protecting against status
* Remove badge boosts, to be more modern


## Unsorted Notes
* Pokégear/Pokénav would replace Town Map, have a VS Seeker option, a radio, etc.
* Several things in WRAM could stand to be optimized, such as event flags and map script bytes
* Hide/Show routine needs work. Probably better to redo it based on normal flags somehow, like Gen 2
* IndexToPokedex and PokedexToIndex are pointless now, and can be removed
* Remove the weird TM Name Generation routine, TM Case will work differently.
* Add even more trainer classes and cameo trainers
* Johto needs songs from Crystal, of course
* Johto should include areas that were in Polished Crystal/Christmas
* Battle Tower will be in Johto
* Pokémon World Tournement will be where Pokéathalon was in HGSS
* Battle Tent will be in Celadon
* Battle Factory will be in Johto with the Battle Tower
* Instead of CheckForHex and CheckForElectroBall, there should be one routine to calculate variable BP moves
* Once Held Items are a thing, Acrobatics needs to be variable BP, too
* Any checks for hard-coded map IDs need to also check wCurRegion when the time comes
* New trainer AI will be more modular, and AI_BASIC will be at least be generically intelligent
* Pull Swimmer F data out of Beauty class list
* Consolidate Leader classes and Elite Four classes
* Maybe change Trainer DVs back to checking AI Number, instead of Trainer Class, once those are consolidated
* If Natures are disabled in intro, do not display on status screens, and use a neutral nature always
* If Abilities are disabled in intro, do not display on status screens, and use a blank ability for everyone
* EXP on catch is annoying, since a lot of variables are reused during the EXP Gain process. Will require a lot of testing.
