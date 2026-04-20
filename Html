<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Block Dash Legendary - Balão Edition</title>
    <style>
        body { margin: 0; overflow: hidden; background-color: #050505; touch-action: none; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
        canvas { display: block; }
        #ui { position: absolute; top: 20px; width: 100%; text-align: center; color: #00ffff; font-size: 28px; font-weight: bold; pointer-events: none; text-shadow: 0 0 15px #00ffff; }
        #reviveBtn { display: none; position: absolute; top: 60%; left: 50%; transform: translate(-50%, -50%); padding: 20px 40px; font-size: 22px; background: #ff0055; color: #fff; border: none; border-radius: 50px; cursor: pointer; box-shadow: 0 0 30px #ff0055; font-weight: bold; }
    </style>
</head>
<body>
    <div id="ui">ONDA: <span id="waveCount">0</span> | MELHOR: <span id="bestWave">0</span></div>
    <button id="reviveBtn" onclick="revive()">REVIVER ⚡</button>
    <canvas id="gameCanvas"></canvas>

<script>
    const canvas = document.getElementById('gameCanvas');
    const ctx = canvas.getContext('2d');
    const waveElement = document.getElementById('waveCount');
    const bestElement = document.getElementById('bestWave');
    const reviveBtn = document.getElementById('reviveBtn');

    canvas.width = window.innerWidth;
    canvas.height = window.innerHeight;

    let waves = 0;
    let highScore = localStorage.getItem("blockDashWaveRecord") || 0;
    bestElement.innerText = highScore;

    let gameActive = true;
    let gameSpeed = 6;
    let frameCount = 0;
    let canRevive = true;

    const player = { x: canvas.width / 2, y: canvas.height * 0.8, width: 35, height: 35, targetX: canvas.width / 2 };
    let obstacles = [];

    const move = (e) => {
        let x = e.touches ? e.touches[0].clientX : e.clientX;
        player.targetX = x - player.width / 2;
    };
    window.addEventListener('mousemove', move);
    window.addEventListener('touchstart', move);
    window.addEventListener('touchmove', move);

    function createWall() {
        const gapWidth = 110; 
        const gapX = Math.random() * (canvas.width - gapWidth);
        obstacles.push({ x: 0, y: -60, width: gapX, height: 40, passed: false });
        obstacles.push({ x: gapX + gapWidth, y: -60, width: canvas.width - (gapX + gapWidth), height: 40, passed: false });
    }

    function update() {
        if (!gameActive) return;
        player.x += (player.targetX - player.x) * 0.25;

        frameCount++;
        if (frameCount % Math.max(35, 90 - (waves * 2)) === 0) createWall();

        obstacles.forEach((obs, i) => {
            obs.y += gameSpeed;

            if (player.
