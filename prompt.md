# Prompt for Fractional Logic Engine Development

## Objective

Construct a single-file HTML5/JavaScript application serving as an interactive worksheet for adding and subtracting fractions with unlike denominators. Target audience: 10-11 years old.

## Functional Requirements

- Dynamic Problem Generation: Randomly generate two fractions with denominators between 2 and 12. Ensure denominators are unequal.
- Scaffolded Input: Divide the solution process into four discrete, validated steps:
    1. Find the Least Common Denominator (LCD).
    2. Convert both fractions to equivalent fractions using the LCD.
    3. Perform the operation (addition or subtraction) on the numerators.
    4. Simplify the resulting fraction to its lowest terms.

- Real-Time Validation: Input fields must turn green upon correct entry and red/shake upon incorrect entry. Block progression to the next step until the current step is solved.
- Visual Feedback: Use a progress bar to indicate completion percentage.

## Technical Specifications

- Logic Handling: Use the Greatest Common Divisor (GCD) to calculate the Least Common Multiple (LCM) for denominators.
    - `Formula: LCM(a, b) = (a - b) / GCD(a, b)`
- UI/UX:
    - Use CSS Flexbox for a centered, clean layout.
    - Implement large, accessible font sizes (min 18px).
    - Use standard fraction notation: numerator over a horizontal rule over the denominator.

- State Management: Maintain an object to track the current problem's state: `rawFractions`, `commonDenominator`, `intermediateNumerators`, and `finalSimplifiedAnswer`.

## Styling Constraints

- High contrast colors for readability.
- No external libraries (Vanilla JS/CSS only).
- Responsive design for tablet/desktop use.

## Example Interaction Logic

- User is presented with 1/3 + 1/4.
- Step 1: Input box for LCD. Correct answer: 12.
- Step 2: Two pairs of input boxes appear: [ ]/12 and [ ]/12. Correct answers: 4 and 3.
- Step 3: Input box for [ ]/12. Correct answer: 7.
- Step 4: Final simplification. If 7/12 is irreducible, user confirms. If reducible (e.g., 2/4), user must provide 1/2.
