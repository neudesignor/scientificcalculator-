<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    * { box-sizing: border-box; font-family: 'Segoe UI', Arial; }
    body { margin: 0; padding: 10px; background: #f0f0f0; display: flex; justify-content: center; align-items: center; min-height: 100vh; }
    .calculator { width: 100%; max-width: 400px; background: #222; border-radius: 20px; box-shadow: 0 10px 30px rgba(0,0,0,0.3); overflow: hidden; }
    .display { background: #1a1a1a; color: white; padding: 20px; text-align: right; }
    .history { min-height: 20px; font-size: 1rem; color: #aaa; }
    .current { font-size: 2.5rem; min-height: 60px; overflow: hidden; text-overflow: ellipsis; }
    .buttons { display: grid; grid-template-columns: repeat(5, 1fr); gap: 8px; padding: 15px; }
    button { border: none; border-radius: 50%; height: 60px; font-size: 1.2rem; background: #333; color: white; }
    .num { background: #505050; }
    .op, .func { background: #ff9500; }
    .equals { background: #34c759; grid-column: span 2; border-radius: 30px; }
  </style>
</head>
<body>
  <div class="calculator">
    <div class="display">
      <div class="history" id="history"></div>
      <div class="current" id="display">0</div>
    </div>
    <div class="buttons">
      <button class="func" data-value="mc">MC</button>
      <button class="func" data-value="mr">MR</button>
      <button class="func" data-value="m+">M+</button>
      <button class="func" data-value="m-">M-</button>
      <button class="func" data-value="ac">AC</button>
      
      <button class="op" data-value="sin">sin</button>
      <button class="op" data-value="cos">cos</button>
      <button class="op" data-value="tan">tan</button>
      <button class="op" data-value="(">(</button>
      <button class="op" data-value=")">)</button>
      
      <button class="op" data-value="log">log</button>
      <button class="op" data-value="ln">ln</button>
      <button class="op" data-value="√">√</button>
      <button class="op" data-value="^">^</button>
      <button class="op" data-value="!">!</button>
      
      <button class="num" data-value="7">7</button>
      <button class="num" data-value="8">8</button>
      <button class="num" data-value="9">9</button>
      <button class="op" data-value="/">÷</button>
      <button class="op" data-value="π">π</button>
      
      <button class="num" data-value="4">4</button>
      <button class="num" data-value="5">5</button>
      <button class="num" data-value="6">6</button>
      <button class="op" data-value="*">×</button>
      <button class="op" data-value="e">e</button>
      
      <button class="num" data-value="1">1</button>
      <button class="num" data-value="2">2</button>
      <button class="num" data-value="3">3</button>
      <button class="op" data-value="-">−</button>
      <button class="op" data-value=".">.</button>
      
      <button class="num" data-value="0">0</button>
      <button class="equals" data-value="=">=</button>
      <button class="op" data-value="+">+</button>
    </div>
  </div>
  <script>
    let currentInput = '0';
    let history = '';
    let memory = 0;
    const display = document.getElementById('display');
    const historyDisplay = document.getElementById('history');

    document.querySelectorAll('button').forEach(button => {
      button.addEventListener('click', () => {
        const value = button.getAttribute('data-value');
        if (button.classList.contains('num')) handleNumber(value);
        else if (button.classList.contains('op')) handleOperator(value);
        else if (button.classList.contains('func')) handleFunction(value);
        else if (button.classList.contains('equals')) calculate();
        updateDisplay();
      });
    });

    function handleNumber(num) {
      if (currentInput === '0' || currentInput === 'Error') currentInput = num;
      else currentInput += num;
    }

    function handleOperator(op) {
      const lastChar = currentInput.slice(-1);
      const operators = ['+', '-', '*', '/', '^'];
      if (op === 'π') currentInput += Math.PI;
      else if (op === 'e') currentInput += Math.E;
      else if (op === '√') currentInput = `Math.sqrt(${currentInput})`;
      else if (operators.includes(lastChar) && operators.includes(op)) {
        currentInput = currentInput.slice(0, -1) + op;
      } else currentInput += op;
    }

    function handleFunction(func) {
      switch(func) {
        case 'ac': currentInput = '0'; history = ''; break;
        case 'sin': currentInput = `Math.sin(${currentInput})`; break;
        case 'cos': currentInput = `Math.cos(${currentInput})`; break;
        case 'tan': currentInput = `Math.tan(${currentInput})`; break;
        case 'log': currentInput = `Math.log10(${currentInput})`; break;
        case 'ln': currentInput = `Math.log(${currentInput})`; break;
        case '!': currentInput = factorial(currentInput); break;
        case 'm+': memory += parseFloat(currentInput) || 0; break;
        case 'm-': memory -= parseFloat(currentInput) || 0; break;
        case 'mr': currentInput = memory.toString(); break;
        case 'mc': memory = 0;
      }
    }

    function factorial(n) {
      n = parseInt(n);
      if (n < 0) return 'Error';
      let result = 1;
      for (let i = 2; i <= n; i++) result *= i;
      return result;
    }

    function calculate() {
      try {
        let expression = currentInput
          .replace(/×/g, '*')
          .replace(/÷/g, '/')
          .replace(/π/g, Math.PI)
          .replace(/e/g, Math.E);
        history = currentInput;
        currentInput = eval(expression).toString();
      } catch (error) {
        currentInput = 'Error';
      }
    }

    function updateDisplay() {
      display.textContent = currentInput;
      historyDisplay.textContent = history;
    }
  </script>
</body>
</html>