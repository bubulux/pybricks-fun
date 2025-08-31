# Solution Structure Pattern

This document defines the structure for solution files that accompany practice tasks in the Pybricks programming curriculum.

## Reference Implementation

See: `course/1-fundamentals-of-programming/1.2-data-types-operations/1.2.2-numbers/solutions.mdx`

## Overall Philosophy

Solutions serve multiple purposes:
- **Teaching tool**: Explain the reasoning behind each solution
- **Reference**: Show correct implementation patterns
- **Debugging aid**: Help students understand where they went wrong
- **Visual guide**: Provide block-based representations for implement tasks

## File Structure

### solutions.mdx Template

```mdx
import { Meta } from "@storybook/addon-docs/blocks";

<Meta title="Path/To/Topic/Solutions" />

# Topic - Solutions

---

## Easy

### Implement

#### 1. [Task Name] — solution and explanation

<img
  src="/path/to/res/SOL-1.1.png"
  alt="Implementation solution visual"
  style={{ width: "appropriate%" }}
/>

Solution (code):

```python
# Initialize variables (if needed)
variable = value

# The main program starts here
solution_code_here
```

Explanation:

- [Step-by-step breakdown of the solution]
- [Explain key concepts used]
- [Connect to learning objectives]

Expected output:

```
expected_result_here
```

#### 2. [Task Name] — solution and explanation

[Same pattern for each implement task]

#### 3. [Task Name] — solution and explanation

[Same pattern for each implement task]

### Predict

#### 4. [Task Name] — solution and explanation

Code:

```python
code_from_task_here
```

Step-by-step analysis:

- [Line-by-line execution trace]
- [Explain each operation and its result]  
- [Highlight key concepts being tested]

Expected output:

```
actual_output_here
```

#### 5. [Task Name] — solution and explanation

[Same pattern for each predict task]

#### 6. [Task Name] — solution and explanation

[Same pattern for each predict task]

---

## Medium

[Same structure as Easy, with SOL-2.X.png for implement tasks]

---

## Hard

[Same structure as Easy, with SOL-3.X.png for implement tasks]

---

## Challenge

[Same structure as Easy, with SOL-4.X.png for implement tasks]
```

## Image Policy

### Implement Solutions
- **MUST have img tags**: Shows the visual block representation
- **Naming convention**: `SOL-X.Y.png`
  - X = difficulty level (1=Easy, 2=Medium, 3=Hard, 4=Challenge)  
  - Y = task number within that difficulty's implement section
- **Purpose**: Students can see how to build the solution visually

### Predict Solutions  
- **NO img tags needed**: The code is already shown in the task
- **Reference original**: Can mention "refer to the code shown in the task"
- **Focus on analysis**: Emphasis on step-by-step reasoning

## Solution Explanation Patterns

### Implement Task Explanations

#### Structure
1. **Visual representation**: Image showing block-based solution
2. **Code solution**: Clean, well-commented Python code
3. **Step-by-step explanation**: Break down the logic
4. **Concept connections**: Link to learning objectives
5. **Expected output**: Confirm the result

#### Explanation Style
```mdx
Explanation:

- We [action taken] to [achieve goal]
- The [operation/concept] [explanation of how it works]
- [Key insight or learning point]
- This demonstrates [connection to broader concept]
```

#### Example Patterns
- "We create variables to store..."
- "The comparison asks 'Is X greater than Y?'"
- "Since [condition], the result is [outcome]"
- "This shows how [concept] works in practice"

### Predict Task Explanations

#### Structure
1. **Code display**: Show the exact code from task
2. **Step-by-step analysis**: Trace through execution
3. **Result explanation**: Why this output occurs
4. **Concept reinforcement**: What this tests/teaches

#### Analysis Style
```mdx
Step-by-step analysis:

- [Variable/operation] → [intermediate result] ([explanation])
- [Next operation] → [next result] ([why this happens])
- [Final step] → [final output] ([key insight])
```

#### Tracing Patterns
- "First, [initial state/values]"
- "Then, [operation] gives us [result]"
- "Finally, [conclusion] because [reasoning]"
- "The output shows [key concept] in action"

## Progressive Complexity in Explanations

### Easy Solutions
- **Simple explanations**: Focus on basic understanding
- **Clear connections**: Link code to concepts
- **Encouraging tone**: Build confidence
- **Foundation building**: Establish core patterns

### Medium Solutions  
- **More detail**: Explain intermediate steps
- **Pattern recognition**: Point out recurring themes
- **Application focus**: Connect to real-world scenarios
- **Building complexity**: Show how concepts combine

### Hard Solutions
- **Deep analysis**: Thorough step-by-step breakdowns
- **Edge case discussion**: Explain tricky behaviors
- **Advanced patterns**: Introduce sophisticated techniques
- **Problem-solving focus**: Emphasize analytical thinking

### Challenge Solutions
- **Expert explanations**: Assume strong foundation
- **System thinking**: Show how parts work together
- **Real-world context**: Professional programming practices
- **Mastery demonstration**: Complete understanding

## Code Style in Solutions

### Comments
- Clear, educational comments that explain why, not just what
- `# Initialize variables` for setup sections
- `# The main program starts here` for main logic
- Inline comments for complex operations

### Variable Names
- Descriptive, meaningful names
- Consistent with robotics context
- Clear purpose and scope

### Structure
- Logical organization
- Consistent formatting  
- Educational clarity over clever brevity

## Common Explanation Patterns

### For Comparisons
- "The comparison `X op Y` asks 'Is X [relationship] Y?'"
- "Since [values], this evaluates to [True/False]"

### For Logical Operations
- "The AND operation requires both conditions to be True"
- "Since [left] is [True/False] and [right] is [True/False], the result is [outcome]"

### For Variable Operations
- "We assign the result back to the variable using [pattern]"
- "Notice how the original variable [changes/stays the same]"

### For Complex Expressions
- "Working from the inside out:"
- "Following the order of operations:"
- "Let's trace through this step by step:"

## Quality Checklist

- [ ] All implement solutions have SOL-X.Y.png images
- [ ] All predict solutions have step-by-step analysis
- [ ] Explanations build understanding, not just show answers
- [ ] Code is clean, commented, and educational
- [ ] Expected outputs match exactly
- [ ] Progressive difficulty in explanation depth
- [ ] Consistent formatting and structure
- [ ] Clear connections to learning objectives
- [ ] Encourages understanding over memorization
- [ ] Addresses common misconceptions where relevant

## Error Handling in Explanations

### Common Student Mistakes
- Address typical misunderstandings in explanations
- Show why wrong approaches don't work
- Provide debugging tips and strategies

### Conceptual Clarifications
- Clarify subtle distinctions (like 5 vs 5.0)
- Explain unexpected behaviors
- Connect to broader programming concepts

### Learning Reinforcement
- Emphasize key takeaways
- Connect solutions to previous learning
- Preview how concepts will be used later
