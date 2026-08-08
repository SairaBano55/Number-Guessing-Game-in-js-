🎯 Number Guessing Game | JavaScript Loop Mastery

## Description
This repository contains a fully functional, interactive **Number Guessing Game** built with pure JavaScript. The game challenges players to find a hidden secret number within 3 attempts. It is a highly effective practice file showcasing efficient loop control, accurate variable updates, and strict user input evaluation.

---

## ⚡ Key Programming Concepts Applied
* **Dynamic Loop Management:** Running a standard `while` loop that depends entirely on a decrementing counter state (`chances > 0`).
* **Input Data Type Parsing:** Wrapping browser prompts inside the `Number()` method to enforce strict numeric comparisons.
* **State Decrementing:** Using the arithmetic post-decrement operator (`chances--`) inside the execution block to control game progression.
* **Loop Braking Mechanism:** Utilizing the `break` command to instantly stop operations once the correct target is reached, preventing redundant loops.
* **Dynamic Conditional Trees:** Employing sequential `if-else if-else` expressions to evaluate higher, lower, and exact value matches.

---

## 💻 Source Code

Here is the exact bug-free source code configured in this repository:

```javascript
let number = 6;
let chances = 3;

while(chances > 0){
   
   let num = Number(prompt("Guess the number between 1 to 10"));

   if(num < number){
       alert("Too Low");
   }
   else if(num > number){
       alert("Too High");
   }
   else{
        alert("🎉🎊🎉 CONGRATULATIONS! 🎉🎊🎉\n\n🏆 You Won, Champ! 🏆\n🥳🥳🥳 PARTY TIME! 🥳🥳🥳");
         break;
   }

     chances--;

   }

  if (chances === 0) { 
     alert("💥 GAME OVER 💥\n\n😢 Better luck next time!\n🎯 The number was " + number);
}
```

---

## 📊 Game Logic Flow Matrix

| Game Iteration State | Guess Value Evaluation | Alert Feedback Window | Loop Behavior Status |
| :--- | :--- | :--- | :--- |
| **Chances remaining** | Target value is smaller | `"Too Low"` | Deducts 1 chance; loops again |
| **Chances remaining** | Target value is larger | `"Too High"` | Deducts 1 chance; loops again |
| **Chances remaining** | Target value matches (`6`) | `"CONGRATULATIONS!"`| Hits `break`; exits instantly |
| **Chances hit `0`** | No successful matches | `"GAME OVER"` | Terminates; shows correct number |

---

## 🖥️ Expected Gameplay Scenarios

1. **Winning Sequence:**
   * Player prompts `3` ➡️ `"Too Low"` (Chances left: 2)
   * Player prompts `6` ➡️ `"CONGRATULATIONS!"` 🎉 (Game ends successfully)

2. **Losing Sequence:**
   * Player prompts `2` ➡️ `"Too Low"` (Chances left: 2)
   * Player prompts `9` ➡️ `"Too High"` (Chances left: 1)
   * Player prompts `5` ➡️ `"Too Low"` (Chances left: 0) ➡️ `"GAME OVER"` 💥

---

## 🚀 Execution Guide

1. Because this script interacts directly with window alerts and user input bars, it **must run inside a browser layout**.
2. Open any active browser tab.
3. Access your developer dashboard console by hitting `F12` (or Right-Click ➡️ **Inspect**).
4. Head straight over to the **Console** sub-tab layout.
5. Paste this entire clean code block and press **Enter**.
6. Follow the pop-up screens to play!

---
*Perfecting loops and states is a major step forward. Happy coding, keep raising the bar!* 🚀

## ✍️ Author
- GitHub: [SairaBano55](https://github.com/SairaBano55)
