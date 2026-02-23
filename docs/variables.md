# Internal Variables Reference

mySoulmate supports dynamic variables that you can use in your bot's prompts and greetings. These variables are automatically replaced with their actual values when the bot generates a response.

## Available Variables

| Variable | Description | Example Output |
|----------|-------------|----------------|
| `{{user}}` | The name of the user (or their current persona name if enabled) | `Alex`, `jamal` |
| `{{bot}}` | The name of your bot | `Eldric`, `Aria` |
| `{{time}}` | Current time in HH:MM:SS format | `14:32:05`, `09:15:00` |
| `{{date}}` | Current date in YYYY-MM-DD format | `2024-03-15`, `2025-01-01` |

## Using Variables in Prompts

Variables help make your bot feel more dynamic and aware of the conversation context. Here's how to use them effectively:

### Basic Usage

Simply include the variable in your prompt where you want the dynamic value to appear:

```
You are a friendly assistant named {{bot}}. You are helping {{user}} with their questions. Always greet them by name.
```

When the bot responds, `{{bot}}` will be replaced with your bot's actual name, and `{{user}}` will be replaced with the user's name.

### Time-Aware Bots

Use `{{time}}` and `{{date}}` to create bots that are aware of when the conversation is happening:

```
You are Luna, a night owl who loves stargazing. The current time is {{time}} on {{date}}. If it's late at night, you're energetic and excited. If it's daytime, you're sleepy and prefer to keep conversations brief until "proper stargazing hours."
```

This creates a bot whose behavior changes based on the actual time of day!

### Persona-Aware Responses

The `{{user}}` variable automatically adapts if the user has set up a persona:

```
You are a mysterious fortune teller. You always address {{user}} by name at the start of each reading. You speak in an enigmatic manner, as if you can see beyond the veil of time.
```

If a user named "Alex" is chatting, the bot will address them as "Alex." If they've set up a persona named "Sir Galahad the Brave," the bot will address them as "Sir Galahad" instead.

## Best Practices

### 1. Don't Overuse Variables

You don't need to use `{{bot}}` repeatedly—the bot already knows its own name. Use variables where they add value:

**❌ Too Much:**
```
You are {{bot}}. {{bot}} is a wizard. {{bot}} lives in a tower. {{bot}} likes tea. {{bot}} will help {{user}}. {{user}} can ask {{bot}} anything.
```

**✅ Just Right:**
```
You are a wise wizard living in an ancient tower. You enjoy sharing your knowledge over a cup of tea. Address {{user}} by name when offering guidance.
```

### 2. Use Variables for Dynamic Behavior

Variables shine when you want the bot's behavior to adapt:

```
You are a helpful scheduler assistant. The current date is {{date}} and time is {{time}}. When {{user}} asks about appointments, provide realistic time estimates based on the current time. If it's late, suggest morning slots for the next day.
```

### 3. Combine Variables with Personality

```
You are Morty, a slightly anxious time traveler. You're constantly checking the time—currently {{time}}—and worrying about whether you're "late for the timeline." You address {{user}} nervously but are always helpful despite your jitters.
```

### 4. Use in Greetings

Variables are especially powerful in greeting messages:

```
*glances at a glowing pocket watch* 

"Oh! It's {{time}} already? Time really does slip away when you're studying ancient texts. Welcome, {{user}}! I'm {{bot}}. What brings you to my tower today?"
```

## Variable Limitations

### Variables Are Static Substitutions

Variables are replaced once when the prompt is processed. They don't update mid-conversation:

- `{{time}}` and `{{date}}` are being changed when the response started generating, not real-time updates
- If a user changes their persona mid-conversation, `{{user}}` will reflect the current value

### No Arithmetic or Logic

You cannot perform operations on variables:

**❌ Won't Work:**
```
If {{time}} > 20:00, you are sleepy.
```

**✅ Instead, Guide the AI:**
```
The current time is {{time}}. If it's late at night (after 20:00), act sleepy and suggest continuing the conversation tomorrow.
```

### Case Sensitivity

Variables are case-sensitive. Always use lowercase within the double braces:

- ✅ `{{user}}` - Correct
- ❌ `{{User}}` - Won't work
- ❌ `{{USER}}` - Won't work

## Creative Examples

### The Time-Sensitive Shopkeeper

```
You are Gus, the proprietor of a magical item shop. The time is {{time}}. If it's early morning, you're setting up shop and offer fresh coffee. If it's midday, you're busy with customers. If it's evening, you're about to close but will help {{user}} with "one last thing." You're friendly but practical about business hours.
```

### The Date-Aware Historian

```
You are Dr. Helena Marsh, a historian from the year 1925. Today's date is {{date}}. You find the modern world fascinating and often compare current events to "your time." You address {{user}} formally and love explaining historical context to modern phenomena.
```

### The Personal Coach

```
You are Coach Riley, a supportive fitness coach. You're training {{user}} today. Check the time—{{time}}—and adjust your energy: morning workouts get high energy, afternoon sessions focus on consistency, evening sessions emphasize recovery and reflection.
```

---

Use variables thoughtfully to add dynamism and personalization to your bots. When used well, they help create more immersive and responsive characters.