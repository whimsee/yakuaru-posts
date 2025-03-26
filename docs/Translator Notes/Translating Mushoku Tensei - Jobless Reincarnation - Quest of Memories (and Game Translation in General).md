* * *

Published: 2024-6-21

* * *

![](/images/mushoku-banner.jpg)

This is my unofficial writeup working on [*Mushoku Tensei: Jobless Reincarnation - Quest of Memories*](https://store.steampowered.com/app/2459420/Mushoku_Tensei_Jobless_Reincarnation_Quest_of_Memories/), a licensed dungeon crawler RPG based on an established franchise. While I can't go into the game's production, the localized text is out there now, which I can discuss to an extent having done a bit of everything: story, systems, UI, the restaurant minigame, archive entries, and some original content.

For those interested in the game localization process, I'll do my best to cover challenges related to the medium that aren't unique to this title. But as a licensed game with publisher support, there are differences as well. So let's get into it!

**Philosophy**

The medium of a work affects its presentation and that comes with its unique quirks. Naturally, this applies to its localization as well. Anime subtitles are constrained by time vs number of characters. Manga text work hand-in-hand with the illustration. Light Novels deal with prose and its many incompatibilities in both source and target language. There are overlaps but overall, these are linear experiences with static text.

Games are at the mercy of player agency and dynamic text. You don't really know how a player will approach a situation, let alone what they'll do at a given time. They might get lost or confused, leading to frustration and a bad experience. They might drop the game for a while and return not knowing what's going on anymore because they can't just read/listen/watch back. They could may go down an unintended path and stumble to where they should be. That's why games are guided experiences to some degree.

What does this have to do with localization? When localizing a game, you don't just translate lines and have them make sense or flow naturally within character limits. You're writing a game, which means being mindful of game design principles that communicate to the player what is expected of them and how the game expresses that.

As someone who prioritizes flow, it's tempting to simply smooth out the text when it seems wordy, literal, or repetitive. But good game design effectively carries the player to the end, whether they realize it or not. Dialogue and descriptions say where the player is supposed to go, what they're supposed to do, what to expect, what the enemy's weaknesses are, etc., and it's done consistently to prime them in receiving the information with as little ambiguity as possible. Sure, it's okay to get creative and be playful with the text, but there's always a consideration if it makes those ideas (if they are present) harder to communicate. That's not to say everything has to be spelled out for the player, but it's worth a thought when a line is meant to explicitly guide them. This probably seems obvious, but it's easy to fall into the trap of making things sound right yet miss the point entirely.

**Handling Text**

Game translation means dealing with the game engine's text rendering quirks. This can be as simple as symbol-to-text substitutions (ie. \[@\] rendered as \[heart\]) to putting explicit line breaks for engines that don't support text wrapping or having set text styles, colors, sizes, etc. But the most important detail is the character limit. Since text is usually laid over a background element, which you don't usually get to see beforehand, the goal is simple: Make sure it fits. And if it doesn't, make it fit.

Depending on the segment, this project had three hard limits—characters per line, characters per cell/field, and lines per cell/field. Text wrapping wasn't supported so script tags were used for line breaks, allowing for some discretion. Usually, it was safest to simply match the visual structure of the JP lines. But exceptions were unavoidable, if not preferred, for readability or to simply make it fit.

The line limits between EN and JP were the same. The EN, however, had 25% (50% in rare sections) more characters to work with, a tight limit considering the JP usually hovered around 35 characters per line, but enough in most cases and easier when multiple lines are involved. Still, there were a few unavoidable compromises, which were easy to spot when the JP text's length was close to its respective character limit, when the text used established terms, or (painfully) both.

**When Character Limits Aren't the Only Limit**

Generally, you have options when you expect a line to run over. You can simplify the construction—trim words, use pronouns and fewer spaces, avoid passives (even if it technically accurate, they're usually longer), etc. You can also merge word meanings (ie. "morose" for "sullen and brooding", "bravado" for "brave but scared", etc.) if character voice allows. For multiple lines, there's the concept of compensation in place, where the text segment and its effect is shifted from one place to another to fit or to improve readability. They're all compromises, but a better outcome than omitting the word and/or its meaning entirely.

Established terms add a wrinkle to that. These can be genre legacy terms like Dungeon, Extermination, or stats like Strength and Dexterity. Or specific terms provided by the publisher that must be used as is. Of course, consistency matters; a name like "Rudeus" shouldn't have different spellings and the terms should be relatable to players familiar with the genre or source material. It also sets an authoritative spelling between plausible reads like "Wenport"/"Wind port"/"Windport". However, because it usually takes precedence over character limits, this caused a few issues.

For example, Kishirika Kishirisu's title is "*The Great Empress of the Demon Realm*." That's 36 characters. In JP, it's *魔界大帝*. 4 characters (8 for full-width). Lines usually have a limit of 40-60 characters. So... yup, her title alone can take up at least half the line in EN. There are more instances of that. Events such as "The Fittoa Mass Teleportation Incident" must be rendered in full. Places such as "The Demon Continent" (魔大陸) and spell incantations can run long. There's never a good handling for these. Unless there's space for characters on the next line, it must be trimmed (if allowed) or expressed with shorter words, or with some meanings omitted entirely.

Voiced lines, which this game features, can be limiting in certain respects. This is definitely down to preference and philosophy, but I tend to approach voiced lines differently from unvoiced. Voices add a layer of context and a sort of dissonance can occur when you read a line that doesn't quite match the cadence and tone of the voice, even when done in a foreign language. I wasn't able to hear the lines while working on them, but I knew they were voiced so I erred on the side of matching the line's natural pace if read aloud.

**References and coining terms**

Since the game is from an established franchise and publisher-supported, we were provided a glossary of terms and subtitles from the anime to use as references, and they were willing to help cross-reference the light novel when asked. This was valuable for consistency because it was actually more important to know which terms weren't translated, which was quite a lot.

But it's not as if we could simply coin terms. It still had to be double-checked and approved by the publisher, especially if it's lore-related. One notable veto was 魔石. In context, this referred to the radiant stones that illuminated Rikarisu City. Suffice to say, I had a more specific term in mind to add flavor to the concept (that was also shorter), but we ended up settling with "Magic stone."

There's more leeway for game-specific names and terms. I did the Sortia-related ones, the monster names, quest names, and recipes in the minigame, which were kept save for one monster that had already been established in the light novel. This was fun. Monster names were straightforward and often followed a theme depending on their family or subtype that allowed room for creativity. Whipping up recipe names and descriptions was a blast because they were weird but meant to attract potential customers; some were just asking for a pun, which I gladly delivered. Both the monster and recipe names benefitted from having descriptions; they can 'inherit' the meaning of a name, saving some space to fit more characters in.

The subtitles were a welcome revelation. More than a couple of lines were heavily inspired or lifted straight from the anime or the light novel and they fit contextually so there really was no reason to rewrite them. This actually inspired [SubArchivist](https://subs.yakuaru.com), an anime subtitle archive that I host and maintain.

But when I lacked options and time, I tapped into JP and EN fan wikis, even forums and video explainers. It's good practice to take unofficial info with a grain of salt, but wikis have a knack of archiving the most random bits of info so they're always worth checking. They definitely helped especially for the demon tribes that were usually mentioned in passing without much context or reference.

Finally, pop culture references. Rudeus loves sprinking them in. Handling these can be challenging. For one, you're hoping for a reference that carries over well in EN. One may argue that a pop culture reference must be kept as is for posterity (and that is perfectly valid especially for very specific references), but if the effect of the line is to be cheeky and relatable, then a dated or obscure reference won't do. Second, it breaks banter. Imagine temporarily alienating yourself by dropping a reference that no one will ever get, even if you explain it. This happens often with Rudeus and it wasn't easy making the subsequent confused response sound stilted or repetitive.

**Game-isms**

Generic placeholders are dynamic text objects that, at the time of rendering, are replaced by some value based on the game state or variable. For example, "\<time\> A.M.", where "\<time\>" is the placeholder and "A.M." is static text. This means it could be displayed as "3 A.M." or "10 A.M.", etc. It's a simple concept but this can clash with plurals, among other grammar concepts.

This game features several items and enemies and since Japanese can be rather vague with its plurals, there's always a nagging unease that it might show up in some dialogue box that says "You fought \<val\> cockroach". "1 cockroach" is fine. "2 cockroach" sounds off but good enough. This usually isn't much of an issue (or we just got used to it), but it does make you think twice when it involves mass nouns like sand, wood, or lumber, which are often used as crafting materials. Ideally, you use a quantifier for uncountable nouns like "some" or "a bit of" but the placeholder expects a number. You may also attach another noun that can be counted like "(bundles of) wood", but that assumes they come in bundles (especially if there's a visual) or it may not even fit character-wise.

So when encountering lines with placeholders, it's worth considering the possible values it will hold and minimize these weird phrasings when possible. Honestly though, it does lend a certain charm because this clunkiness is an RPG staple. But if you see instances of that, yeah, chalk it up to JP-EN incompatibilities on top of other constraints. There's always the option to ask for clarification, but only if time allows.

Gender pronouns tend to get flattened when a line expects characters of different genders. For example, the party's exploring a dungeon and one of the members steps on a trap, a line might pop up and say "\<charname\> stepped on a spike trap. They received \<val\> damage." Or descriptions like "Infuses your weapon with the power of light." "They" and "your" here account for the unknown gender. It makes sense in action, but when you're focused on a spreadsheet, you can lose sight of the wider context and just autopilot on a pronoun as it's usually expected in EN but doesn't appear in the JP. Neutral options like "they" and "you" are safe, but sometimes the best option is to omit the pronoun entirely as it takes up characters as well.

Some game dialogue is, by nature, instructive in nature. When a player accepts a quest, the quest giver's expectations are usually explicit. They may not be as specific (ie. they may not indicate how many pieces of lumber they need), but it gives the player a lead on what MacGuffin to deliver or what monster to exterminate by the end of the dialogue. Sometimes this happens with foreshadowing dialogue as well. Once I identify a line like this, which makes up the bulk of dialogue (and most dialogue sequences in the game are short and point toward some action), I prioritize making the line read clear and consistent with its reference. It limits alternative takes, but I'd rather have the player go smoothly through a quest than wonder if they got the right thing.

Menus and UI elements are challenging because you usually have only one of two words to spare. Systems text is more forgiving but the stilted yet descriptive wording usually runs long. Word order suddenly becomes quite important. The minigame was full of these on top of generic placeholders. From menu options to customer barks and status notices, you have to approach them in a utilitarian way, though I was able to add some flair whenever possible.

**The Occupational Hazard of Localization**

Localization involves having to experience the source material ahead of the work's intended audience to get much needed context. Because sometimes that one-off reference that you offhandedly translated might come back and bite you. Or you miss some key foreshadowing detail that ruins the payoff. Sounds cool but you do run the risk of spoiling yourself. Admittedly, this happened to me with Mushoku Tensei. I started the anime for research and came to like the world and characters through the first season of the anime despite its faults, or rather *because* of the flaws it wears on its sleeve. Learning more, however, got me a little too close to the sun, so to speak, and I had to reconcile my disappointment with it.

Don't get me wrong. I appreciate Mushoku Tensei and I'm aware it's contentious for its themes, but that's not where my misgivings are. It's in the execution of those themes and the wasted potential by focusing too much on Rudeus. But that has its own appeal too, which it does well enough. So, just not for me as I think it could be better and let's leave it that.

Did that affect my work? Not really. I can't speak for anyone who's been in this position, but it's better to be informed than uninformed. The rest is up to your work ethic. I believe that translation is writing, and writing is meant to enhance the experience of the reader. I wanted to do that better here and besides, I enjoy the process itself so it wouldn't do to let my opinions get in the way of that.

**Debriefing**

![](/images/mushoku-example.jpg)
[Looked nicer on the spreadsheet but could've done "take on a few requests" instead.]

After seeing the game in action, I honestly think there are bits here and there I could've done better. Some dialogue could've been trimmed or handled more gracefully because the approach was stiffer than I thought it would be, especially now that I see how the pieces fit. Game development being what it is, everything's in flux so you don't always have enough context and not enough time to ask for one since visual references might not exist in the first place.

Still, I'm quite proud and glad I get to experience this kind of thing (and thankful for everyone I got to work with) so I can finally write about my thoughts about it!