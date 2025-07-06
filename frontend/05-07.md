
### CAT 3: Frontend Coding
-- curtosy Kyle Simpson, the JavaScript guru


# ✨ The *Newer* JavaScript – A Glow-Up from 2009 Onwards

JavaScript used to be that kid in class who did just enough to pass. From 2009 to 2016? Meh. Nothing too exciting happened. But then… 💥 **ES6 dropped**, and suddenly JavaScript got a makeover.

Since then, the updates have been coming in hot — smoother, cleaner, more *declarative*.
> **Declarative?** Think of it as telling the code *what* you want, not *how* to do it. Like saying “make me a sandwich” instead of listing out the entire sandwich-making process step-by-step. 🍞🥪

Let’s talk about some of the cool new tricks JS picked up in its post-ES6 era.

---

## 🎀 Template Strings – Strings, but Make Them Fancy

Back in the day, joining strings in JS was a hot mess:

```js
const name = "Alex";
const greeting = "Hello, " + name + "! Welcome.";
```
Now? Just add backticks ( ` ) and some ${} magic, and you’re golden:

## 🏷️ Tagged Template – When Strings Meet Superpowers

Okay, so you’ve seen how template strings clean up messy concatenation. But what if you want **more**? Like… format values, escape stuff, or maybe add drama? 🎭

Enter: **Tagged Templates** — a way to hook into the template string process and do custom stuff with it.

### 🧪 What it looks like:

```js
function dramatic(strings, ...values) {
  let result = "";

  for (let i = 0; i < strings.length; i++) {
    result += strings[i];

    if (i < values.length) {
      const val = values[i].toUpperCase() + "!!!";
      result += val;
    }
  }

  return result;
}

const name = "javascript";
const shout = dramatic`I LOVE ${name} so much`;
console.log(shout); // I LOVE JAVASCRIPT!!! so much
```




