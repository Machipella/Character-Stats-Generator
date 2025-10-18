# Character-Stats-Generator
Enter your character's name and the program randomly generates their stats.
print("Character Stats Generator")
def generate_stats(name):
    import random
    stats = {
        "Strength": random.randint(1, 20),
        "Dexterity": random.randint(1, 20),
        "Constitution": random.randint(1, 20),
        "Intelligence": random.randint(1, 20),
        "Wisdom": random.randint(1, 20),
        "Charisma": random.randint(1, 20)
    }
    print(f"Stats for {name}:")
    for stat, value in stats.items():
        print(f"{stat}: {value}")
input_name = input("Enter your character's name: ")
generate_stats(input_name)
