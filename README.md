# Deterministic Finite Automaton (DFA) Implementation

## Overview

This project is a Java implementation of a Deterministic Finite Automaton (DFA). A DFA is a computational model used in automata theory to recognize patterns and process strings belonging to specific formal languages. It is widely used in the fields of computer science, particularly in language parsing and lexical analysis.

The project consists of three main classes: `DFA`, `Transition`, and `Main`, which work together to simulate a DFA that processes input strings to determine whether they are accepted by the given state machine.

## Components

### 1. DFA Class (`DFA.java`)
The `DFA` class is responsible for defining the structure of the automaton. It contains:
- **States**: A list of all possible states in the DFA.
- **Alphabet**: A set of allowed characters.
- **Transitions**: Defines the transitions between states based on the input character.
- **Start State**: The initial state where processing starts.
- **Accept States**: A set of states that are designated as accepting (or final) states.

Key methods include:
- `addTransition()`: Adds a transition rule to the DFA.
- `processString()`: Processes an input string and determines if it is accepted or rejected by the DFA based on the defined transitions.

### 2. Transition Class (`Transition.java`)
The `Transition` class represents the transition between states based on the input character. It contains:
- **Current State**: The state from which the transition starts.
- **Input Symbol**: The character that triggers the transition.
- **Next State**: The state to which the DFA transitions after consuming the input symbol.

This class helps manage the transition rules in a structured and readable way, allowing the `DFA` class to efficiently determine state transitions.

### 3. Main Class (`Main.java`)
The `Main` class serves as the entry point for the application. It is responsible for:
- Creating an instance of the `DFA` class.
- Defining the states, alphabet, transitions, start state, and accept states.
- Accepting user input to test different strings against the DFA.
- Displaying whether the given strings are accepted or rejected based on the DFA's rules.

## How to Use
1. **Clone the Repository**:
   ```sh
   git clone https://github.com/YourUsername/DFA-Implementation.git
   cd DFA-Implementation
   ```

2. **Compile the Java Files**:
   ```sh
   javac Main.java DFA.java Transition.java
   ```

3. **Run the Program**:
   ```sh
   java Main
   ```
   You will be prompted to enter strings to check if they are accepted by the DFA.

## Example Usage
The DFA is defined with specific states and transitions. When you run the program, you can enter strings, and the DFA will determine if they belong to the recognized language by:
- Moving between states based on the input string.
- Reaching an accept state or rejecting the string if no valid transition exists.

An example interaction:
- Enter the string: `abba`
- Output: `The string 'abba' is accepted by the DFA.`

## Features
- **Customizable DFA**: The states, transitions, and alphabet can be easily modified to represent different automata.
- **Input Validation**: Ensures that only characters from the defined alphabet are processed.
- **Console Interaction**: Allows users to input strings interactively for immediate feedback.

## Future Improvements
- **Graphical Representation**: Add a feature to visualize the DFA transitions graphically.
- **Enhanced User Interface**: Develop a GUI for better interaction.
- **Non-Deterministic Finite Automaton (NFA)**: Extend the implementation to include support for NFAs and conversion between NFA and DFA.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Contributing
Contributions are welcome! Feel free to submit pull requests or open issues for bug reports, feature requests, or enhancements.

## Contact
For any questions or issues, please contact [Your Name](mailto:youremail@example.com).

