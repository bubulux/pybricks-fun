# Task Structure Pattern

This document defines the structure for practice tasks and solutions in the Pybricks programming curriculum.

## Reference Implementation

See: `course/1-fundamentals-of-programming/1.2-data-types-operations/1.2.2-numbers/tasks.mdx` and `solutions.mdx`

## Overall Structure

Each topic has exactly **24 tasks** organized as:

- **Easy**: 6 tasks (3 implement + 3 predict)
- **Medium**: 6 tasks (3 implement + 3 predict)
- **Hard**: 6 tasks (3 implement + 3 predict)
- **Challenge**: 6 tasks (3 implement + 3 predict)

## Task Types

### Implement Tasks

- **Purpose**: Students write code to solve a problem
- **Image policy**: **NO img tags** (would be spoilers)
- **Structure**: Goal description + expected output only
- **Numbering**: Sequential within each difficulty level

### Predict Tasks

- **Purpose**: Students predict output of given code
- **Image policy**: **MUST have img tags** (students need visual representation)
- **Structure**: Question + img + code block
- **Image naming**: `PRED-X.Y.png` format

## File Structure

### tasks.mdx Template

```mdx
import { Meta } from "@storybook/addon-docs/blocks";

<Meta title="Path/To/Topic/Tasks" />

# Topic - Tasks

Below are practice tasks based only on the material covered so far: [list relevant topics].
We'll provide a separate solutions article later — try these on your own first.

Rules:

- The tasks can be solved with the things you have learned so far.
- You can use everything from the [relevant] sections
- But you cannot use anything else from other sections (like control flow, loops, etc.)

---

## Easy

### Implement

#### 1. [Task Name]

Goal: [Clear description of what to build]

Expected output:
```

expected_result_here

```

#### 2. [Task Name]

Goal: [Clear description of what to build]

Expected output:
```

expected_result_here

```

#### 3. [Task Name]

Goal: [Clear description of what to build]

Expected output:
```

expected_result_here

````

### Predict

#### 4. [Task Name]

What will this code print?

<img
  src="/path/to/res/PRED-1.1.png"
  alt="Descriptive prediction alt text"
  style={{ width: "appropriate%" }}
/>

```python
code_to_predict_here
````

#### 5. [Task Name]

What will this code print?

<img
src="/path/to/res/PRED-1.2.png"
alt="Descriptive prediction alt text"  
 style={{ width: "appropriate%" }}
/>

```python
code_to_predict_here
```

#### 6. [Task Name]

What will this code print?

<img
src="/path/to/res/PRED-1.3.png"
alt="Descriptive prediction alt text"
style={{ width: "appropriate%" }}
/>

```python
code_to_predict_here
```

---

## Medium

### Implement

#### 7. [Task Name]

[Same pattern as Easy, but more complex]

#### 8. [Task Name]

[Same pattern as Easy, but more complex]

#### 9. [Task Name]

[Same pattern as Easy, but more complex]

### Predict

#### 10. [Task Name]

[Same pattern as Easy, with PRED-2.X.png images]

#### 11. [Task Name]

[Same pattern as Easy, with PRED-2.X.png images]

#### 12. [Task Name]

[Same pattern as Easy, with PRED-2.X.png images]

---

## Hard

### Implement

#### 13. [Task Name]

[Same pattern, more sophisticated problems]

#### 14. [Task Name]

[Same pattern, more sophisticated problems]

#### 15. [Task Name]

[Same pattern, more sophisticated problems]

### Predict

#### 16. [Task Name]

[Same pattern as Easy, with PRED-3.X.png images]

#### 17. [Task Name]

[Same pattern as Easy, with PRED-3.X.png images]

#### 18. [Task Name]

[Same pattern as Easy, with PRED-3.X.png images]

---

## Challenge

### Implement

#### 19. [Task Name]

[Advanced real-world scenarios]

#### 20. [Task Name]

[Advanced real-world scenarios]

#### 21. [Task Name]

[Advanced real-world scenarios]

### Predict

#### 22. [Task Name]

[Complex prediction scenarios with PRED-4.X.png images]

#### 23. [Task Name]

[Complex prediction scenarios with PRED-4.X.png images]

#### 24. [Task Name]

[Complex prediction scenarios with PRED-4.X.png images]

```

## Difficulty Progression

### Easy (Tasks 1-6)
- **Implement**: Basic usage of single concepts
- **Predict**: Simple, single-operation code
- **Goals**: Build familiarity and confidence

### Medium (Tasks 7-12)
- **Implement**: Combining 2-3 concepts, real-world scenarios
- **Predict**: Multi-step operations, variable interactions
- **Goals**: Apply knowledge in practical contexts

### Hard (Tasks 13-18)
- **Implement**: Complex multi-step problems, edge cases
- **Predict**: Nested operations, order of operations
- **Goals**: Deep understanding and problem-solving

### Challenge (Tasks 19-24)
- **Implement**: Real-world robotics scenarios, system design
- **Predict**: Complex expressions, advanced patterns
- **Goals**: Mastery and application to authentic problems

## Image Naming Convention

### Predict Task Images
- **Format**: `PRED-X.Y.png`
- **X**: Difficulty level (1=Easy, 2=Medium, 3=Hard, 4=Challenge)
- **Y**: Task number within that difficulty's predict section
- **Example**: `PRED-2.3.png` = Medium difficulty, 3rd predict task

### Implementation Task Images
- **Policy**: **NO IMAGES** in tasks.mdx
- **Rationale**: Would reveal the solution structure
- **Exception**: Only in solutions.mdx with `SOL-X.Y.png` format

## Task Content Guidelines

### Implement Task Goals
- **Be specific**: "Create a variable X, then do Y, then print Z"
- **Provide context**: "Simulate a battery check..."
- **Show expected output**: Always include the exact expected result
- **Build progressively**: Each task slightly more complex than previous

### Predict Task Code
- **Show realistic code**: Code that students might actually write
- **Build on concepts**: Use patterns from the article
- **Vary complexity**: Start simple, build to complex within each level
- **Test understanding**: Focus on common misconceptions or tricky cases

### Context Themes
- **Battery management**: Levels, charging, power saving
- **Sensor readings**: Distance, color, pressure detection
- **Motor control**: Speed, direction, timing
- **Safety systems**: Multiple condition checking
- **Navigation**: Position, obstacles, pathfinding

## Common Task Patterns

### Implement Tasks
1. **Variable creation + operation**: "Create variables X and Y, then..."
2. **Simulation scenarios**: "Simulate a robot that..."
3. **Multi-step processes**: "First check A, then do B, finally print C"
4. **Real-world applications**: "Design a safety system that..."

### Predict Tasks
1. **Step-by-step evaluation**: Code that requires following execution order
2. **Variable tracking**: Code where variable values change over time
3. **Operation precedence**: Code testing understanding of operator priority
4. **Edge cases**: Code with potentially surprising results

## Quality Checklist

- [ ] Exactly 24 tasks total (6 per difficulty level)
- [ ] 3 implement + 3 predict per difficulty level
- [ ] No img tags on implement tasks
- [ ] All predict tasks have img tags with correct PRED-X.Y.png naming
- [ ] Sequential task numbering (1-24)
- [ ] Progressive difficulty within and across levels
- [ ] Consistent formatting and structure
- [ ] Clear, specific goals for implement tasks
- [ ] Realistic, educational code for predict tasks
- [ ] Expected outputs provided for implement tasks
- [ ] Robotics context maintained throughout
```
