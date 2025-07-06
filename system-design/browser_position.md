## 📍 CSS Positioning – Who Moved My Div?

Browsers lay things out nicely by default... until you mess with `position`. Then it's every element for itself.

---

### 🔢 The Lineup

#### 🟢 `static` – The Default Dude
- Just vibes. No positioning.
- Can’t use `top`, `left`, etc.
> “I go where the flow takes me.” 🧘

---

#### 🟡 `relative` – The Sneaky Shifter
- Stays in flow, but moves *a bit*.
- Keeps its space in the layout.
- Starts a new **stacking context** if `z-index` is used.
> “I'm here… but like, slightly over there.” 👣

---

#### 🔴 `absolute` – The Lone Wolf
- Jumps out of the normal flow.
- Anchors to the nearest non-static parent.
> “I work alone. Don’t wait up.” 🕶️

---

#### 🔵 `fixed` – The Viewport VIP
- Like `absolute`, but glued to the screen.
- Ignores scrolling.
> “I’m always on top. Literally.” 📌

---

#### 🟣 `sticky` – The Clingy One
- Scrolls like `relative`… until it sticks.
> “I’m chill… until I’m not.” 😅

---

## 🧱 Stacking Contexts – The Browser’s Layer Cake

Any element with `position (not static)` + `z-index` creates a **new stacking context**.

Think of it like Photoshop layers — whoever’s higher wins.

---

### 🖼️ Visual Cheat Sheet

![Browser Positioning & Stacking Contexts](../resources/browser-positioning-stack-diagram.png)

---

🔍 **Debug tip**: Weird overlap? Vanishing buttons?  
Check your stacking context. It’s probably being dramatic. 🎭
