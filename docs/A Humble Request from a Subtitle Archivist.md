---

Published: 2023-11-12

---
![](/images/subs.png)

Creating these files needs to follow a standard. Or at least it needs better standards. Let's get into why.

On March 2022, several anime shows left the streaming service Crunchyroll ([https://www.siliconera.com/shows-leaving-crunchyroll-in-march-2022-include-danmachi-no-game-no-life/](https://www.siliconera.com/shows-leaving-crunchyroll-in-march-2022-include-danmachi-no-game-no-life/)). While that doesn't necessarily mean you won't be able to watch those shows anymore, there is an integral part of it that's often lost and taken for granted whenever this happens: the subtitles.

Sure, shows can have any number of official and unofficial subtitles, and one can argue it's layered on top of the content you're watching and you can freely turn it off or watch dubs instead. But consider that a person worked on this, that it can actually enhance the experience of watching the show, even get referenced in wikis or memes or turned into legacy terminologies for future iterations. Regardless of whether or not the subtitles are good, there's value in preserving them, especially because these pieces of text aren't easily text-searchable and exist mostly in screenshots or bound to the files that play alongside them. Doubly so if there's a point of comparison between the quality of subs. Or in some cases, name or term spellings between episodes.

Personally though, clever and creative writing exists in these subs and deserves to be kept as a source of inspiration or learning. And once those shows are off the platform, they're gone unless it's archived in some way. And ironically unofficial are better archived because of piracy.

It's because of that I've decided to build a subtitle archive for official subs. Currently, it's in a testing phase, but you may check it out at [https://subs.yakuaru.com](https://subs.yakuaru.com) and the pages will be editable once it's fully live.

There is one problem though and it's naming the speaker. Here's a typical dialogue line if you read a .ass subtitle file:

Dialogue: 0,0:05:09.81,0:05:11.64,**Default**,**Chise**,0000,0000,0000,,**There are a lot of cats here.**

I won't get into the technical details of parsing these for archiving, but there are three fields that matter, bolded for emphasis:

**Default** \- Style

**Chise** \- The Speaker Name. Let's call this Speaker

**There are a lot of cats here.** - The line shown on screen. Let's call this Line.

The Style is linked to a preset that determines how it looks. It's a good way to tell if it's a spoken line, an internal monologue, a flashback, or a sign. This one's fairly consistent because you see it on screen, ie. _internal monologues are always italicized_.

The Line can be handled differently since they can be modified inline instead of the Style preset but they're generally manageable, ie. "internal monologues are {\\i1}always{\\i0} italicized" will come out as "internal monologues are _always_ italicized" on screen.

The Speaker is where it consistently falls apart, primarily because no one usually sees it aside from whoever handles the subs. This is a perfect example. For reference it's from Crunchyroll's English sub of The Ancient Magus' Bride EP 4 _Everything must have a beginning_.

![](/images/screenshot_20231111_141708c.png)

And this is a snippet of my Speaker substitution list. Left is what's on the subtitle file, right is what shows on the archive:

![](/images/screenshot_20231111_124455c.png)

You have proper names, along with rather descriptive names, wildcards (which may also refer to named characters), emojis, and what seems to be an excerpt from an economics paper. This goes on for the entire 24-episode season and there are several shows like this. It's funny at first, and I get it, but it's terrible from a preservationist's standpoint.

I've decided to fix these on a best-effort basis since the alternatives are to leave them in or to blank out the Speakers, neither of which are preferable (there is an exception). That means essentially rewatching the show to check discrepancies (not the worst deal since I love the show), but that takes so much time compared to a properly named subtitle file. They do exist… as well as shows with the Speakers blanked out or replaced with a wildcard. Those I make a compromise of blanking out entirely since it didn't have names in the first place (or it was likely a conversion from a different subtitle format).

Just to be clear, I'm not telling people how to do their job. It's hard enough as it is sometimes and it's an ask to keep the names right and consistent. However, consider the value of making your works easier to understand and parse. You might never have to look at those files again, but someone else might and they will thank you for it. And my examples are not to shame anyone, but they are the best ones I currently have.

If you want recommendations:

1. Keep the names consistent. If a Speaker goes by X, keep it X for that Speaker alone. Typos can happen but that's easier to catch.

3. Avoid wildcards. I've seen a few where "A" could be anyone. "Ferdinand" can turn into "F", which is kinda okay, until you see a "Fran" that becomes "F" as well in certain cases. (This happened in Ascendance of a Bookworm.)

5. It's fine to have fun with the names, but tone it down a bit as it takes time to add those in. Here's an example from Crunchyroll's English sub of Yuru Camp S1. Credit to them, it was consistent:

![](/images/screenshot-2023-11-11-163924.png)

Finally, if it's really too much trouble though, it's fine. The dialogue is ultimately more important and those are kept as is.

And that's about it. There's a lot of anime to go through. Again the pages can edited once it's live so feel free to help out if the names are off.
