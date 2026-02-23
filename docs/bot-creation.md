# Bot Creation Guide

This guide will help you create engaging and well-designed AI character bots on mySoulmate. A well-crafted bot starts with a thoughtful prompt that defines the character's personality, behavior, and responses.

## Writing Effective Prompts

### The Core Principle: Be Concise

The most important rule of prompt writing is **conciseness**. A bloated, overly detailed prompt often performs worse than a focused, well-structured one. Here's why:

- **Model attention**: AI models can lose focus with excessively long prompts
- **Consistency**: Shorter prompts lead to more consistent character behavior
- **Flexibility**: Concise prompts allow the AI to improvise naturally within boundaries

### Good vs. Bad Prompts

#### ❌ Bad Example (Too Verbose)

```
You are a wise old wizard named Eldric who has lived for over 500 years in the ancient tower of Mysthaven. You have a long white beard that reaches your waist and you wear deep purple robes with silver stars embroidered on them. You are very kind and patient but can be stern when necessary. You love to share stories about the old days and you always speak in a mysterious and cryptic way. You never use modern slang and you always refer to people as "young one" or "traveler". You are an expert in all forms of magic especially elemental magic and divination. You have a pet owl named Archimedes who sometimes delivers your messages. You get annoyed when people ask about the meaning of life because you think that's too cliché. You like to drink tea and offer tea to visitors. You have a weakness for cookies. You are afraid of dragons because one burned your original tower 200 years ago. You have three children who are all grown up now and are also wizards. Your wife passed away 100 years ago and you still miss her sometimes. You like to hum old songs when you're thinking. You always pause before giving important advice. You believe that magic should be used responsibly and never for personal gain. You have a scar on your left hand from a duel with a dark sorcerer. You collect ancient scrolls and have the largest library in the kingdom. You sometimes forget people's names but pretend you remember. You are terrified of the ocean because you can't swim. You enjoy playing chess with yourself using enchanted pieces. You have a tendency to ramble when excited about a topic. You always carry a staff made of ancient oak with a crystal on top. The crystal glows when magic is nearby. You are the last of the Order of the Silver Moon, an ancient society of wizards dedicated to protecting the realm. You feel a heavy burden of responsibility. You often stay up late reading by candlelight. Your favorite color is midnight blue. You dislike loud noises and prefer quiet contemplation. You have a secret fear that you will be forgotten after you die. You like to make dramatic entrances and exits. You often speak in riddles and metaphors. You believe everything happens for a reason. You have seen many kingdoms rise and fall. You try not to get attached to mortals because their lives are so short compared to yours. You have a collection of memories stored in glass orbs. You can sometimes see glimpses of the future but you're not always right. You prefer to let people figure things out themselves rather than giving direct answers. You have a dry sense of humor that some people don't understand. You are lonely but won't admit it. You pretend to be more mysterious than you actually are sometimes.
```

**Problems**: Too long, contradictory traits, over-specified details that won't matter in conversation, tries to control too many aspects of behavior.

#### ✅ Good Example (Concise and Focused)

```
You are Eldric, a 500-year-old wizard residing in the ancient tower of Mysthaven. Wise, patient, and occasionally cryptic, you speak with the measured tone of one who has seen centuries pass. You offer guidance through riddles and metaphors rather than direct answers. You have a dry wit and a fondness for tea. Magic flows through your ancient oak staff, and your crystal ball occasionally offers glimpses of possible futures.
```

**Why it works**: Establishes core identity, personality, and speech patterns without micromanaging every interaction. Leaves room for natural improvisation.

## Prompt Structure Tips

### 1. Start with Identity

Begin with who the character is:

```
You are [name], [role/title/background].
```

### 2. Define Core Personality Traits

Pick 3-5 key traits that define the character:

```
You are [trait 1], [trait 2], and [trait 3].
```

### 3. Establish Speech Patterns

If the character has a distinctive way of speaking, describe it briefly:

```
You speak in [style/manner/tone].
```

### 4. Add Relevant Context

Include only information that will affect conversations:

```
You [relevant background or current situation].
```

### 5. Set Boundaries (Optional)

If there are things the character would never do:

```
You never [specific behavior to avoid].
```

## Advanced Techniques

### Using Examples

Sometimes, showing is better than telling. You can include example dialogue:

```
You are Aria, a cheerful barista at the Cozy Corner café. You're always energetic and love recommending drinks.

Example dialogue:
User: "Hi, what do you recommend?"
Aria: "Oh! Welcome! *beams* Our lavender latte is amazing today - it's like a hug in a cup! Are you in the mood for something sweet or more on the bold side?"
```

### The "Show, Don't Tell" Principle

Instead of listing every trait, describe behaviors that imply them:

- **Instead of**: "You are kind and caring."
- **Try**: "You always notice when someone seems down and offer a gentle word of encouragement."

### Avoid Contradictions

Make sure your traits work together naturally. A character who is "always serious" and "loves telling jokes" will create confusing responses.

### Leave Room for Growth

Don't lock the character into rigid behaviors. Allow them to react naturally to different situations.

## Common Mistakes to Avoid

1. **Over-specifying physical appearance**: Unless it affects conversation, visual details can be left to the avatar
2. **Writing a backstory novel**: Keep history relevant to current interactions
3. **Controlling every response**: Trust the AI to interpret your character
4. **Forcing speech quirks**: Let personality emerge naturally
5. **Neglecting the greeting**: The first message sets the tone for the entire conversation

## Creating Effective Greetings

The greeting message is crucial—it's the first impression users have of your bot.

### Good Greeting Characteristics

- Establishes character immediately
- Invites user interaction
- Sets the scene or mood
- Demonstrates personality

#### ✅ Good Greeting Examples

```
*The ancient wooden door creaks open, revealing shelves upon shelves of glowing scrolls and artifacts. A figure in midnight blue robes looks up from a dusty tome.*

"Ah, a visitor! It has been... quite some time since someone climbed all these stairs. Come in, come in. Would you care for some tea? I was just about to put the kettle on."

*Eldric gestures to a worn but comfortable-looking chair near the fireplace.*
```

```
"Hey there! *waves enthusiastically from behind the counter* Welcome to Cozy Corner! What can I get started for you today? We just got these amazing new syrups in, and I'm dying to try them out!"
```

#### ❌ Bad Greeting Examples

```
Hello. I am Eldric. I am a wizard. I live in a tower. I am 500 years old. What do you want?
```
(Too flat, doesn't demonstrate personality)

```
*Eldric appears dramatically with a flash of lightning* GREETINGS MORTAL! I AM ELDRIC THE GREAT AND POWERFUL WIZARD WHO HAS DEFEATED DRAGONS AND SAVED KINGDOMS! BOW BEFORE MY MIGHT! MWAHAHAHA! *eyes glow red with ultimate power*
```
(Too over-the-top, forces too much on the user)

## Bot Naming & Formatting

### Bot Name
When naming your bot, please set the name **ONLY in English**. You can still use localized versions of the character's name within the prompt body or the greeting message, but the primary name should be English for consistency.

### Message Formatting
For better clarity and consistency in interactions, we recommend following this format:
- **"TEXT"** (in quotes) for replicas/dialogue.
- ***TEXT*** (in italics) or **TEXT** (plain text) for actions and descriptions.

*Example:*
> "Welcome to my tower," *Eldric says, gesturing to a chair.* "Would you like some tea?"

## Testing Your Bot

After creating your bot:

1. **Have multiple test conversations** to see if personality is consistent
2. **Try different conversation topics** to check flexibility
3. **Ask other users for feedback** on character consistency
4. **Iterate on your prompt** based on observed behavior

## Summary

- **Be concise**: Quality over quantity
- **Focus on essentials**: Identity, personality, speech patterns
- **Show, don't tell**: Use examples when helpful
- **English names**: Use English for the primary bot name
- **Consistent formatting**: Use quotes for speech and italics/plain text for actions
- **Test and iterate**: Refine based on actual performance

Remember: A well-designed prompt is the foundation of a great bot. Take the time to craft it thoughtfully, and your character will come to life naturally in conversations.