<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora Juguetona</title>
    <!-- Usamos una fuente divertida de Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;600;700&display=swap" rel="stylesheet">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: 'Fredoka', sans-serif;
            margin: 0;
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            /* Fondo animado vibrante */
            background: linear-gradient(-45deg, #ff9a9e, #fecfef, #a1c4fd, #c2e9fb);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
            overflow: hidden;
        }

        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* Estilo de Juguete para la Calculadora */
        .toy-calc {
            background: white;
            border-radius: 40px;
            box-shadow: 0 20px 0 #e2e8f0, 0 30px 40px rgba(0,0,0,0.2);
            border: 8px solid white;
            transition: transform 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }
        .toy-calc:hover {
            transform: translateY(-5px);
        }

        /* Pantalla de la calculadora */
        .screen-container {
            background: #1e293b;
            border-radius: 25px;
            box-shadow: inset 0 10px 20px rgba(0,0,0,0.5);
            border: 6px solid #cbd5e1;
            position: relative;
            overflow: hidden;
        }

        /* Botones estilo Teclas Mecánicas Gruesas */
        .btn-toy {
            position: relative;
            background: #f8fafc;
            border-radius: 20px;
            font-size: 1.75rem;
            font-weight: 700;
            color: #334155;
            box-shadow: 0 8px 0 #cbd5e1, 0 15px 10px rgba(0,0,0,0.1);
            transition: all 0.1s;
            user-select: none;
            display: flex;
            align-items: center;
            justify-content: center;
            height: 70px;
            cursor: pointer;
        }
        
        .btn-toy:active {
            transform: translateY(8px);
            box-shadow: 0 0px 0 #cbd5e1, 0 5px 5px rgba(0,0,0,0.1);
        }

        /* Colores especiales para botones */
        .btn-op {
            background: #ffb703;
            color: white;
            box-shadow: 0 8px 0 #fb8500, 0 15px 10px rgba(0,0,0,0.1);
        }
        .btn-op:active {
            box-shadow: 0 0px 0 #fb8500, 0 5px 5px rgba(0,0,0,0.1);
        }

        .btn-eq {
            background: #fb8500;
            color: white;
            box-shadow: 0 8px 0 #e85d04, 0 15px 10px rgba(0,0,0,0.1);
        }
        .btn-eq:active {
            box-shadow: 0 0px 0 #e85d04, 0 5px 5px rgba(0,0,0,0.1);
        }

        .btn-clear {
            background: #ef476f;
            color: white;
            box-shadow: 0 8px 0 #c1121f, 0 15px 10px rgba(0,0,0,0.1);
        }
        .btn-clear:active {
            box-shadow: 0 0px 0 #c1121f, 0 5px 5px rgba(0,0,0,0.1);
        }

        /* Animación para los números al aparecer */
        .pop-in {
            display: inline-block;
            animation: popIn 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275) forwards;
        }

        @keyframes popIn {
            0% { transform: scale(0.5) translateY(20px); opacity: 0; }
            100% { transform: scale(1) translateY(0); opacity: 1; }
        }

        /* Panel de Historial */
        .history-panel {
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(10px);
            border-radius: 30px;
            border: 4px dashed #fb8500;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            max-height: 500px;
        }

        /* Scrollbar personalizado para el historial */
        .custom-scroll::-webkit-scrollbar { width: 8px; }
        .custom-scroll::-webkit-scrollbar-track { background: #f1f1f1; border-radius: 10px; }
        .custom-scroll::-webkit-scrollbar-thumb { background: #ffb703; border-radius: 10px; }
        .custom-scroll::-webkit-scrollbar-thumb:hover { background: #fb8500; }

        /* Confeti */
        .confetti {
            position: absolute;
            width: 10px;
            height: 10px;
            border-radius: 50%;
            pointer-events: none;
            z-index: 50;
        }
    </style>
</head>
<body class="p-4 md:p-8">

    <div class="flex flex-col lg:flex-row gap-8 items-start w-full max-w-5xl mx-auto z-10">
        
        <!-- Calculadora Principal -->
        <div class="toy-calc w-full max-w-[380px] p-6 mx-auto flex-shrink-0 relative">
            
            <!-- Adorno superior -->
            <div class="absolute -top-6 left-1/2 -translate-x-1/2 bg-white px-6 py-2 rounded-full font-bold text-gray-400 text-sm shadow-md border-b-4 border-gray-200 uppercase tracking-widest">
                Math Play
            </div>

            <!-- Pantalla -->
            <div class="screen-container p-4 mb-8 h-32 flex flex-col justify-between mt-2">
                <div id="equation" class="text-right text-cyan-300 font-semibold h-6 text-sm tracking-wider opacity-80 truncate"></div>
                <div id="display" class="text-right text-white font-bold text-5xl truncate tracking-wide flex justify-end gap-1">
                    <span class="pop-in">0</span>
                </div>
            </div>

            <!-- Teclado -->
            <div class="grid grid-cols-4 gap-x-4 gap-y-6">
                <!-- Fila 1 -->
                <button onclick="clearAll()" class="btn-toy btn-clear col-span-2">AC</button>
                <button onclick="deleteLast()" class="btn-toy text-2xl">🔙</button>
                <button onclick="setOp('/')" class="btn-toy btn-op text-3xl">÷</button>
                
                <!-- Fila 2 -->
                <button onclick="addNum('7')" class="btn-toy">7</button>
                <button onclick="addNum('8')" class="btn-toy">8</button>
                <button onclick="addNum('9')" class="btn-toy">9</button>
                <button onclick="setOp('*')" class="btn-toy btn-op text-3xl">×</button>
                
                <!-- Fila 3 -->
                <button onclick="addNum('4')" class="btn-toy">4</button>
                <button onclick="addNum('5')" class="btn-toy">5</button>
                <button onclick="addNum('6')" class="btn-toy">6</button>
                <button onclick="setOp('-')" class="btn-toy btn-op text-3xl">-</button>
                
                <!-- Fila 4 -->
                <button onclick="addNum('1')" class="btn-toy">1</button>
                <button onclick="addNum('2')" class="btn-toy">2</button>
                <button onclick="addNum('3')" class="btn-toy">3</button>
                <button onclick="setOp('+')" class="btn-toy btn-op text-3xl">+</button>
                
                <!-- Fila 5 -->
                <button onclick="addNum('.')" class="btn-toy text-4xl pb-4">.</button>
                <button onclick="addNum('0')" class="btn-toy">0</button>
                <button onclick="calculate()" class="btn-toy btn-eq col-span-2 text-3xl">=</button>
            </div>
        </div>

        <!-- Panel de Historial -->
        <div class="history-panel w-full lg:w-80 p-6 flex flex-col mx-auto h-[550px]">
            <div class="flex justify-between items-center mb-4 border-b-2 border-dashed border-gray-300 pb-2">
                <h3 class="text-xl font-bold text-slate-700 flex items-center gap-2">
                    <span>📜</span> Historial
                </h3>
                <button onclick="clearHistory()" class="text-xs bg-slate-200 hover:bg-slate-300 text-slate-600 px-3 py-1 rounded-full transition-colors font-bold">
                    Limpiar
                </button>
            </div>
            
            <div id="history-list" class="flex-1 overflow-y-auto custom-scroll space-y-3 pr-2">
                <!-- Los items del historial se insertan aquí -->
                <div class="text-center text-slate-400 mt-10 italic font-medium">
                    ¡Haz un cálculo para empezar la diversión! ✨
                </div>
            </div>
        </div>

    </div>

    <script>
        const display = document.getElementById('display');
        const equation = document.getElementById('equation');
        const historyList = document.getElementById('history-list');
        
        let currentNum = '0';
        let previousNum = '';
        let operation = null;
        let shouldResetDisplay = false;
        let historyData = [];

        // --- MANEJO DE NÚMEROS Y PANTALLA ---
        
        // Función para animar el número al entrar
        function renderDisplay(value) {
            // Dividimos el valor en caracteres y los metemos en spans para animarlos
            display.innerHTML = '';
            const chars = value.toString().split('');
            chars.forEach((char, index) => {
                const span = document.createElement('span');
                span.innerText = char;
                span.className = 'pop-in';
                // Pequeño retraso secuencial para un efecto de "ola"
                span.style.animationDelay = `${index * 0.03}s`;
                display.appendChild(span);
            });
        }

        function addNum(num) {
            if (currentNum === '0' || shouldResetDisplay) {
                currentNum = num === '.' ? '0.' : num;
                shouldResetDisplay = false;
            } else {
                if (num === '.' && currentNum.includes('.')) return; // Evitar multiples puntos
                if (currentNum.length > 12) return; // Límite de caracteres
                currentNum += num;
            }
            renderDisplay(currentNum);
        }

        function setOp(op) {
            if (operation !== null) calculate(false); // Falso indica que no lance confeti al encadenar
            previousNum = currentNum;
            operation = op;
            equation.innerText = `${previousNum} ${getOpSymbol(op)}`;
            shouldResetDisplay = true;
        }

        function getOpSymbol(op) {
            if (op === '*') return '×';
            if (op === '/') return '÷';
            return op;
        }

        function deleteLast() {
            if (shouldResetDisplay) return;
            currentNum = currentNum.length > 1 ? currentNum.slice(0, -1) : '0';
            renderDisplay(currentNum);
        }

        function clearAll() {
            currentNum = '0';
            previousNum = '';
            operation = null;
            equation.innerText = '';
            renderDisplay('0');
        }

        // --- CÁLCULO Y LÓGICA ---

        function calculate(celebrate = true) {
            if (operation === null || shouldResetDisplay) return;

            const a = parseFloat(previousNum);
            const b = parseFloat(currentNum);
            let result;

            switch (operation) {
                case '+': result = a + b; break;
                case '-': result = a - b; break;
                case '*': result = a * b; break;
                case '/': 
                    if (b === 0) {
                        display.innerHTML = '<span class="text-rose-400 pop-in">Error</span>';
                        setTimeout(clearAll, 1500);
                        return;
                    }
                    result = a / b; 
                    break;
            }

            // Redondear para evitar problemas de coma flotante largos
            result = Math.round(result * 100000000) / 100000000;
            
            const eqString = `${a} ${getOpSymbol(operation)} ${b}`;
            equation.innerText = `${eqString} =`;
            currentNum = result.toString();
            operation = null;
            shouldResetDisplay = true;
            
            renderDisplay(currentNum);
            addToHistory(eqString, currentNum);

            // Efecto divertido al dar igual
            if (celebrate) triggerConfetti();
        }

        // --- HISTORIAL ---

        function addToHistory(eq, res) {
            historyData.unshift({ equation: eq, result: res }); // Añadir al principio
            renderHistory();
        }

        function renderHistory() {
            historyList.innerHTML = '';
            if (historyData.length === 0) {
                historyList.innerHTML = '<div class="text-center text-slate-400 mt-10 italic font-medium">¡Haz un cálculo para empezar la diversión! ✨</div>';
                return;
            }

            historyData.forEach((item, index) => {
                const div = document.createElement('div');
                // Animación de entrada para el nuevo item del historial
                div.className = `p-3 bg-white rounded-2xl shadow-sm border border-slate-100 flex flex-col items-end gap-1 hover:bg-orange-50 transition-colors cursor-pointer pop-in`;
                div.style.animationDelay = `${index * 0.05}s`;
                
                div.innerHTML = `
                    <span class="text-xs text-slate-400 font-semibold">${item.equation} =</span>
                    <span class="text-xl font-bold text-slate-700">${item.result}</span>
                `;
                
                // Permitir recuperar resultados del historial
                div.onclick = () => {
                    currentNum = item.result;
                    shouldResetDisplay = true;
                    renderDisplay(currentNum);
                };

                historyList.appendChild(div);
            });
        }

        function clearHistory() {
            historyData = [];
            renderHistory();
        }

        // --- EFECTOS VISUALES (CONFETI) ---

        function triggerConfetti() {
            const colors = ['#ffb703', '#fb8500', '#ef476f', '#06d6a0', '#118ab2'];
            const container = document.querySelector('.toy-calc');
            const rect = container.getBoundingClientRect();

            for (let i = 0; i < 40; i++) {
                createParticle(rect.left + rect.width / 2, rect.top + rect.height / 2, colors);
            }
        }

        function createParticle(x, y, colors) {
            const particle = document.createElement('div');
            particle.className = 'confetti';
            
            // Atributos aleatorios
            const color = colors[Math.floor(Math.random() * colors.length)];
            const size = Math.random() * 8 + 6;
            const angle = Math.random() * Math.PI * 2;
            const velocity = 50 + Math.random() * 100;
            const tx = Math.cos(angle) * velocity;
            const ty = Math.sin(angle) * velocity - 100; // Tendencia hacia arriba
            const rot = Math.random() * 360;

            particle.style.backgroundColor = color;
            particle.style.width = `${size}px`;
            particle.style.height = `${size}px`;
            particle.style.left = `${x}px`;
            particle.style.top = `${y}px`;
            
            document.body.appendChild(particle);

            // Animar con Web Animations API
            const animation = particle.animate([
                { transform: `translate(0, 0) rotate(0deg)`, opacity: 1 },
                { transform: `translate(${tx}px, ${ty}px) rotate(${rot}deg)`, opacity: 1, offset: 0.8 },
                { transform: `translate(${tx}px, ${ty + 50}px) rotate(${rot}deg)`, opacity: 0 }
            ], {
                duration: 800 + Math.random() * 500,
                easing: 'cubic-bezier(0.25, 1, 0.5, 1)'
            });

            animation.onfinish = () => particle.remove();
        }

        // --- SOPORTE TECLADO FÍSICO ---
        document.addEventListener('keydown', (e) => {
            if (e.key >= '0' && e.key <= '9') addNum(e.key);
            if (e.key === '.') addNum('.');
            if (e.key === 'Enter' || e.key === '=') {
                e.preventDefault();
                calculate();
            }
            if (e.key === 'Backspace') deleteLast();
            if (e.key === 'Escape') clearAll();
            if (['+', '-', '*', '/'].includes(e.key)) setOp(e.key);
        });

    </script>
</body>
</html>
