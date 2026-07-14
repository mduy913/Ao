<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🌍 Thế giới AI 3D</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #0a0e17;
            color: #c8d6e5;
            overflow: hidden;
            height: 100vh;
        }

        #app {
            display: flex;
            flex-direction: column;
            height: 100vh;
        }

        #header {
            background: rgba(20, 28, 43, 0.9);
            padding: 10px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid rgba(30, 42, 58, 0.5);
            flex-shrink: 0;
            flex-wrap: wrap;
            gap: 8px;
            backdrop-filter: blur(10px);
            z-index: 10;
            position: relative;
        }

        .logo {
            font-size: 20px;
            font-weight: 700;
            color: #48dbfb;
            text-shadow: 0 0 20px rgba(72, 219, 251, 0.3);
        }

        #stats {
            display: flex;
            gap: 16px;
            font-size: 13px;
            flex-wrap: wrap;
        }

        #stats span {
            background: rgba(13, 20, 33, 0.8);
            padding: 4px 12px;
            border-radius: 12px;
            white-space: nowrap;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }

        #controls {
            display: flex;
            gap: 6px;
            flex-wrap: wrap;
        }

        #controls button {
            background: rgba(30, 42, 58, 0.8);
            border: 1px solid rgba(255, 255, 255, 0.05);
            color: #c8d6e5;
            padding: 4px 12px;
            border-radius: 8px;
            cursor: pointer;
            font-size: 12px;
            transition: 0.3s;
            backdrop-filter: blur(5px);
        }

        #controls button:hover {
            background: #48dbfb;
            color: #0a0e17;
            border-color: #48dbfb;
        }

        #controls button.active {
            background: #48dbfb;
            color: #0a0e17;
            border-color: #48dbfb;
        }

        #controls button.danger {
            background: rgba(255, 107, 107, 0.3);
            color: #ff6b6b;
            border-color: rgba(255, 107, 107, 0.3);
        }

        #controls button.danger:hover {
            background: #ff6b6b;
            color: #0a0e17;
            border-color: #ff6b6b;
        }

        #world-container {
            flex: 1;
            position: relative;
            overflow: hidden;
        }

        #world-container canvas {
            display: block;
            width: 100% !important;
            height: 100% !important;
        }

        #info-panel {
            position: absolute;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            background: rgba(20, 28, 43, 0.85);
            padding: 8px 16px;
            border-radius: 12px;
            font-size: 12px;
            color: #8395a7;
            border: 1px solid rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            pointer-events: none;
            white-space: nowrap;
        }

        /* Modal */
        #npc-modal {
            display: none;
            position: fixed;
            z-index: 1000;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.7);
            justify-content: center;
            align-items: center;
            animation: fadeIn 0.3s ease;
            backdrop-filter: blur(5px);
        }

        #npc-modal.show {
            display: flex;
        }

        @keyframes fadeIn {
            0% {
                opacity: 0;
                transform: scale(0.9);
            }
            100% {
                opacity: 1;
                transform: scale(1);
            }
        }

        .modal-content {
            background: #141c2b;
            padding: 28px;
            border-radius: 16px;
            max-width: 450px;
            width: 90%;
            max-height: 80vh;
            overflow-y: auto;
            border: 1px solid #1e2a3a;
            position: relative;
        }

        .close-btn {
            position: absolute;
            top: 12px;
            right: 16px;
            font-size: 24px;
            cursor: pointer;
            color: #8395a7;
            transition: 0.3s;
            background: none;
            border: none;
        }

        .close-btn:hover {
            color: #ff6b6b;
            transform: rotate(90deg);
        }

        #npc-info .field {
            display: flex;
            justify-content: space-between;
            padding: 5px 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.04);
            font-size: 13px;
        }

        #npc-info .field .label {
            color: #8395a7;
        }

        #npc-info .field .value {
            color: #ecf0f1;
        }

        #npc-info .field .value.highlight {
            color: #48dbfb;
            font-weight: 600;
        }

        .modal-title {
            color: #48dbfb;
            font-size: 20px;
            margin-bottom: 12px;
            padding-right: 30px;
        }

        /* Responsive */
        @media (max-width: 768px) {
            #stats {
                font-size: 11px;
                gap: 8px;
            }

            #stats span {
                padding: 2px 8px;
            }

            .logo {
                font-size: 16px;
            }

            #controls button {
                font-size: 10px;
                padding: 3px 8px;
            }

            #info-panel {
                font-size: 10px;
                padding: 4px 12px;
                bottom: 10px;
            }
        }

        @media (max-width: 480px) {
            #header {
                flex-direction: column;
                align-items: stretch;
                gap: 4px;
                padding: 8px;
            }

            #stats {
                justify-content: center;
            }

            #controls {
                justify-content: center;
            }

            #info-panel {
                display: none;
            }
        }
    </style>
</head>
<body>

    <div id="app">
        <div id="header">
            <div class="logo">🌍 Thế giới AI 3D</div>
            <div id="stats">
                <span id="time-display">⏰ Đang tải...</span>
                <span id="weather-display">🌤️ --°C</span>
                <span id="npc-count">👥 0</span>
                <span id="fps-display">⚡ 0 FPS</span>
            </div>
            <div id="controls">
                <button onclick="togglePause()" id="pause-btn">⏸️ Tạm dừng</button>
                <button onclick="setSpeed(0.5)">🐢 0.5x</button>
                <button onclick="setSpeed(1)" class="active" id="speed-1">▶️ 1x</button>
                <button onclick="setSpeed(2)">🐇 2x</button>
                <button onclick="setSpeed(5)">🚀 5x</button>
                <button onclick="addRandomNPC()" class="danger">➕ NPC</button>
                <button onclick="toggleCamera()">🎥 Cam</button>
            </div>
        </div>

        <div id="world-container">
            <div id="info-panel">🖱️ Click NPC → Xem thông tin | 🔄 Scroll → Zoom | 🖱️ Kéo → Xoay</div>
        </div>

        <!-- Modal -->
        <div id="npc-modal" onclick="if(event.target===this)closeModal()">
            <div class="modal-content">
                <button class="close-btn" onclick="closeModal()">&times;</button>
                <div id="npc-info"></div>
            </div>
        </div>
    </div>

    <script type="importmap">
        {
            "imports": {
                "three": "https://cdn.jsdelivr.net/npm/three@0.160.0/build/three.module.js",
                "three/addons/": "https://cdn.jsdelivr.net/npm/three@0.160.0/examples/jsm/"
            }
        }
    </script>

    <script type="module">
        import * as THREE from 'three';
        import { OrbitControls } from 'three/addons/controls/OrbitControls.js';
        import { CSS2DRenderer, CSS2DObject } from 'three/addons/renderers/CSS2DRenderer.js';

        // ============================================================
        // WORLD STATE
        // ============================================================
        const world = {
            npcs: [],
            hours: 6,
            days: 0,
            months: 0,
            years: 0,
            weather: '☀️ Nắng',
            temperature: 25,
            isPaused: false,
            speed: 1,
            tickCount: 0,
            npcIdCounter: 0,
            worldSize: 200
        };

        // ============================================================
        // THREE.JS SETUP
        // ============================================================
        const container = document.getElementById('world-container');
        const width = container.clientWidth;
        const height = container.clientHeight;

        // Scene
        const scene = new THREE.Scene();
        scene.background = new THREE.Color(0x0a0e17);
        scene.fog = new THREE.Fog(0x0a0e17, 150, 300);

        // Camera
        const camera = new THREE.PerspectiveCamera(60, width / height, 0.1, 1000);
        camera.position.set(80, 60, 80);
        camera.lookAt(0, 0, 0);

        // Renderer
        const renderer = new THREE.WebGLRenderer({
            antialias: true,
            alpha: true
        });
        renderer.setSize(width, height);
        renderer.setPixelRatio(Math.min(window.devicePixelRatio, 2));
        renderer.shadowMap.enabled = true;
        renderer.shadowMap.type = THREE.PCFSoftShadowMap;
        renderer.toneMapping = THREE.ACESFilmicToneMapping;
        renderer.toneMappingExposure = 1.2;
        container.appendChild(renderer.domElement);

        // CSS2D Renderer for labels
        const labelRenderer = new CSS2DRenderer();
        labelRenderer.setSize(width, height);
        labelRenderer.domElement.style.position = 'absolute';
        labelRenderer.domElement.style.top = '0';
        labelRenderer.domElement.style.left = '0';
        labelRenderer.domElement.style.pointerEvents = 'none';
        container.appendChild(labelRenderer.domElement);

        // Controls
        const controls = new OrbitControls(camera, renderer.domElement);
        controls.enableDamping = true;
        controls.dampingFactor = 0.05;
        controls.maxPolarAngle = Math.PI / 2.1;
        controls.minDistance = 10;
        controls.maxDistance = 300;
        controls.target.set(0, 0, 0);
        controls.update();

        // ============================================================
        // LIGHTING
        // ============================================================
        // Ambient light
        const ambientLight = new THREE.AmbientLight(0x404060, 0.4);
        scene.add(ambientLight);

        // Sunlight
        const sunLight = new THREE.DirectionalLight(0xffeedd, 1.5);
        sunLight.position.set(50, 80, 30);
        sunLight.castShadow = true;
        sunLight.shadow.mapSize.width = 2048;
        sunLight.shadow.mapSize.height = 2048;
        sunLight.shadow.camera.near = 0.1;
        sunLight.shadow.camera.far = 300;
        sunLight.shadow.camera.left = -150;
        sunLight.shadow.camera.right = 150;
        sunLight.shadow.camera.top = 150;
        sunLight.shadow.camera.bottom = -150;
        scene.add(sunLight);

        // Fill light
        const fillLight = new THREE.DirectionalLight(0x8888ff, 0.3);
        fillLight.position.set(-30, 20, -30);
        scene.add(fillLight);

        // Hemisphere light
        const hemiLight = new THREE.HemisphereLight(0x87ceeb, 0x3a1c00, 0.6);
        scene.add(hemiLight);

        // ============================================================
        // GROUND
        // ============================================================
        const groundGeometry = new THREE.PlaneGeometry(400, 400);
        const groundMaterial = new THREE.MeshStandardMaterial({
            color: 0x1a1a2e,
            roughness: 0.9,
            metalness: 0.0,
        });
        const ground = new THREE.Mesh(groundGeometry, groundMaterial);
        ground.rotation.x = -Math.PI / 2;
        ground.receiveShadow = true;
        scene.add(ground);

        // Grid
        const gridHelper = new THREE.GridHelper(400, 40, 0x2a2a4e, 0x1a1a3e);
        gridHelper.position.y = 0.1;
        scene.add(gridHelper);

        // ============================================================
        // DECORATIONS
        // ============================================================
        // Trees
        function createTree(x, z) {
            const group = new THREE.Group();

            // Trunk
            const trunkGeo = new THREE.CylinderGeometry(0.3, 0.5, 2, 6);
            const trunkMat = new THREE.MeshStandardMaterial({ color: 0x4a3728, roughness: 0.9 });
            const trunk = new THREE.Mesh(trunkGeo, trunkMat);
            trunk.position.y = 1;
            trunk.castShadow = true;
            group.add(trunk);

            // Leaves
            const leafMat = new THREE.MeshStandardMaterial({
                color: new THREE.Color().setHSL(0.3 + Math.random() * 0.1, 0.6, 0.3 + Math.random() * 0.2),
                roughness: 0.8
            });
            for (let i = 0; i < 3; i++) {
                const size = 1.5 - i * 0.3;
                const leaf = new THREE.Mesh(
                    new THREE.SphereGeometry(size, 6, 6),
                    leafMat
                );
                leaf.position.y = 2.5 + i * 0.8;
                leaf.position.x = (Math.random() - 0.5) * 0.5;
                leaf.position.z = (Math.random() - 0.5) * 0.5;
                leaf.castShadow = true;
                group.add(leaf);
            }

            group.position.set(x, 0, z);
            const scale = 0.8 + Math.random() * 0.6;
            group.scale.set(scale, scale, scale);
            group.rotation.y = Math.random() * Math.PI * 2;

            return group;
        }

        // Buildings
        function createBuilding(x, z, color = 0x2a2a4e) {
            const group = new THREE.Group();

            const height = 2 + Math.random() * 4;
            const width = 2 + Math.random() * 3;
            const depth = 2 + Math.random() * 3;

            const box = new THREE.Mesh(
                new THREE.BoxGeometry(width, height, depth),
                new THREE.MeshStandardMaterial({
                    color: color,
                    roughness: 0.7,
                    metalness: 0.1
                })
            );
            box.position.y = height / 2;
            box.castShadow = true;
            box.receiveShadow = true;
            group.add(box);

            // Roof
            const roof = new THREE.Mesh(
                new THREE.ConeGeometry(Math.max(width, depth) * 0.7, 1.5, 4),
                new THREE.MeshStandardMaterial({
                    color: 0x4a2a1a,
                    roughness: 0.9
                })
            );
            roof.position.y = height + 0.75;
            roof.rotation.y = Math.PI / 4;
            roof.castShadow = true;
            group.add(roof);

            group.position.set(x, 0, z);
            group.rotation.y = Math.random() * Math.PI * 2;

            return group;
        }

        // Generate decorations
        function generateDecorations() {
            // Trees
            for (let i = 0; i < 80; i++) {
                const x = (Math.random() - 0.5) * 350;
                const z = (Math.random() - 0.5) * 350;
                if (Math.abs(x) < 20 && Math.abs(z) < 20) continue;
                const tree = createTree(x, z);
                scene.add(tree);
            }

            // Buildings
            const buildingColors = [0x2a2a4e, 0x3a2a4e, 0x2a3a4e, 0x4a2a3a];
            for (let i = 0; i < 20; i++) {
                const x = (Math.random() - 0.5) * 200;
                const z = (Math.random() - 0.5) * 200;
                if (Math.abs(x) < 30 && Math.abs(z) < 30) continue;
                const color = buildingColors[Math.floor(Math.random() * buildingColors.length)];
                const building = createBuilding(x, z, color);
                scene.add(building);
            }
        }
        generateDecorations();

        // ============================================================
        // NPC SYSTEM
        // ============================================================
        const npcMeshes = new Map();

        function generateName() {
            const first = ['Nguyễn', 'Trần', 'Lê', 'Phạm', 'Hoàng', 'Vũ', 'Đặng', 'Bùi', 'Đỗ', 'Hồ'];
            const middle = ['Văn', 'Thị', 'Đức', 'Minh', 'Hữu', 'Kim', 'Xuân', 'Hải', 'Quang', 'Ngọc'];
            const last = ['An', 'Bình', 'Cường', 'Dung', 'Hạnh', 'Huy', 'Lan', 'Mai', 'Nam', 'Phúc'];
            return `${first[Math.floor(Math.random()*first.length)]} ${middle[Math.floor(Math.random()*middle.length)]} ${last[Math.floor(Math.random()*last.length)]}`;
        }

        function createNPC(name) {
            const id = ++world.npcIdCounter;
            const npc = {
                id: id,
                name: name || generateName(),
                gender: Math.random() > 0.5 ? 'Nam' : 'Nữ',
                age: 18 + Math.floor(Math.random() * 42),
                profession: ['Nông dân', 'Công nhân', 'Giáo viên', 'Bác sĩ', 'Kỹ sư',
                    'Thương nhân', 'Nghệ sĩ', 'Chiến binh', 'Nhà khoa học'
                ][Math.floor(Math.random() * 9)],
                position: {
                    x: (Math.random() - 0.5) * 160,
                    z: (Math.random() - 0.5) * 160
                },
                targetX: 0,
                targetZ: 0,
                emotion: ['Vui vẻ', 'Bình thường', 'Tức giận', 'Sợ hãi', 'Mệt mỏi', 'Cô đơn', 'Lo lắng'][
                    Math.floor(Math.random() * 7)
                ],
                health: 70 + Math.random() * 30,
                energy: 50 + Math.random() * 50,
                hunger: 30 + Math.random() * 40,
                thirst: 30 + Math.random() * 40,
                money: 100 + Math.random() * 4900,
                isAlive: true,
                speed: 0.3 + Math.random() * 0.4,
                action: 'Đứng yên',
                actionTimer: 0
            };

            // Random target
            npc.targetX = (Math.random() - 0.5) * 160;
            npc.targetZ = (Math.random() - 0.5) * 160;

            // Create 3D mesh
            const color = new THREE.Color().setHSL(0.6 + Math.random() * 0.3, 0.7, 0.5);
            const group = new THREE.Group();

            // Body
            const bodyGeo = new THREE.SphereGeometry(0.8, 8, 8);
            const bodyMat = new THREE.MeshStandardMaterial({ color: color, roughness: 0.6, metalness: 0.1 });
            const body = new THREE.Mesh(bodyGeo, bodyMat);
            body.position.y = 1.2;
            body.castShadow = true;
            group.add(body);

            // Head
            const headGeo = new THREE.SphereGeometry(0.5, 8, 8);
            const headMat = new THREE.MeshStandardMaterial({
                color: new THREE.Color().setHSL(0.08, 0.3, 0.7),
                roughness: 0.8
            });
            const head = new THREE.Mesh(headGeo, headMat);
            head.position.y = 2.0;
            head.castShadow = true;
            group.add(head);

            // Hat
            const hatGeo = new THREE.ConeGeometry(0.7, 0.4, 6);
            const hatMat = new THREE.MeshStandardMaterial({
                color: new THREE.Color().setHSL(0.6 + Math.random() * 0.2, 0.8, 0.3),
                roughness: 0.9
            });
            const hat = new THREE.Mesh(hatGeo, hatMat);
            hat.position.y = 2.4;
            group.add(hat);

            // Eyes (two small spheres)
            const eyeMat = new THREE.MeshStandardMaterial({ color: 0xffffff });
            const pupilMat = new THREE.MeshStandardMaterial({ color: 0x222222 });
            for (let side = -1; side <= 1; side += 2) {
                const eye = new THREE.Mesh(new THREE.SphereGeometry(0.1, 6, 6), eyeMat);
                eye.position.set(side * 0.2, 2.05, 0.45);
                group.add(eye);

                const pupil = new THREE.Mesh(new THREE.SphereGeometry(0.05, 6, 6), pupilMat);
                pupil.position.set(side * 0.22, 2.05, 0.5);
                group.add(pupil);
            }

            // Label
            const labelDiv = document.createElement('div');
            labelDiv.textContent = name;
            labelDiv.style.color = '#c8d6e5';
            labelDiv.style.fontSize = '10px';
            labelDiv.style.fontWeight = '600';
            labelDiv.style.textShadow = '0 0 10px rgba(0,0,0,0.8)';
            labelDiv.style.background = 'rgba(0,0,0,0.5)';
            labelDiv.style.padding = '2px 8px';
            labelDiv.style.borderRadius = '10px';
            labelDiv.style.border = '1px solid rgba(255,255,255,0.1)';
            labelDiv.style.backdropFilter = 'blur(4px)';
            labelDiv.style.pointerEvents = 'none';
            labelDiv.style.whiteSpace = 'nowrap';

            const label = new CSS2DObject(labelDiv);
            label.position.set(0, 2.8, 0);
            group.add(label);

            // Store reference
            npc.mesh = group;
            npc.label = label;
            npc.bodyMat = bodyMat;
            npc.headMat = headMat;

            // Position
            group.position.set(npc.position.x, 0, npc.position.z);

            // Add to scene
            scene.add(group);
            npcMeshes.set(id, group);

            return npc;
        }

        function createInitialNPCs(count) {
            for (let i = 0; i < count; i++) {
                const npc = createNPC();
                world.npcs.push(npc);
            }
            updateUI();
        }

        // ============================================================
        // NPC AI
        // ============================================================
        function updateNPC(npc) {
            if (!npc.isAlive) return;

            // Update needs
            npc.hunger += 0.02 * world.speed;
            npc.thirst += 0.02 * world.speed;
            npc.energy -= 0.01 * world.speed;

            // Clamp
            npc.hunger = Math.min(100, npc.hunger);
            npc.thirst = Math.min(100, npc.thirst);
            npc.energy = Math.max(0, npc.energy);

            // Check needs -> action
            if (npc.hunger > 80) {
                npc.action = 'Tìm thức ăn';
                npc.hunger = Math.max(0, npc.hunger - 20);
                npc.emotion = 'Tức giận';
            } else if (npc.thirst > 80) {
                npc.action = 'Tìm nước uống';
                npc.thirst = Math.max(0, npc.thirst - 20);
                npc.emotion = 'Khát';
            } else if (npc.energy < 20) {
                npc.action = 'Nghỉ ngơi';
                npc.energy = Math.min(100, npc.energy + 10);
                npc.emotion = 'Mệt mỏi';
            } else {
                // Random action
                const actions = ['Đi dạo', 'Làm việc', 'Trò chuyện', 'Quan sát', 'Đứng yên'];
                if (npc.actionTimer <= 0) {
                    npc.action = actions[Math.floor(Math.random() * actions.length)];
                    npc.actionTimer = 50 + Math.random() * 100;

                    // Random new target
                    npc.targetX = (Math.random() - 0.5) * 160;
                    npc.targetZ = (Math.random() - 0.5) * 160;

                    // Random emotion
                    const emotions = ['Vui vẻ', 'Bình thường', 'Tò mò', 'Hào hứng', 'Thư thái'];
                    npc.emotion = emotions[Math.floor(Math.random() * emotions.length)];
                }
                npc.actionTimer -= world.speed;
            }

            // Move towards target
            const dx = npc.targetX - npc.position.x;
            const dz = npc.targetZ - npc.position.z;
            const dist = Math.sqrt(dx * dx + dz * dz);

            if (dist > 1) {
                const speed = npc.speed * world.speed * 0.5;
                npc.position.x += (dx / dist) * speed;
                npc.position.z += (dz / dist) * speed;

                // Rotate mesh to face movement direction
                if (npc.mesh) {
                    const angle = Math.atan2(dx, dz);
                    npc.mesh.rotation.y = angle;
                }

                // Bob animation
                if (npc.mesh) {
                    const bob = Math.sin(Date.now() / 500 + npc.id) * 0.05;
                    npc.mesh.position.y = Math.abs(bob);
                }
            }

            // Update mesh position
            if (npc.mesh) {
                npc.mesh.position.x = npc.position.x;
                npc.mesh.position.z = npc.position.z;

                // Update color based on emotion
                const emotionColors = {
                    'Vui vẻ': 0x4ade80,
                    'Bình thường': 0x48dbfb,
                    'Tức giận': 0xff6b6b,
                    'Sợ hãi': 0xfacc15,
                    'Mệt mỏi': 0x8395a7,
                    'Cô đơn': 0xa29bfe,
                    'Lo lắng': 0xfd79a8,
                    'Hào hứng': 0x00d2d3,
                    'Tò mò': 0x0984e3,
                    'Thư thái': 0x00b894,
                    'Khát': 0x4a9eff
                };
                const color = emotionColors[npc.emotion] || 0x48dbfb;
                npc.bodyMat.color.setHex(color);
            }

            // Update label visibility based on distance
            if (npc.label) {
                const distToCam = camera.position.distanceTo(npc.mesh.position);
                npc.label.element.style.display = distToCam < 80 ? 'block' : 'none';
            }
        }

        // ============================================================
        // WORLD UPDATE
        // ============================================================
        function updateWorld() {
            if (world.isPaused) return;

            world.tickCount++;

            // Update time
            if (world.tickCount % 2 === 0) {
                world.hours += 0.5;
                if (world.hours >= 24) {
                    world.hours = 0;
                    world.days++;
                    if (world.days >= 30) {
                        world.days = 0;
                        world.months++;
                        if (world.months >= 12) {
                            world.months = 0;
                            world.years++;
                        }
                    }
                }
            }

            // Update weather
            if (world.tickCount % 60 === 0) {
                const weathers = ['☀️ Nắng', '☁️ Mây', '🌧️ Mưa', '🌤️ Nắng nhẹ', '💨 Gió'];
                world.weather = weathers[Math.floor(Math.random() * weathers.length)];
                world.temperature = 20 + Math.random() * 15;
                updateSceneLighting();
            }

            // Update NPCs
            for (const npc of world.npcs) {
                updateNPC(npc);
            }

            updateUI();
        }

        function updateSceneLighting() {
            // Adjust lighting based on time
            const hour = world.hours;
            const isNight = hour < 5 || hour > 19;
            const intensity = isNight ? 0.2 : 1.0;

            sunLight.intensity = 1.2 * intensity;
            ambientLight.intensity = 0.3 + 0.3 * intensity;

            // Sky color
            const skyColor = isNight ? 0x050510 : 0x0a0e17;
            scene.background = new THREE.Color(skyColor);
            scene.fog = new THREE.Fog(skyColor, 150, 300);
        }

        // ============================================================
        // UI FUNCTIONS
        // ============================================================
        function updateUI() {
            const alive = world.npcs.filter(n => n.isAlive);
            const dead = world.npcs.filter(n => !n.isAlive);

            document.getElementById('time-display').textContent =
                `⏰ ${Math.floor(world.hours)}:00 - Ngày ${world.days+1}/${world.months+1}/${world.years+1}`;

            document.getElementById('weather-display').textContent =
                `${world.weather} ${Math.round(world.temperature)}°C`;

            document.getElementById('npc-count').textContent = `👥 ${alive.length}`;

            document.getElementById('stat-total').textContent = world.npcs.length;
            document.getElementById('stat-alive').textContent = alive.length;
            document.getElementById('stat-dead').textContent = dead.length;

            // Most common profession
            const profs = {};
            for (const n of alive) {
                profs[n.profession] = (profs[n.profession] || 0) + 1;
            }
            let maxProf = '-';
            let maxCount = 0;
            for (const [prof, count] of Object.entries(profs)) {
                if (count > maxCount) { maxCount = count;
                    maxProf = prof; }
            }
            document.getElementById('stat-prof').textContent = maxProf;

            // Most common emotion
            const emos = {};
            for (const n of alive) {
                emos[n.emotion] = (emos[n.emotion] || 0) + 1;
            }
            let maxEmo = '-';
            let maxEmoCount = 0;
            for (const [emo, count] of Object.entries(emos)) {
                if (count > maxEmoCount) { maxEmoCount = count;
                    maxEmo = emo; }
            }
            document.getElementById('stat-emotion').textContent = maxEmo;

            // NPC list
            const list = document.getElementById('npc-list');
            list.innerHTML = '';
            for (const npc of alive.slice(0, 15)) {
                const item = document.createElement('div');
                item.className = 'npc-item';
                const emoClass = {
                    'Vui vẻ': 'happy',
                    'Tức giận': 'angry',
                    'Sợ hãi': 'fear',
                    'Mệt mỏi': 'sad',
                    'Cô đơn': 'sad',
                    'Lo lắng': 'fear'
                } [npc.emotion] || '';
                item.innerHTML = `
                            <span class="name">${npc.name}</span>
                            <span class="emotion-badge ${emoClass}">${npc.emotion}</span>
                        `;
                item.onclick = () => showNPCInfo(npc.id);
                list.appendChild(item);
            }
        }

        // ============================================================
        // NPC INFO
        // ============================================================
        function showNPCInfo(id) {
            const npc = world.npcs.find(n => n.id === id);
            if (!npc) return;

            const modal = document.getElementById('npc-modal');
            const info = document.getElementById('npc-info');

            info.innerHTML = `
                        <div class="modal-title">${npc.name}</div>
                        <div class="field"><span class="label">Giới tính</span><span class="value">${npc.gender}</span></div>
                        <div class="field"><span class="label">Tuổi</span><span class="value">${npc.age}</span></div>
                        <div class="field"><span class="label">Nghề nghiệp</span><span class="value highlight">${npc.profession}</span></div>
                        <div class="field"><span class="label">Cảm xúc</span><span class="value">${npc.emotion}</span></div>
                        <div class="field"><span class="label">Sức khỏe</span><span class="value">${Math.round(npc.health)}%</span></div>
                        <div class="field"><span class="label">Năng lượng</span><span class="value">${Math.round(npc.energy)}%</span></div>
                        <div class="field"><span class="label">Đói</span><span class="value">${Math.round(npc.hunger)}%</span></div>
                        <div class="field"><span class="label">Khát</span><span class="value">${Math.round(npc.thirst)}%</span></div>
                        <div class="field"><span class="label">Tiền</span><span class="value">${Math.round(npc.money).toLocaleString()}đ</span></div>
                        <div class="field"><span class="label">Hành động</span><span class="value highlight">${npc.action}</span></div>
                        <div class="field"><span class="label">Vị trí</span><span class="value">(${Math.round(npc.position.x)}, ${Math.round(npc.position.z)})</span></div>
                    `;

            modal.classList.add('show');
        }

        function closeModal() {
            document.getElementById('npc-modal').classList.remove('show');
        }

        // ============================================================
        // CONTROLS
        // ============================================================
        window.togglePause = function() {
            world.isPaused = !world.isPaused;
            document.getElementById('pause-btn').textContent = world.isPaused ? '▶️ Tiếp tục' : '⏸️ Tạm dừng';
            document.getElementById('pause-btn').classList.toggle('active', world.isPaused);
        };

        window.setSpeed = function(speed) {
            world.speed = speed;
            document.querySelectorAll('#controls button').forEach(b => b.classList.remove('active'));
            document.getElementById(`speed-${speed}`)?.classList.add('active');
        };

        window.addRandomNPC = function() {
            const npc = createNPC();
            world.npcs.push(npc);
            updateUI();
        };

        window.toggleCamera = function() {
            // Switch between top-down and orbit
            const pos = camera.position;
            if (pos.y > 50) {
                camera.position.set(60, 30, 60);
            } else {
                camera.position.set(0, 100, 0.1);
            }
            controls.target.set(0, 0, 0);
            controls.update();
        };

        // ============================================================
        // RAYCASTER - Click NPC
        // ============================================================
        const raycaster = new THREE.Raycaster();
        const pointer = new THREE.Vector2();

        renderer.domElement.addEventListener('click', (event) => {
            const rect = renderer.domElement.getBoundingClientRect();
            pointer.x = ((event.clientX - rect.left) / rect.width) * 2 - 1;
            pointer.y = -((event.clientY - rect.top) / rect.height) * 2 + 1;

            raycaster.setFromCamera(pointer, camera);

            // Check all NPC meshes
            const meshes = [];
            for (const [id, mesh] of npcMeshes) {
                meshes.push(mesh);
            }

            const intersects = raycaster.intersectObjects(meshes, true);

            if (intersects.length > 0) {
                let npcId = null;
                let obj = intersects[0].object;
                while (obj) {
                    if (obj.userData && obj.userData.npcId) {
                        npcId = obj.userData.npcId;
                        break;
                    }
                    obj = obj.parent;
                }

                // Find NPC by mesh
                for (const [id, mesh] of npcMeshes) {
                    if (mesh === intersects[0].object || mesh.children.includes(intersects[0].object)) {
                        npcId = id;
                        break;
                    }
                }

                if (npcId) {
                    const npc = world.npcs.find(n => n.id === npcId);
                    if (npc && npc.isAlive) {
                        showNPCInfo(npcId);
                    }
                }
            }
        });

        // Set NPC ID on meshes
        const originalCreateNPC = createNPC;
        createNPC = function(name) {
            const npc = originalCreateNPC(name);
            npc.mesh.userData.npcId = npc.id;
            npc.mesh.children.forEach(child => {
                child.userData.npcId = npc.id;
            });
            return npc;
        };

        // ============================================================
        // FPS COUNTER
        // ============================================================
        let frameCount = 0;
        let lastFpsUpdate = Date.now();

        // ============================================================
        // RESIZE
        // ============================================================
        window.addEventListener('resize', () => {
            const w = container.clientWidth;
            const h = container.clientHeight;
            camera.aspect = w / h;
            camera.updateProjectionMatrix();
            renderer.setSize(w, h);
            labelRenderer.setSize(w, h);
        });

        // ============================================================
        // ANIMATION LOOP
        // ============================================================
        function animate() {
            requestAnimationFrame(animate);

            // Update world every frame
            updateWorld();

            // FPS
            frameCount++;
            const now = Date.now();
            if (now - lastFpsUpdate > 1000) {
                document.getElementById('fps-display').textContent = `⚡ ${frameCount} FPS`;
                frameCount = 0;
                lastFpsUpdate = now;
            }

            controls.update();
            renderer.render(scene, camera);
            labelRenderer.render(scene, camera);
        }

        // ============================================================
        // INIT
        // ============================================================
        console.log('🌍 Thế giới AI 3D');
        console.log('📌 Click NPC → Xem thông tin');
        console.log('📌 Scroll → Zoom');
        console.log('📌 Kéo → Xoay');
        console.log('📌 Space → Tạm dừng');

        // Create initial NPCs
        createInitialNPCs(30);

        // Start
        animate();

        // Expose for console debugging
        window.world = world;
        window.scene = scene;
        window.camera = camera;
        window.controls = controls;

        console.log('✅ Đã sẵn sàng!');
    </script>
</body>
</html>
