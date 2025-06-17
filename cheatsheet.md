# Python Magic Kingdom Cheat Sheets ✨

## 🚀 Basic Python Spells (Syntax)

### Essential Magic Commands
```python
# Print to the magical console
print("Welcome to the Python Kingdom!")

# Variable enchantments
hero_level = 25
magic_power = 99.5
is_chosen_one = True

# Magical comments
# This is a single spell comment
"""
This is a multi-line
magical incantation
"""

# Gather wisdom from users
hero_name = input("What is your name, brave adventurer? ")

# Discover the nature of your magic
print(type(hero_level))  # <class 'int'>

# Transform magic types
level_str = str(hero_level)        # "25"
power_int = int("42")              # 42
magic_float = float("3.14")        # 3.14
```

## 📚 Enchanted Data Structures

### Lists - Your Adventuring Party
```python
# Assemble your party
party_members = ["Hero", "Wizard", "Rogue", "Healer"]

# Meet your first companion
first_member = party_members[0]    # "Hero"

# Select part of your party
active_party = party_members[1:3]  # ["Wizard", "Rogue"]

# Recruit new members
party_members.append("Dragon")

# Say farewell to a member
party_members.remove("Rogue")

# Count your allies
party_size = len(party_members)
```

### Tuples - Unchanging Prophecies
```python
# Ancient prophecy (immutable)
prophecy = ("Chosen One", "Will Rise", "Kingdom", "Saved")
first_word = prophecy[0]  # "Chosen One"
```

### Sets - Unique Magical Artifacts
```python
# Collection of unique artifacts
artifacts = {"Excalibur", "Magic Ring", "Crystal Ball", "Phoenix Feather"}
artifacts.add("Dragon Scale")
```

### Dictionaries - The Royal Registry
```python
# Character stats registry
character_stats = {
    "Hero": {"level": 25, "hp": 100, "magic": 50},
    "Wizard": {"level": 30, "hp": 80, "magic": 95}
}

# Access character info
hero_level = character_stats["Hero"]["level"]

# Add new character
character_stats["Rogue"] = {"level": 20, "hp": 90, "magic": 15}
```

## 🎯 Control Flow Magic

### Decision Spells (If Statements)
```python
# Simple decision
if hero_level > 20:
    print("You are a powerful adventurer!")

# Binary choice
if magic_power >= 50:
    print("Your magic is strong!")
else:
    print("You need more training!")

# Multiple paths
if hero_level >= 50:
    print("You are a legendary hero!")
elif hero_level >= 25:
    print("You are an experienced adventurer!")
else:
    print("You are just starting your journey!")
```

### Loop Enchantments
```python
# For loop - Practice your spells
for spell_level in range(1, 6):
    print(f"Casting level {spell_level} spell!")

# While loop - Train until mastery
training_level = 0
while training_level < 10:
    print(f"Training session {training_level + 1}")
    training_level += 1

# Break - Emergency escape
for monster in range(10):
    if monster == 5:
        print("Dragon appeared! Retreat!")
        break
    print(f"Fighting monster {monster + 1}")

# Continue - Skip weak enemies
for enemy_power in range(10):
    if enemy_power < 3:
        continue  # Skip weak enemies
    print(f"Fighting enemy with power {enemy_power}")
```

## ⚡ Functions - Your Spell Book

### Basic Spell Creation
```python
# Simple spell
def cast_healing_spell():
    print("✨ Healing light surrounds you!")

# Spell with parameters
def greet_adventurer(name):
    print(f"Welcome to the kingdom, {name}!")

# Spell that returns magic
def calculate_damage(attack, defense):
    return max(0, attack - defense)

# Quick spell (Lambda magic)
power_boost = lambda base_power, multiplier: base_power * multiplier
```

### Advanced Spell Patterns
```python
# Spell with default enchantments
def cast_fireball(damage=25, mana_cost=10):
    return f"Fireball deals {damage} damage, costs {mana_cost} mana"

# Spell with multiple return values
def level_up_stats():
    return 10, 5, 3  # hp_gain, mana_gain, skill_points

hp_gain, mana_gain, skills = level_up_stats()
```

## 📜 String Sorcery

### Text Manipulation Magic
```python
# Combine magical words
hero_title = "Sir" + " " + "Brave" + "heart"
# OR using f-strings (more magical!)
hero_title = f"Sir Braveheart"

# Measure the power of words
name_length = len("Excalibur")  # 9

# Transform text magic
battle_cry = "for the kingdom!".upper()  # "FOR THE KINGDOM!"
whisper = "QUIET SPELL".lower()          # "quiet spell"

# Extract magical essence
magic_word = "Abracadabra"[0:5]  # "Abrac"

# Seek hidden words
spell_book = "Learn Python Magic"
python_location = spell_book.find("Python")  # 6

# Transform spells
new_spell = spell_book.replace("Python", "Coding")

# Break apart incantations
spell_parts = "Fire, Water, Earth, Air".split(", ")
```

## 📖 Scroll Management (File Handling)

### Reading Ancient Texts
```python
# Open the ancient scroll
with open("prophecy.txt", "r") as scroll:
    prophecy = scroll.read()

# Read line by line for power
with open("spells.txt", "r") as spell_book:
    spells = spell_book.readlines()

# Write new legends
with open("hero_story.txt", "w") as story:
    story.write("Once upon a time, a hero learned Python...")
```

## 🎨 List Comprehension Wizardry

### Efficient Magic Creation
```python
# Create power levels for all party members
power_levels = [member_level ** 2 for member_level in range(1, 6)]
# Result: [1, 4, 9, 16, 25]

# Filter worthy adventurers
worthy_heroes = [level for level in range(1, 21) if level >= 10]
# Result: [10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]

# Transform character names
party_names = ["alice", "bob", "charlie"]
royal_names = [name.title() + " the Brave" for name in party_names]
```

## 🛡️ Error Handling - Protective Spells

### Shield Against Magical Mishaps
```python
# Basic protection spell
try:
    magic_result = 100 / 0
except ZeroDivisionError:
    print("🛡️ Cannot divide magical energy by zero!")

# Comprehensive protection
try:
    risky_spell = dangerous_magic()
except ValueError as e:
    print(f"⚠️ Spell casting error: {e}")
except Exception as e:
    print(f"🚨 Unexpected magical mishap: {e}")
finally:
    print("🌟 Spell casting session complete!")
```

## 📚 Magical Libraries & Imports

### Summoning External Magic
```python
# Import the math grimoire
import math
circle_area = math.pi * (5 ** 2)

# Summon specific spells
from random import choice, randint
random_spell = choice(["Fireball", "Ice Storm", "Lightning"])

# Install new magical libraries
# Terminal command: pip install requests pandas numpy

# Data Science Magic
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

# Create magical data
heroes_df = pd.DataFrame({
    "Name": ["Arthur", "Merlin", "Guinevere"],
    "Level": [50, 99, 45],
    "Class": ["Warrior", "Mage", "Paladin"]
})

# Analyze your data
print(heroes_df.describe())
high_level_heroes = heroes_df[heroes_df["Level"] > 40]
```

## 🔢 NumPy - Numerical Sorcery

### Array Magic for Advanced Calculations
```python
import numpy as np

# Create magical arrays
damage_rolls = np.array([8, 12, 6, 15, 10])
party_levels = np.array([25, 30, 22, 28, 26])

# Array transformations
boosted_damage = damage_rolls * 1.5
level_advantage = party_levels + 5

# Statistical insights
average_damage = np.mean(damage_rolls)
max_level = np.max(party_levels)
level_variance = np.std(party_levels)

# Reshape for battle formations
battle_grid = np.array([1, 2, 3, 4, 5, 6]).reshape(2, 3)
```

## 📊 Matplotlib - Charting Your Adventures

### Visualize Your Journey
```python
import matplotlib.pyplot as plt

# Plot your level progression
days = [1, 2, 3, 4, 5]
levels = [1, 3, 7, 12, 20]
plt.plot(days, levels, marker='o')
plt.title("Hero's Level Progression")
plt.xlabel("Days")
plt.ylabel("Level")
plt.show()

# Bar chart of party stats
party_members = ["Hero", "Wizard", "Rogue"]
power_levels = [85, 95, 70]
plt.bar(party_members, power_levels, color=['gold', 'blue', 'green'])
plt.title("Party Power Levels")
plt.show()

# Scatter plot of damage vs level
plt.scatter(party_levels, damage_rolls, alpha=0.7)
plt.title("Level vs Damage Output")
plt.show()
```

## 🎯 Pro Tips from the Magic Kingdom

### Wisdom from Experienced Adventurers
```python
# Use enumerate for indexed adventures
party = ["Hero", "Mage", "Rogue"]
for index, member in enumerate(party):
    print(f"Position {index + 1}: {member}")

# Zip for parallel quests
names = ["Arthur", "Merlin", "Lancelot"]
classes = ["Knight", "Wizard", "Paladin"]
for name, char_class in zip(names, classes):
    print(f"{name} the {char_class}")

# Dictionary methods for efficient lookups
character_info = {"Arthur": 50, "Merlin": 99}
for name, level in character_info.items():
    print(f"{name} is level {level}")

# List slicing mastery
party_members = ["Tank", "DPS", "Healer", "Support", "Buffer"]
front_line = party_members[:2]      # First 2
back_line = party_members[2:]       # Rest
every_other = party_members[::2]    # Every 2nd member
reversed_party = party_members[::-1] # Reverse order
```

---

*"Remember, young adventurer: The most powerful magic comes from understanding, practice, and a willingness to debug your spells!"* ✨🏰
