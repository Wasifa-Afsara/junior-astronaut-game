# 🚀 Junior Astronaut Mission Trainer

A fun, kid-friendly browser game where you train as an astronaut, survive on the Moon, and fly safely home to earn your diploma.

**▶️ Play now:** [junior-astronaut-game.vercel.app](https://junior-astronaut-game.vercel.app)

---

## 🎮 How to Play

1. Press **Start Mission**.
2. Type your name and pick an animal astronaut (🐶 🐰 🐱 🦉 🐻 🦁).
3. Complete 3 levels with 3 tasks each. Robo-Buddy 🤖 gives you a hint for every task.
4. Earn **50 XP** for each task you finish.
5. Finish all 9 tasks to get your **Junior Astronaut Diploma**, which you can print.

Every task starts with 3 ❤️. If you run out of hearts, you recharge and try the task again.

## 🌍 Levels

| Level | Theme | What you learn |
|-------|-------|----------------|
| 1 | Earth Workshop | Oxygen levels, radiation shielding, solar power |
| 2 | Moon Survival | Fixing air leaks, growing food, saving power |
| 3 | Return to Earth | Radiation storms, counting supplies, launch checklist |

## 🧩 Task Types

- **Slider**: set a value (like oxygen at 21%) and hold it steady.
- **Pick**: choose the best answer from a few options.
- **Tap all**: tap every item (like air leaks) to fix them.
- **Order**: tap the steps in the correct order.

## 📁 Project Structure

```
junior-astronaut-game/
├── index.html   ← HTML, CSS and JavaScript all in one file
└── README.md
```

Everything lives in `index.html`:

- `<style>` block at the top: all the CSS
- HTML screens in the middle: start, setup, play, diploma
- `<script>` block at the bottom: game data (`LEVELS`) and game code

## 🛠️ Run It Locally

No installs or build tools needed.

1. Download or clone the repo:
   ```bash
   git clone https://github.com/Wasifa-Afsara/junior-astronaut-game.git
   ```
2. Open `index.html` in any modern browser.

## ✏️ Add Your Own Tasks

Open `index.html` and find the `LEVELS` array in the `<script>` section. Each task is a small object, so you can change the questions, hints and answers, or add new ones. Each level shows "Task X of 3", so keep 3 tasks per level unless you update that text.

Example of a **pick** task:

```js
{ type:'pick', title:'☀️ Generate Power',
  hint:'Solar panels need lots of direct sunlight.',
  q:'Where should we place the solar panels?',
  opts:[['🌧️','Storm Valley','Clouds block the sun'],
        ['⛰️','Sunny Hilltop','Clear sky, no shadows']],
  a:1,                       // index of the correct option
  done:'The hilltop gives us maximum power!' }
```

## 🚀 Deployment

The game is hosted on [Vercel](https://vercel.com). Changes pushed to the `main` branch redeploy automatically.

## 🧰 Built With

- HTML5
- CSS3
- Vanilla JavaScript (no libraries or frameworks)
- Web Audio API for sound effects


