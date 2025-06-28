# 🌟 Md Riad Ali

> 🚀 Frontend Web Developer  
> Skills: **HTML**, **CSS**, **Tailwind CSS**, **JavaScript**, **React**  

---

## 👋 About Me

Hello! I'm Md Riad Ali, a passionate frontend web developer focused on creating beautiful, responsive websites with modern technologies and smooth user experiences.  

---

## 🎨 Skills & Proficiency Report

| Skill         | Level        | Progress               |
|---------------|--------------|------------------------|
| 🟧 **HTML**    | Expert       | ![95%](https://progress-bar.dev/95/?color=fc466b&title=95%)       |
| 🟦 **CSS**     | Advanced     | ![90%](https://progress-bar.dev/90/?color=3f5efb&title=90%)       |
| 🌊 **Tailwind**| Pro          | ![85%](https://progress-bar.dev/85/?color=00c9ff&title=85%)       |
| 💛 **JavaScript** | Intermediate | ![80%](https://progress-bar.dev/80/?color=f7df1e&title=80%)     |
| ⚛️ **React**    | Learning     | ![75%](https://progress-bar.dev/75/?color=61dafb&title=75%)       |

---

## 💻 JavaScript Animation Code (Types text 1 char per second)

```js
const text = "Hello, I'm Md Riad Ali 👋 A Frontend Web Developer!";
let i = 0;

function type() {
  if (i < text.length) {
    process.stdout.write(text.charAt(i));
    i++;
    setTimeout(type, 1000);
  }
}

type();
