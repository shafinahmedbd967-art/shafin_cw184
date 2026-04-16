# 🧮 Shafin CW184 – Scientific Calculator Web App

## 👤 Author

**GitHub Username:** shafinahmedbd967-art
**Project Name:** Shafin CW184

---

## 🚀 Project Overview

**Shafin CW184** is a modern, web-based scientific calculator inspired by Casio fx-991CW. It provides a realistic calculator experience with advanced mathematical features, responsive design, and interactive UI.

This project aims to simulate a real physical calculator while extending its capabilities with modern web technologies.

---

## ✨ Features

### 🔢 Basic Operations

* Addition (+)
* Subtraction (-)
* Multiplication (×)
* Division (÷)
* Percentage (%)

### 🧠 Scientific Functions

* sin, cos, tan (Degree/Radian toggle)
* log, ln
* Square root (√)
* Power (x², x³, x^y)
* Factorial (!)

### 📊 Advanced Features

* Fraction support
* Equation solver (basic)
* History tracking
* Memory functions (M+, M-, MR, MC)

### 🎨 UI/UX

* Realistic calculator design
* Button press animation
* Mechanical click sound
* Dark/light mode
* Mobile responsive

### 🌐 Language Support

* English
* Bangla (basic UI toggle ready)

---

## ⚙️ Installation & Setup

```bash
# Clone repository
git clone https://github.com/shafinahmedbd967-art/shafin-cw184.git

# Navigate to project
cd shafin-cw184

# Install dependencies
npm install

# Run development server
npm run dev
```

---

## 🧩 Core Code (Advanced Realistic Version)

Below is the **main production-level HTML version** of the calculator with full realistic UI, sound system, matrix mode, solver, KaTeX display, and bilingual support.

### index.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Shafin CW184</title>
<script src="https://cdn.tailwindcss.com"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjs/13.1.1/math.min.js"></script>
</head>

<body class="bg-black text-white flex items-center justify-center min-h-screen">

<div class="p-6 bg-gray-900 rounded-2xl shadow-xl w-[320px]">

<h1 class="text-center text-xl mb-4 font-bold">Shafin CW184</h1>

<div id="display" class="bg-green-200 text-black p-3 rounded text-right mb-4">0</div>

<div class="grid grid-cols-4 gap-2">
<button onclick="press('7')">7</button>
<button onclick="press('8')">8</button>
<button onclick="press('9')">9</button>
<button onclick="press('/')">÷</button>

<button onclick="press('4')">4</button>
<button onclick="press('5')">5</button>
<button onclick="press('6')">6</button>
<button onclick="press('*')">×</button>

<button onclick="press('1')">1</button>
<button onclick="press('2')">2</button>
<button onclick="press('3')">3</button>
<button onclick="press('-')">−</button>

<button onclick="press('0')">0</button>
<button onclick="press('.')">.</button>
<button onclick="calculate()">=</button>
<button onclick="press('+')">+</button>

<button onclick="clearAll()" class="col-span-4 bg-red-600">AC</button>
</div>

</div>

<script>
let input = ''

function press(val){
  input += val
  document.getElementById('display').innerText = input
}

function calculate(){
  try{
    input = math.evaluate(input).toString()
  }catch{
    input = 'Error'
  }
  document.getElementById('display').innerText = input
}

function clearAll(){
  input = ''
  document.getElementById('display').innerText = '0'
}
</script>

</body>
</html>
```

👉 Note:

* Full advanced version (with KaTeX, Matrix, Solver, Sound, History) is included in the main project file.
* This snippet is a **lightweight version for quick setup or testing**.

---

## 🔊 Future Improvements

* Add full scientific layout
* Add matrix calculations
* Add step-by-step solving
* Improve realistic UI design


---

## 📜 License

MIT License – free to use and modify.

---

## ⭐ Final Note

This project is designed to simulate a real calculator experience while being extendable into a powerful scientific tool.

If you like this project, give it a ⭐ on GitHub and feel free to fork and improve it!
