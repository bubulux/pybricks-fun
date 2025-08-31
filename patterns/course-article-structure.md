# Course Article Structure Pattern

This document defines the educational structure and tone for course articles in the Pybricks programming curriculum.

## Reference Implementation

See: `course/1-fundamentals-of-programming/1.2-data-types-operations/1.2.2-numbers/index.mdx`

## Target Audience

- **Primary**: Middle and high school students (ages 12-18)
- **Context**: Learning programming with LEGO robotics using Pybricks
- **Assumed knowledge**: Basic computer literacy, some math concepts

## Article Structure

### 1. Header and Introduction

```mdx
import { Meta } from "@storybook/addon-docs/blocks";

<Meta title="1. Fundamentals of Programming/1.2 Data Types & Operations/1.2.X Topic/1.2.X.1 Introduction" />

# 1.2.X.1 Topic Name - Introduction

Welcome to the [engaging opening that connects to real-world robotics]!
[Brief explanation of how this topic relates to robot programming]
```

### 2. Finding the UI Panel

- Always show students where to find relevant blocks in Pybricks Code Editor
- Include screenshot with specific panel highlighted
- Use consistent image styling: `style={{ width: "50%" }}`

### 3. What Are [Topic] in Programming?

- Start with relatable analogies (cooking ingredients, light switches, etc.)
- Provide 5-7 real-world robotics examples
- Connect abstract concepts to concrete robot behaviors
- Use bullet points for examples

### 4. Progressive Content Sections

Each major concept follows this pattern:

#### Section Header with Clear Purpose

- **Interactive opening**: "Let's start with a simple example..."
- **Prediction elements**: "Before you run this, take a moment to predict..."
- **Code example with image**: Every code block MUST have preceding img tag
- **Step-by-step breakdown**: Explain the output line by line
- **Concept reinforcement**: "This teaches us..."

#### Code Block Format

````mdx
<img src="/path/to/screenshot.png" alt="Descriptive alt text" style={{ width: "appropriate%" }} />

```python
# Initialize variables (when needed)
variable_name = value

# The main program starts here
code_example()
```
````

Expected output:

```
actual_output_here
```

````

### 5. Progressive Complexity

1. **Basic Examples**: Single concept, clear output
2. **Variable Usage**: Same operations with variables
3. **Combinations**: Multiple concepts together
4. **Advanced Applications**: Real-world scenarios
5. **Complex Examples**: Nested operations, multiple steps

### 6. Interactive Learning Elements

- **Prediction challenges**: "Can you guess what this will print?"
- **Step-by-step traces**: Break down complex operations
- **Comparison examples**: "Notice the difference between..."
- **Challenge questions**: Extend the concept

### 7. Summary Section

```mdx
## Summary - Your [Topic] Mastery Journey

Congratulations! You've just learned [brief recap]. Let's recap what you now know:

**The Basics:**
- [3-4 fundamental points]

**[Main Operations/Concepts]:**
- [Key operational knowledge]

**Advanced Tools:**
- [More sophisticated concepts covered]

**The Big Picture:**
[Connect to overall programming/robotics context]

**Next up:** [Preview of next topic and how it builds on this one]
````

## Educational Tone Guidelines

### Voice and Style

- **Conversational**: Use "you" and "your robot"
- **Encouraging**: "Congratulations!", "Perfect!", "Great job!"
- **Analogical**: Connect abstract concepts to familiar objects
- **Progressive**: Build complexity gradually
- **Interactive**: Frequent questions and predictions

### Language Patterns

- **Opening sections**: "Welcome to the [exciting/wonderful] world of..."
- **Transitions**: "Here's where things get really [powerful/interesting]..."
- **Explanations**: "Think of it like..." followed by analogy
- **Code introduction**: "Let's see this in action..."
- **Concept reinforcement**: "This shows how..."

### Technical Explanations

- **Start simple**: Basic concept first
- **Add complexity**: Build on previous knowledge
- **Use analogies**: Real-world comparisons
- **Provide context**: Why this matters for robotics
- **Show patterns**: How concepts connect

## Image Requirements

Every code block must have an accompanying image:

- **Placement**: Immediately before the code block
- **Naming**: Descriptive and consistent (e.g., `base.png`, `print_arith.png`)
- **Alt text**: Descriptive of the visual content
- **Width**: Appropriate percentage (25%, 50%, 75%, 100%)
- **Purpose**: Shows the visual block representation in Pybricks Code Editor

## Code Examples Standards

### Comments

- `# Initialize variables.` (when setting up variables)
- `# The main program starts here.` (before main logic)
- Inline comments explaining complex operations

### Variable Naming

- Descriptive names: `battery_level`, `sensor_reading`, `robot_speed`
- Consistent with robotics context
- Clear purpose and meaning

### Output Format

- Always show expected output after code
- Use proper formatting with code blocks
- Explain unexpected results (like 5.0 vs 5)

## Connection Patterns

### To Previous Topics

- "Remember from the [Variables section](../link/)"
- "Just like we learned with..."
- "Building on what we know about..."

### To Robotics Applications

- Battery management examples
- Sensor reading scenarios
- Motor control situations
- Safety system checks
- Navigation decisions

### To Next Topics

- "Next up, we'll explore..."
- "This foundation will help us..."
- "Get ready to learn..."

## Common Mistakes to Avoid

1. **Technical jargon without explanation**
2. **Missing img tags before code blocks**
3. **Skipping prediction exercises**
4. **Not connecting to robotics context**
5. **Too much complexity too quickly**
6. **Missing step-by-step explanations**
7. **Inconsistent tone or voice**
8. **Not building on previous knowledge**
