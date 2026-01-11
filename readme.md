# How to Build Your Own Educational Web Apps (For Teachers)

Welcome! This guide explains how you can turn a simple lesson idea into an interactive web application, even if you don't know how to code. We use Artificial Intelligence (like ChatGPT or Google Gemini) to do the heavy lifting.

The process has 3 main steps:
1.  **Write your Idea (The Spec)**
2.  **Create a Technical Blueprint (The Prompt)**
3.  **Build the App (The Code)**

---

## Step 1: Write Your Idea (`spec.md`)

First, write down exactly what you want your app to do in plain English. Think of this as explaining your idea to a colleague. We call this the "Specification" or `spec.md`.

**What to include:**
*   **Goal:** What should the student learn?
*   **Audience:** How old are the students?
*   **Steps:** What exactly happens on the screen? Step-by-step.
*   **Feedback:** What happens when they are right? What about when they are wrong?

**Example:**
See the included `spec.md` file for an example of a teacher wanting a fraction addition tool.

---

## Step 2: Create the Blueprint (`prompt.md`)

Now, we need to translate your friendly idea into instructions that an AI developer understands perfectly. We call this the `prompt.md`.

You can actually ask the AI to help you do this!

**Action:**
Copy your text from `spec.md` and paste it into ChatGPT/Gemini with this request:

> "I am a non-technical teacher. Please take this app idea and rewrite it into a strict, professional technical prompt for a developer. It should include sections for: Objective, Functional Requirements, Technical Specifications (HTML5/JS only), and Example Interaction Logic."

**Why this step matters:**
Role-playing as a rigorous technical lead forces the AI to think about edge cases (like "what if the denominator is 0?") and structure the code better.

See `prompt.md` for what a polished blueprint looks like.

---

## Step 3: Build the App (`index.html`)

Finally, you will use your blueprint to generate the actual application.

**Action:**
1.  Copy the entire text of your new `prompt.md`.
2.  Paste it into a **new** ChatGPT/Gemini chat.
3.  Add this instruction at the top:
    > "Please build this application as a single-file HTML solution (index.html). Include all CSS and JavaScript inside the file so I can just run it by double-clicking."

**The Result:**
The AI will write a long block of code.
1.  Copy that code.
2.  Create a new file on your computer named `index.html`.
3.  Paste the code in and save.
4.  Double-click `index.html` to open it in your browser.

Voila! You have your own custom educational tool.

---

## Tips for Success
*   **Iterate:** If the app isn't quite right, don't give up! Go back to Step 2, update your `prompt.md` with the correction, and generate the code again.
*   **Keep it Simple:** Single-file HTML apps are the easiest to manage and share. You can email them or put them on a USB drive.
