---
description: Copied from dbd.js docs
---

# Compact functions

**Compact functions are really easy to use, they are the replacements for some functions. This functions returns values.**

## $msg\[chid;mid;property\] or $msg\[property\]

**Properties**

* author - Message's Author's ID
* authormention - Message's Author's mention
* authortag - Message's Author's tag
* authorname - Message's Author's name
* channel - Message's channel id location
* channelname - Message's channel name location
* cleancontent - Message's content without any mentions \(excludes `@here` / `@everyone\`\)
* content - Message's content
* created - Message's date and time of creation
* guildid - Message's guild's id of origin
* id - Message's ID
* isdeleteable - Whether or not the author of the command can delete the message, returns a Boolean.
* isdeleted - Whether or not the message was deleted, returns a Boolean.
* iseditable - Whether or not the author of the command can edit the message, returns a Boolean.
* ispinnable - Whether or not the author of the command can pin the message, returns a Boolean.
* ispinned - Whether or not the message is pinned, returns a Boolean.
* rawcontent - Message's content without _**ANY**_ mentions.
* guildname - Message's guild's name of origin.
* url - Message's URL.

```text
$msg[content]
//will return the content
```

## $role\[rid;property\]

### Properties

* name - Role's name.
* mention - Role's mention.
* id - Role's ID.
* hex - Role's hex color.
* created - Role's date and time of creation.
* position - Role's position.
* rawposition - Role's raw position.
* guild - Role's guild's id of origin.
* guildname - Role's guild's name of origin.
* timestamp - How long ago the role was created.
* isdeleted - Whether or not the role has been deleted, returns a Boolean.
* ismentionable - Whether or not the role can be mentioned, returns a Boolean.
* iseditable - Whether or not the author of the command can edit the role, returns a Boolean.
* ismanaged - Whether or not a Discord Integration manages the role, returns a Boolean.
* ishoisted - Whether or not the role is hoisted, returns a Boolean.

```javascript
$role[1979790790790789;name]
//returns the name of the role
```

## $user\[uid;property\]

### Properties

* name - User's name.
* id - User's ID.
* tag - User's Tag.
* discrim - User's discriminator.
* mention - User's mention.
* avatar - User's avatar URL.
* isbot - Whether or not the user is a bot, returns a Boolean.
* istyping - Whether or not the user is typing, returns a Boolean.
* created - User's account's date and time of creation.
* timestamp - How long ago the user was created.
* lastmessageid - User's last message ID.
* lastmessagechannelid - User's last channel ID.

```javascript
$user[1979790790790789;name]
//returns the name of the user with the id
```

## $channel\[id;property\] or $channel\[property\]

### Properties

* name - Channel's Name.
* topic - Channel's Topic.
* ID - Channel's ID.
* position - Channel's position organized by categories.
* rawposition - Channel's position.
* mention - Mentions the Channel.
* created - Channel's date and time of creation.
* isdeleted - Whether or not the channel has been deleted from the current guild, returns a Boolean.
* type - Channel's Type - `Text` **/** `Voice` **/** `Category`.
* timestamp - How long ago the channel was created.
* guildid - Channel's home guild's id.
* guildname - Channel's home guild's name.
* ismanageable - Whether or not the the author of the command has permission to manage the channel, returns a Boolean.
* parentid - Channel's category's id.
* parentname - Channel's category's name.
* isviewable - Wehther or not the author of the command can view the channel, returns a Boolean.
* isdeleteable - Whether or not the author of the command can delete the channel, returns a Boolean.

```javascript
$channel[797907907097907;name]
//returns the name of the channel
```

## $guild\[property\]

guild = Discord Server

### Properties

* name - Guild's Name. 
* id - Guild's ID.
* acronym - Guild's name acronym.
* afkchannelid - Guild's AFK Channel's ID.
* boostcount - Guild's boost count.
* boostlevel - Guild's boot level.
* created - Guild's date and time of creation.
* description - Guild's description.
* emojicount - Guild's emoji count.
* isavailable - Whether or not the guild is available, returns a Boolean.
* isbotremoved - Whether or not the bot is in the guild, returns a Boolean.
* ispartnered - Whether or not the guild is partnered, returns a Boolean.
* isverified - Whether or not the guild is verified, returns a Boolean.
* membercount - Guild's membercount.
* ruleschannel - Guild's rule channel's id.
* systemchannelid - Guild's system channel's id.
* timestamp - How long ago the guild was created.
* updateschannel - Guild's moderator news channel's id.
* verificationlvl - Guild's verification level.

```javascript
$guild[name]
//returns the name of the guild
```

## $emoji\[emojiID;property\]

### Properties

* name - Emoji's name.
* id - Emoji's ID.
* created - Emoji's date and time of creation.
* url - Emoji's URL.
* identifier - Emoji's name:ID.
* isanimated - Whether or not the emoji is animated, returns a Boolean.
* isdeleted - Whether or not the emoji is deleted, returns a Boolean.
* guildid - Emoji's guild of origin.
* ismanaged - Whether or not the emoji is a custom or discord default emoji, returns a Boolean

```javascript
$emoji[789789790790808;name]
//returns the emoji's name
```

