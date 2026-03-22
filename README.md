# 💌 Interactive Love Letter — Customization Guide

A beautiful, animated love letter you can personalize and share with your special someone. Just edit a few lines and send the magic! 🌸

---

## 🌐 Live Demo

👉 **[Click here to see it live](https://anshmajumdar121.github.io/love-letter-for-you/)**

---

## 🚀 How to Customize

Open `index.html` in any text editor and find this section near the top:

```
==================== CUSTOMIZATION SECTION ====================
```

Edit the `CONFIG` object between the comments. **Do NOT touch anything outside this section** unless you know what you're doing!

---

## ✏️ What You Can Change

### 1. 👤 Name `(Line ~15)`

```js
name: "Nancy"  // Change to your person's name
```

Appears in: browser tab title, main heading "For [Name]", and greeting "My Dearest [Name]"

---

### 2. 🏷️ Tagline `(Line ~18)`

```js
tagline: "5FT+ OF PURE SUNSHINE"
```

| Example Taglines |
|-----------------|
| "The Most Beautiful Girl" |
| "My Sunshine" |
| "Taller Than My Problems" |
| *(leave blank for none)* |

---

### 3. 💬 Compliments List `(Lines ~21–29)`

Format for each compliment:

```js
{ icon: "🌟", text: "Your compliment here" }
```

Example additions:

```js
{ icon: "🎵", text: "Your laugh is my favorite sound" },
{ icon: "☕", text: "You make mornings better" },
{ icon: "🌙", text: "You shine brighter than the stars" },
```

💡 **Tip:** 7–10 compliments is the sweet spot!

---

### 4. ❓ The Question `(Line ~32)`

```js
question: "Will you be my chat partner?"
```

| Example Questions |
|------------------|
| "Will you go on a date with me?" |
| "Will you be my Valentine?" |
| "Coffee this weekend?" |

---

### 5. 🔘 Button Texts `(Lines ~35–36)`

```js
buttonYes: "Yes! 🎉"
buttonNo:  "No 🙈"    // This button runs away — it's a fun game!
```

---

### 6. 🎉 Success Message `(Lines ~39–40)`

Shown when they click **YES**:

```js
successMessage:    "I knew you were the best!"
successSubMessage: "Let's chat forever! 💕"
```

---

## 🎨 Advanced: Change Colors

Find the CSS variables at the top of the file:

```css
:root {
    --envelope-bg:     #ffe4e1;  /* Envelope main color   */
    --envelope-dark:   #ffb7c5;  /* Envelope shadow       */
    --envelope-darker: #ff9eb5;  /* Darker accents        */
}
```

Use any [online color picker](https://htmlcolorcodes.com/) to find hex codes.

---

## 📱 How to Use

1. Open `index.html` in VS Code, Notepad, or any text editor
2. 2. Find the **CUSTOMIZATION SECTION**
   3. 3. Edit the values between quotes `" "`
      4. 4. Save the file
         5. 5. Open in a browser to preview
            6. 6. Share the link or file with your special someone 💝
              
               7. ---
              
               8. ## ⚠️ Important Rules
              
               9. | Rule | Why |
               10. |------|-----|
               11. | Keep quotes around text | JavaScript needs them |
               12. | Keep commas after each item | Separates list items |
               13. | Don't delete curly braces | Wraps each compliment object |
               14. | Don't delete square brackets | Wraps the whole list |
              
               15. If something breaks, check you didn't accidentally delete a quote or comma!
              
               16. ---
              
               17. ## 💖 Full Example
              
               18. ```js
                   const CONFIG = {
                       name: "Sarah",
                       tagline: "MY FAVORITE PERSON",
                       compliments: [
                           { icon: "☕", text: "You make my mornings better" },
                           { icon: "😂", text: "Your jokes always make me laugh" },
                           { icon: "🎨", text: "You're so creative and talented" },
                           { icon: "🌟", text: "You inspire me to be better" }
                       ],
                       question: "Will you grab coffee with me?",
                       buttonYes: "Absolutely! ☕",
                       buttonNo: "No way 😜",
                       successMessage: "Best decision ever!",
                       successSubMessage: "Can't wait to see you! 💕"
                   };
                   ```

                   ---

                   ## 📂 Files in This Repo

                   | File | Purpose |
                   |------|---------|
                   | `index.html` | The main love letter — edit this! |
                   | `README.md` | This guide |
                   | `.nojekyll` | Tells GitHub Pages to serve files directly |

                   ---

                   Good luck! Hope they say **YES! 💝**

                   Made with ❤️
