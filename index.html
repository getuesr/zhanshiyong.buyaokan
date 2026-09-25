<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PovPlayServer</title>
    <style>
        /* 基础重置 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            width: 100vw;
            height: 100vh;
            overflow: hidden;
            font-family: 'Segoe UI', 'PingFang SC', 'Microsoft YaHei', sans-serif;
            background-color: #000; /* 图片加载前的黑底 */
            user-select: none;
        }

        /* 全屏随机背景图 */
        #bg-image {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover; /* 保证填满屏幕不变形 */
            z-index: 1;
            transition: opacity 1.5s ease-in-out; /* 1.5秒平滑过渡 */
            opacity: 1;
        }

        /* 渐变遮罩层：确保文字在浅色或复杂图片上也能看清 */
        .overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(to bottom, rgba(0,0,0,0.3) 0%, rgba(0,0,0,0.6) 100%);
            z-index: 2;
        }

        /* 右上角时间 */
        .clock-container {
            position: absolute;
            top: 20px;
            right: 25px;
            background-color: rgba(0, 0, 0, 0.5);
            color: #ffffff;
            padding: 8px 20px;
            border-radius: 20px;
            font-size: 22px;
            font-weight: 600;
            letter-spacing: 1px;
            z-index: 3;
            backdrop-filter: blur(4px);
            font-variant-numeric: tabular-nums;
        }

        /* 正中央的文字区域 */
        .center-content {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
            z-index: 3;
            width: 100%;
        }

        /* 服务器名字 */
        .server-name {
            font-size: 64px;
            font-weight: 900;
            color: #ffffff;
            letter-spacing: 4px;
            text-shadow: 0 4px 15px rgba(0, 0, 0, 0.9);
            margin-bottom: 15px;
            animation: fadeInDown 1.5s ease-out;
        }

        /* 群号胶囊 */
        .group-number {
            display: inline-block;
            font-size: 24px;
            font-weight: bold;
            color: #ffffff;
            background-color: rgba(255, 255, 255, 0.15);
            border: 1px solid rgba(255, 255, 255, 0.3);
            padding: 10px 30px;
            border-radius: 30px;
            backdrop-filter: blur(8px);
            text-shadow: 0 2px 5px rgba(0, 0, 0, 0.8);
            animation: fadeInUp 1.5s ease-out;
        }

        /* 右下角水印 (根据要求：黑色小字) */
        .watermark {
            position: absolute;
            bottom: 15px;
            right: 20px;
            font-size: 14px;
            color: #000000; /* 黑色字 */
            font-weight: bold;
            z-index: 3;
            /* 加白色半透明背景和文字阴影，确保在深色图片上也能看到黑色字 */
            background-color: rgba(255, 255, 255, 0.6);
            padding: 4px 12px;
            border-radius: 6px;
            letter-spacing: 0.5px;
        }

        /* 简单的入场动画 */
        @keyframes fadeInDown {
            from { opacity: 0; transform: translateY(-30px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>
    <!-- 随机背景图 -->
    <img id="bg-image" src="" alt="背景">
    
    <!-- 遮罩层 -->
    <div class="overlay"></div>

    <!-- 右上角时间 -->
    <div class="clock-container" id="clock">00:00:00</div>

    <!-- 居中文字 -->
    <div class="center-content">
        <div class="server-name">PovPlayServer</div>
        <div class="group-number">服务器群号: 732101489</div>
    </div>

    <!-- 右下角版权声明 -->
    <div class="watermark">* 图片为网络随机获取,并不是自己上传！</div>

    <script>
        // 1. 实时时间显示
        function updateTime() {
            const now = new Date();
            const h = String(now.getHours()).padStart(2, '0');
            const m = String(now.getMinutes()).padStart(2, '0');
            const s = String(now.getSeconds()).padStart(2, '0');
            document.getElementById('clock').textContent = `${h}:${m}:${s}`;
        }
        setInterval(updateTime, 1000);
        updateTime();

        // 2. 全屏随机图片轮播
        const imgElement = document.getElementById('bg-image');

        function loadRandomImage() {
            // 请求 1920x1080 的随机图片
            const randomUrl = 'https://picsum.photos/1920/1080?random=' + Math.random();
            
            const tempImg = new Image();
            tempImg.onload = function() {
                // 等新图片完全加载后，淡出当前图片
                imgElement.style.opacity = 0;
                
                // 1.5秒后（完全淡出），替换src并淡入
                setTimeout(() => {
                    imgElement.src = randomUrl;
                    imgElement.style.opacity = 1;
                }, 1500); 
            };
            tempImg.src = randomUrl;
        }

        // 首次加载
        loadRandomImage();

        // 每 15 秒换一张图（10000毫秒 = 10秒，15000毫秒 = 15秒，根据自己喜好调整）
        setInterval(loadRandomImage, 15000);
    </script>
</body>
</html>
