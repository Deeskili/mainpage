---
toc: false
comments: false
layout: post
title: Game of Life
description: A remix of Conway's game of life using timer, onclick and algorithms.
type: hacks
courses: { compsci: {week: 2} }
---


<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Game of Life</title>
    <style>
        #container {
            display: grid;
            gap: 1px;
        }

        .cell {
            width: 15px;
            height: 15px;
            background-color: royalblue;
            border: 1px solid black;
        }
    </style>
</head>
<body>
    <div class="container">
        <header class="pb-3 mb-4 border-bottom border-primary text-dark">
            <span class="fs-4">Remix of Game of Life</span>
        </header>
        <button onclick="start()" id="start-btn">start</button>
        <button onclick="step()">step</button>
        <div id="container" class="container py-4"></div>
    </div>
    <script>
        let GRID_SIZE = 40;
        let CELL_SIZE = "15px";
        let container = document.getElementById("container");
        container.style.gridTemplateColumns = `repeat(${GRID_SIZE}, ${CELL_SIZE})`;

        for (let i = 0; i < GRID_SIZE * GRID_SIZE; i++) {
            let div = document.createElement('div');
            div.style.width = CELL_SIZE;
            div.style.height = CELL_SIZE;
            div.onclick = clicked;
            div.ondragstart = dragged;
            div.className = 'cell';
            div.id = 'cell-' + i;
            container.appendChild(div);
        }

        const CELLS = Array(GRID_SIZE).fill().map(() => Array(GRID_SIZE).fill(0));

        function safeindex(x, y) {
            return !(x < 0 || x >= GRID_SIZE || y < 0 || y >= GRID_SIZE);
        }

        function safeGet(x, y) {
            if (!safeindex(x, y)) return 0;
            return CELLS[y][x];
        }

        function setCell(n, v) {
            let row = Math.floor(n / GRID_SIZE);
            let col = n % GRID_SIZE;
            CELLS[row][col] = v;
        }

        function toggleCell(n) {
            let row = Math.floor(n / GRID_SIZE);
            let col = n % GRID_SIZE;
            CELLS[row][col] = CELLS[row][col] === 0 ? 1 : 0;
        }

        function updateContainer() {
            CELLS.forEach((arr, r) => {
                arr.forEach((val, c) => {
                    let n = r * GRID_SIZE + c;
                    document.getElementById("cell-" + n).style.backgroundColor = val === 1 ? 'yellow' : 'royalblue';
                });
            });
        }

        function clicked() {
            const id = parseInt(this.id.substring(5), 10);
            toggleCell(id);
            updateContainer();
        }

        function dragged() {
            const id = parseInt(this.id.substring(5), 10);
            setCell(id, 1);
            updateContainer();
        }

        // ... (rest of your code)
    </script>
</body>
</html>
