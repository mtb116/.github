# Style Guide

## Writing Format Guide
The following lists writing and format style standards for LearnHowToProgram.com. Each item below is fairly straight forward meaning if you find a violation in LHTP it should be a simple fix. Please readily make issues and PRs for the standards below.

This is a living document (a lot of it is still WIP). It's open for discussion by opening an issue in this repository.

<br>

### W3C Web Accessibility Standards
Follow the [standards in W3C](https://www.w3.org/WAI/tips/writing/) first. Here is a list of tips more relevant to us:

* [Make link text meaningful: W3C](https://www.w3.org/WAI/tips/writing/#make-link-text-meaningful)
* [Write meaningful alternative text for images: W3C](https://www.w3.org/WAI/tips/writing/#write-meaningful-text-alternatives-for-images)
    
    Alt text should be 1-2 sentences. Remember a screen reader will read alt text out loud so too lengthy alt text is annoying.

<br>

### APA Style and Grammar Guidelines
If W3C doesn't have a standard on something, then follow [APA Style and Grammar Guidelines](https://apastyle.apa.org/style-grammar-guidelines) 

1. [When to use italics](https://apastyle.apa.org/style-grammar-guidelines/italics-quotations/italics)

<br>

### Our Style Guide
Lastly, these are guidelines we use that neither W3C nor APA has an option on:

#### Describing interaction with UI
Learners can interact with LearnHowToProgram.com using various input methods: mouse, keyboard, voice to name the most common. Do not use input specific words like "click" or "type." Instead, use the alternatives listed here: 

| Don't Use | Instead use
| :--- | :--- |
| "Click the Next button to go to the next lesson" | "Go to the next lesson"
| "Click the button named Tracks" | "Go to Tracks"
| "In the search box, type..." | "In the search box, enter..." |

#### Formatting and text in instructions:
| Element | Convention | Example |
| :--- | :--- | :--- |
| Code blocks | 3 backticks with syntax highlighting.| Read GitHub docs for [code block syntax highlighting](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-and-highlighting-code-blocks)
| Code snippets that reference an existing larger code block | Backticks. Do not include plural "s" in the code snippt unless it is how it is written in the code block. | In the code block above, the `Album`s class in our application will require a model. This model should include both a `getTitle()` and `getArtist()` method. After creating these, we'll commit our project, push to GitHub, etc...|
| Key names, combinations, and sequences| Capitalize. Use bold formatting for key names and keyboard shortcuts in instructions. Don't put a space around the plus sign (+) in keyboard shortcuts.[^1] | Shift, F7, Ctrl+Alt+Del, Alt, F, O, Spacebar. <br><br>Select the **F1** key. <br><br>To open the Preview tab, select **Alt+3**.|
| Mathematical constants and variables | Italic. | *a2 + b2 = c2* |
| New terminology |  	Italicize the first mention of a new term if you're going to define it immediately in text.[^1] | Microsoft Exchange consists of both *server* and *client* components.
| Strings| When referring to strings in code, a document, a website, or UI, use sentence-style capitalization unless the text you’re referring to is capitalized differently. Enclose in quotation marks.[^1] | Select "Now is the time." <br>Find “font-family:Segoe UI Semibold” in the code. |

[^1] [Formatting text in instructions, Microsoft style guide](https://learn.microsoft.com/en-us/style-guide/procedures-instructions/formatting-text-in-instructions)
Links to sources from the table above:

#### Write code blocks to be copy/pasted   
A reader should be able to copy/paste all code in a code block and have it work; assuming the reader puts it in the right spot. Ex:

🚫 `$` indicates a bash terminal

> ```shell
> $ mkdir example_command
> ```

✅ The `$` symbol should not be included. It will break if the entire code block is copy/pasted. Include instructions for where this code block goes in the written instructions.
> ```shell
> mkdir example_command
> ```

[comment]: <> (Move this lengthy explation to wiki pages when ready.)

Although we don't actively encourage learners to copy/paste, it is still a valid and often necessary approach. Consider the reader who has reading comprehension issues. Transcribing code may be more difficult for them. Consider another reader who is stuck, their eyes are tried, and they are not seeing the typo. Copy/pasting is a reasonable problem-solving approach in this situation. 

Lastly, often our instructions require learners to flip between LHTP and their own terminals/VS Code. This is a slight violation of Clark and Mayer contiguity principle which discourages presenting exercise directions separate from the exercise. Obviously in many cases this can't be helped. Switching between documentation on the web and a code editor is part of developer's reality, but most documentation supports copy/pasting to make the process easier and faster. [Ex: React docs on ESLint plugin does not include the bash $](https://legacy.reactjs.org/docs/hooks-rules.html#eslint-plugin)


## Voice and Tone
Voice is the character whereas tone is expression of that character to the audience at hand.[^4]
For example, the voice of [Duolingo](https://www.duolingo.com/) is an energetic sociable green owl. When you first join Duolingo, the owl's tone is welcoming and encouraging. The owl wants you to be excited about learning a new language through its app. However, the owl's tone changes to pushy, and even judgemental, if you fail to regularly use the app.  

Although voice and tone is often used to describe a brand character (like Duolingo's green owl), when writing for LearnHowToProgram.com the same principles of voice and tone still apply. 

Defining voice and tone helps us to stay on the same page for writing style. 

### Voice of LearnHowToProgram
The voice of LearnHowToProgram is an Epicodus student. This student is a peer to all learners who are visiting LearnHowToProgram.

Write conversationally when writing for LearnHowToProgram. Imagine that you and the reader are pair programming. Here are some points to help put you in the right mindset: 

* You are knowledgeable, but you are eager to share your knowledge with others because you enjoy talking about code. 

* You don't know everything. When topics become more advance you will need to reference external resources.

* You are an ideal pair programming partner. Sometimes you're the driver by providing step-by-step instructions. Other times you encourage the reader to drive by providing prompts.

#### Guidelines for LearnHowToProgram's Voice

1. Use "we" as in "you and me."  

    You are pair programming with the reader. Use "we" to include the reader in your course of action.

---

2. Use plain speech and write casually.  

    Write as if you are having a conversation with another person. It helps to read your writing out loud to make sure it flows naturally. However, do not use idioms and pop culture references. Use analogies and metaphors carefully and sparingly.
---

3. Use simple vocabulary.  

    Aim to keep vocabulary at around a 5th grade level. It is better to use simple words whenever possible.

---

4. Show emotion and have opinions. 

    The developer world is full of opinions and strong feelings. We often have to write persuasively to motivate the reader to take a specific course of action. In these cases it is okay to elevate tone, use similes, metaphors, and analogies (carefully), and to quicken the pace.

### Tones of LearnHowToProgram

The tone in your writing will change depending on audience. Audience refers to the group of people you are speaking to and the context in which you are speaking to them. For example, students in week 1 vs week 15 are two separate audiences.

Below are standards for how you should change your tone depending on the audience.

Audience | Tone | ✅ Do This | 🚫 Not This
--- | --- | --- | ---
Referring to Epicodus staff, policies, expectations, assignments, etc | Don't use "we" as usual. Remember that the voice of LearnHowToProgram is a student, not a staff member.<br><br> Use "Epicodus staff..." or "Epcicodus's student handbook..." | "Epicodus advisors put together a resource on what to expect for the internship." ✅ | "We’ve put together a resource on what to expect at your internship." 🚫




[^4]["What is the difference between voice and tone?" by Kevin Potts, Evoking Brand - Medium, July 11, 2016](https://medium.com/evoking-brand/what-is-the-difference-between-voice-and-tone-5f0fca775520)