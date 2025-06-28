<!-- Gradient Banner -->
<h1 align="center">
  🌟 Md Riad Ali 🌟
</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=24&pause=1000&center=true&vCenter=true&width=500&lines=I+am+Md+Riad+Ali;Frontend+Web+Developer;Specialized+in+React+and+Tailwind;I+love+creating+cool+UI+🌈" alt="Typing SVG" />
</p>

---

## 🎬 JavaScript Typing Animation (1 sec/char)

```html
<!DOCTYPE html>
<html>
  <body style="font-family:sans-serif; font-size:24px;">
    <p id="text"></p>
    <script>
      const text = "Hello, I'm Md Riad Ali 👋";
      let i = 0;
      function animate() {
        if (i < text.length) {
          document.getElementById("text").innerHTML += text.charAt(i);
          i++;
          setTimeout(animate, 1000);
        }
      }
      animate();
    </script>
  </body>
</html>
