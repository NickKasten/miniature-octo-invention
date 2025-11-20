# Sprint 3: Unit Converter - Beginner JavaScript Project
**DevSprint Fall 2025**

## Program Context
ACM Introduces: the DevSprint program! If you are looking for resume-building developer experience with current tools in a low-stakes, collaborative, constructive, and growth-centered environment, this is the place for you! Working on a 4-week rotation between projects and workshops, students will have the opportunity to build and present up to 3 unique, 2-week-long projects. Hope to see you there learning, building, and failing with style 😎

## What You'll Build
A simple web app that converts metric lengths (millimeters, centimeters, meters, kilometers) to imperial lengths (inches, feet, yards, miles). This project teaches you the fundamentals of JavaScript: variables, functions, DOM manipulation, and event handling.

## What's Included
This starter code provides:
- `index.html` - A complete, styled HTML page with a conversion form
- `converter.js` - JavaScript file with TODO comments guiding you step-by-step
- This README - Instructions to get started

## Getting Started

### 1. Open the Project
- Download or clone this repository to your computer
- Open the entire folder in a code editor like [VS Code](https://code.visualstudio.com/)

### 2. Preview in Browser
- Find `index.html` in your file explorer
- Right-click it and select "Open with" your web browser (Chrome, Firefox, Safari, etc.)
- OR if using VS Code, install the "Live Server" extension and click "Go Live" for auto-refresh

### 3. Start Coding!
Open `converter.js` and start filling in the TODOs. The file is organized into 5 steps:

#### STEP 1: Conversion Factors
Fill in the missing numbers. Research or calculate how many meters are in other units.

#### STEP 2: Conversion Function
Write the math to convert from one unit to another. Think: input → meters → output.

#### STEP 3: History Tracking
Create an array to store past conversions so users can see what they've converted.

#### STEP 4: Display Functions
Update the HTML page to show conversion results and history to the user.

#### STEP 5: Form Handling
Connect everything together by handling the form submission.

## Tips for Success

### Read Before You Code
Each TODO has a HINT comment. Read it carefully! It tells you exactly what to do.

### Test Frequently
After completing each TODO, save your file and refresh the browser. Test that your change works before moving to the next one.

### Use console.log()
Not sure what a variable contains? Add `console.log(variableName)` and check your browser's Developer Console (F12).

### Start Simple
Don't try to do everything at once. Complete the TODOs in order, one at a time.

### Debug Errors
If you see a blank page or nothing happens:
1. Open the browser console (F12) and check for error messages
2. The error will tell you the line number - go fix that line
3. Common mistakes: typos, missing semicolons, wrong variable names

## What You'll Learn

### JavaScript Fundamentals
- Variables and data types (numbers, strings, objects)
- Functions and parameters
- Objects and accessing properties with dot notation
- Arrays and array methods (push, map, join, reverse)

### DOM Manipulation
- Selecting HTML elements with `getElementById()`
- Getting values from form inputs
- Updating page content with `.textContent` and `.innerHTML`
- Adding CSS classes dynamically

### Event Handling
- Listening for form submissions
- Preventing default browser behavior
- Responding to user actions

### Math Operations
- Performing calculations with variables
- Chaining conversions (metric → meters → imperial)
- Rounding numbers for display

## Common Gotchas

### Problem: Form submits but page reloads
**Solution:** Make sure you have `event.preventDefault()` in your submit handler.

### Problem: NaN (Not a Number) appears
**Solution:** You forgot to convert the input value to a number. Use `Number()` or `parseFloat()`.

### Problem: Conversion is wrong
**Solution:** Check your math! Are you multiplying by the right conversion factor? Are you doing both steps (to meters, then to imperial)?

### Problem: History doesn't show
**Solution:** Did you call `displayHistory()` after adding to the array?

## Bonus Challenges

Once you complete all the TODOs, try these extensions:

### Easy
1. Add a "Clear History" button
2. Change the colors and styling
3. Add more units (nautical miles, hands, etc.)

### Medium
4. Save history to `localStorage` so it persists after page reload
5. Add a "Swap" button to reverse from/to units
6. Show the conversion formula used
7. Add input validation with helpful error messages

### Hard
8. Allow reverse conversion (Imperial to Metric)
9. Add a visual comparison ("That's about X football fields!")
10. Create a second converter for weight or temperature

## Need Help?

### Learning Resources
- [MDN JavaScript Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)
- [JavaScript.info Tutorial](https://javascript.info/)
- [freeCodeCamp JavaScript Course](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/)

### Specific Topics
- **Getting form values:** [MDN Forms Guide](https://developer.mozilla.org/en-US/docs/Learn/Forms)
- **Array methods:** [MDN Array Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
- **Template literals:** [MDN Template Literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals)

### Debugging
- **Browser DevTools:** Press F12 to open, check the Console tab for errors
- **console.log():** Your best friend for seeing what's happening in your code

## Example Solution Flow

Here's what the completed converter should do:

1. User enters "100" in the value field
2. User selects "centimeter" from the first dropdown
3. User selects "inch" from the second dropdown
4. User clicks "Convert"
5. Page shows: "100 centimeters = 39.3701 inches"
6. This conversion appears in the history below
7. User can convert again, and history keeps growing

## Project Structure

```
miniature-octo-invention/
├── index.html       ← The page structure and styling
├── converter.js     ← YOUR CODE GOES HERE
└── README.md        ← You are here!
```

## Going Further: Next Steps After Completing the TODOs

Congratulations on finishing the basic converter! Here are some ideas to keep building and learning:

### Improve the User Experience
- **Better error messages**: Instead of a generic alert, show a styled message on the page when validation fails
- **Instant conversion**: Make it convert as you type instead of clicking a button (use the `input` event)
- **Unit abbreviations**: Display "5 cm → 1.97 in" instead of the full names for a cleaner look
- **Keyboard shortcuts**: Let users press Enter to convert or Escape to clear the form

### Add Visual Polish
- **Animations**: Use CSS transitions to fade in the result or slide in history items
- **Icons**: Add small icons next to each unit type using emoji or SVG
- **Dark mode**: Add a toggle button to switch between light and dark themes
- **Mobile responsive**: Make it look great on phones by testing different screen sizes

### Expand the Functionality
- **Multiple conversion types**: Add tabs or buttons to switch between length, weight, temperature, etc.
- **Bidirectional conversion**: Automatically update both fields so users can convert in either direction
- **Comparison visuals**: Show a simple graphic (like progress bars) comparing the two measurements
- **Export history**: Let users download their conversion history as a text file or CSV

### Learn New JavaScript Concepts
- **Local storage**: Save history between page reloads (check out `localStorage.setItem()` and `localStorage.getItem()`)
- **API integration**: Fetch currency exchange rates or other real-time conversion data from a free API
- **JavaScript modules**: Split your code into separate files (one for conversions, one for display, one for history)
- **Modern JavaScript**: Refactor using arrow functions, destructuring, and other ES6+ features

### Practice Good Development Habits
- **Code organization**: Create separate functions for each small task instead of one big function
- **Comments**: Add comments explaining your logic for complex parts (but don't over-comment obvious things)
- **Version control**: Learn Git basics and commit your changes with meaningful messages
- **Testing**: Write down test cases (e.g., "100 cm should equal 39.37 in") and manually verify each one

### Connect with Other Projects
- **Share it**: Deploy your converter to GitHub Pages so others can use it
- **Get feedback**: Show it to friends and ask what features they'd want
- **Learn from others**: Look at other converter projects on GitHub for inspiration
- **Help beginners**: Once you're comfortable, help someone else learn by explaining your code

### Resources for Going Further
- **Free hosting**: [GitHub Pages](https://pages.github.com/), [Netlify](https://www.netlify.com/), [Vercel](https://vercel.com/)
- **CSS animations**: [Animate.css](https://animate.style/), [MDN CSS Animations](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations)
- **Free APIs**: [Public APIs List](https://github.com/public-apis/public-apis)
- **Icon libraries**: [Font Awesome](https://fontawesome.com/), [Heroicons](https://heroicons.com/)

## Remember

The best way to learn is to **build something you're excited about**. If weight conversion interests you more than length, modify this project! If you want to build a cooking measurement converter, go for it! The skills you learned here apply to any project.

Programming is a journey. Each feature you add teaches you something new. Celebrate small wins, and don't be afraid to break things - that's how you learn what works!

---

**DevSprint Fall 2025** - Learning, building, and failing with style
