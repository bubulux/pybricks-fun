# Image Requirements Pattern

This document defines the requirements and conventions for images in the Pybricks programming curriculum.

## Core Principle

**Every code block in the curriculum must have a corresponding image** that shows the visual block representation in the Pybricks Code Editor. This is essential because:

1. **Visual Learning**: Students learn through both visual blocks and text code
2. **Editor Correspondence**: Every text code has a block representation
3. **Complete Documentation**: Full coverage of both modalities
4. **Consistency**: Uniform experience across all materials

## Image Placement Rules

### Before Every Code Block

````mdx
<!-- CORRECT: Image immediately before code -->

<img src="/path/to/image.png" alt="Descriptive alt text" style={{ width: "50%" }} />

```python
code_here()
```
````

<!-- INCORRECT: Code without preceding image -->

```python
code_here()
```

````

### No Exceptions
- **Index articles**: Every code example needs an image
- **Task implementations**: NO images (would be spoilers)
- **Task predictions**: Images required (students need to see the code)
- **Solutions for implementations**: Images required (show how to build)
- **Solutions for predictions**: NO additional images (reference task images)

## File Naming Conventions

### Index Articles
Use descriptive names that reflect the content:
- `base.png` - Basic variable setup
- `print_arith.png` - Arithmetic operations with print
- `print_arith_var.png` - Arithmetic with variables
- `random.png` - Random number generation
- `more_ops.png` - Advanced mathematical operations

### Task Files

#### Predict Tasks
- **Format**: `PRED-X.Y.png`
- **X**: Difficulty level (1=Easy, 2=Medium, 3=Hard, 4=Challenge)
- **Y**: Sequential number within that difficulty's predict tasks
- **Examples**:
  - `PRED-1.1.png` - Easy difficulty, first predict task
  - `PRED-2.3.png` - Medium difficulty, third predict task
  - `PRED-4.2.png` - Challenge difficulty, second predict task

#### Implementation Solutions
- **Format**: `SOL-X.Y.png`
- **X**: Difficulty level (1=Easy, 2=Medium, 3=Hard, 4=Challenge)
- **Y**: Sequential number within that difficulty's implement tasks
- **Examples**:
  - `SOL-1.1.png` - Easy difficulty, first implement solution
  - `SOL-3.2.png` - Hard difficulty, second implement solution

### Task Implementation Naming
- **Format**: `TASK-X.Y.png` (for reference, but NOT used in tasks.mdx)
- **Purpose**: For potential future use or internal documentation
- **Note**: These should NOT appear in the actual task files

## Image Properties

### Standard Format
```mdx
<img
  src="/1-fundamentals-of-programming/1.2-data-types-operations/1.2.X-topic/res/filename.png"
  alt="Descriptive alternative text"
  style={{ width: "appropriate%" }}
/>
````

### Width Guidelines

- **Simple examples**: 25% - 50%
- **Standard examples**: 50%
- **Complex examples**: 75%
- **Very complex examples**: 100%

### Alt Text Standards

- **Descriptive**: Explain what the blocks show
- **Concise**: Brief but informative
- **Contextual**: Relevant to the surrounding content
- **Examples**:
  - "Two variables with numbers"
  - "Arithmetic operations with print statements"
  - "Complex logical expression prediction"
  - "Battery check simulation implementation"

## Directory Structure

```
course/1-fundamentals-of-programming/1.2-data-types-operations/1.2.X-topic/
├── index.mdx
├── tasks.mdx
├── solutions.mdx
└── res/
    ├── descriptive_name1.png      # For index.mdx
    ├── descriptive_name2.png      # For index.mdx
    ├── PRED-1.1.png              # Predict tasks
    ├── PRED-1.2.png
    ├── PRED-2.1.png
    ├── SOL-1.1.png               # Implementation solutions
    ├── SOL-1.2.png
    └── SOL-2.1.png
```

## Image Content Requirements

### What Images Should Show

1. **Complete block structure**: Full visual representation of the code
2. **Proper organization**: Blocks arranged as they would be in editor
3. **Clear readability**: High resolution, clear text
4. **Correct implementation**: Matches the accompanying code exactly

### Visual Standards

- **Resolution**: High enough for clear reading
- **Contrast**: Good visibility of text and blocks
- **Cropping**: Focused on relevant blocks, minimal extra space
- **Consistency**: Similar visual style across all images

## Usage by File Type

### index.mdx (Main Articles)

- **Policy**: Image before EVERY code block
- **Purpose**: Show students how to build each example
- **Naming**: Descriptive names reflecting content
- **Context**: Educational examples and demonstrations

### tasks.mdx (Practice Tasks)

- **Implement tasks**: NO images (would reveal solutions)
- **Predict tasks**: Images REQUIRED (students need visual reference)
- **Naming**: PRED-X.Y.png format
- **Context**: Testing comprehension and prediction skills

### solutions.mdx (Solution Guide)

- **Implement solutions**: Images REQUIRED (show how to build)
- **Predict solutions**: NO additional images (reference task images)
- **Naming**: SOL-X.Y.png format
- **Context**: Teaching correct implementation patterns

## Quality Checklist

### Image Technical Quality

- [ ] High resolution and clarity
- [ ] Proper cropping and framing
- [ ] Consistent visual style
- [ ] Accurate representation of code

### Implementation Quality

- [ ] Every code block has preceding image
- [ ] Correct naming convention used
- [ ] Appropriate width percentage
- [ ] Descriptive alt text provided

### Content Quality

- [ ] Image exactly matches code
- [ ] Proper block organization
- [ ] Educational value clear
- [ ] Consistent with curriculum standards

## Common Mistakes to Avoid

1. **Missing images**: Code blocks without preceding images
2. **Wrong placement**: Images not immediately before code
3. **Incorrect naming**: Not following established conventions
4. **Spoiler images**: Images in implement tasks that reveal solutions
5. **Missing predict images**: Predict tasks without visual reference
6. **Inconsistent sizing**: Inappropriate width percentages
7. **Poor alt text**: Non-descriptive or missing alternative text
8. **Wrong file paths**: Incorrect directory references

## Maintenance Guidelines

### When Adding New Content

1. Create code block
2. Generate corresponding block image
3. Add image with proper naming and placement
4. Verify image matches code exactly
5. Test display and accessibility

### When Updating Existing Content

1. Update code as needed
2. Regenerate corresponding block image
3. Verify naming conventions still apply
4. Update alt text if necessary
5. Check all references and links

### File Organization

- Keep all images in topic's `res/` directory
- Use consistent naming across similar content
- Document special cases or exceptions
- Maintain clean directory structure
