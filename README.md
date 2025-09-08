<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Image</title>
    <style>
        /* 基础样式：清除默认边距，设置盒子模型 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /*  Body 样式：让 body 充满整个视口 */
        body, html {
            height: 100%;
            width: 100%;
            overflow: hidden; /* 隐藏滚动条 */
        }

        /* 容器样式：使用 Flexbox 进行绝对居中 */
        .container {
            display: flex;
            justify-content: center; /* 水平居中 */
            align-items: center;     /* 垂直居中 */
            height: 100vh;           /* 容器高度 = 整个视口高度 */
            width: 100vw;            /* 容器宽度 = 整个视口宽度 */
        }

        /* 图片样式：按比例缩放并覆盖容器 */
        .centered-image {
            max-width: 100%;  /* 图片最大宽度为容器宽度 */
            max-height: 100%; /* 图片最大高度为容器高度 */
            width: auto;      /* 宽度自动，保持比例 */
            height: auto;     /* 高度自动，保持比例 */
            object-fit: contain; /* 关键属性：包含整个图片，可能留白 */
            /* object-fit: cover; */ 
            /* 如果用 cover，图片会覆盖整个区域，但可能裁剪边缘 */
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- 
            将 "images/your-image.jpg" 替换为你的实际图片路径！
            例如：src="my-picture.png" 或 src="photos/background.jpg"
        -->
        <img class="centered-image" src="2025-linyiyin-1.jpg" alt="">
        <img class="centered-image" src="2025-linyiyin-2.jpg" alt="">
    </div>
</body>
</html>
