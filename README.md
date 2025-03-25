# C++ Module 03 - Inheritance & Derived Classes

## 🔍 Overview
This module introduces inheritance in C++ by implementing a hierarchy of ClapTrap-based classes. Each exercise builds upon the previous one, enhancing the functionality and complexity of the robots.

## Exercises Breakdown

### 📦 Exercise 00: Aaaaand... OPEN!

- Implement the ClapTrap class with the following attributes:

    - `name` (constructor parameter)

    - `hitPoints = 10`

    - `energyPoints = 10`

    - `attackDamage = 0`

- Public member functions:

    - `void attack(const std::string& target);`

    - `void takeDamage(unsigned int amount);`

    - `void beRepaired(unsigned int amount);`

- Each action costs **1 energy point**.

- Display messages for all actions, constructor, and destructor.

### 🌹 Exercise 01: Serena, my love!

- Introduce the ScavTrap class, inheriting from ClapTrap.

- Modified attributes:

    - `hitPoints = 100`

    - `energyPoints = 50`

    - `attackDamage = 20`

- Override `attack()` with a different message.

- New special function: `void guardGate();`

- Demonstrate proper construction/destruction chaining.

### 💤 Exercise 02: Repetitive work

- Introduce the **FragTrap** class, inheriting from **ClapTrap**.

- Modified attributes:

    - `hitPoints = 100`

    - `energyPoints = 100`

    - `attackDamage = 30`

- Override constructor/destructor messages.

- New special function: `void highFivesGuys();`

- Ensure proper construction/destruction chaining.

### 💎 Exercise 03: Now it’s weird!

-Introduce `DiamondTrap`, inheriting from both `FragTrap` and `ScavTrap`.

- Attributes:

    - `name` (private, constructor parameter)

    - `ClapTrap::name = name + "_clap_name"`

    - `hitPoints` (from FragTrap)

    - `energyPoints` (from ScavTrap)

    -`attackDamage` (from FragTrap)

- Overrides `attack()` (from ScavTrap).

- New special function: `void whoAmI();` (displays both names).

- Ensure **ClapTrap is instantiated only once.**

## 🔧 Compilation and Execution
- Use a **Makefile** with standard rules (`all`, `clean`, `fclean`, `re`).

- Compile with:
```sh
make
./your_program
```

## 🚫 Forbidden Functions

- **None** (all standard functions allowed).

## 📐 Testing

- Implement and submit custom tests to validate functionality.

- Ensure all constructors, destructors, and member functions work as expected.

## 📝 Notes

- Proper use of inheritance, constructors, and destructors is crucial.

- Ensure correct **resource allocation and management.**

- Recommended compiler flags: `-Wall -Wextra -Werror -Wshadow -Wno-shadow`.
## 👥 Author
[**Tudor Ursescu**](https://github.com/Tudor-Ursescu)
## 📜 License
This is an open-source project, and you are free to use, modify, and distribute it as you see fit.