<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nhat Phan - Link Bio</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        body {
            background-color: #050515;
            color: #ffffff;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 20px;
            overflow: hidden;
            position: relative;
        }
        
        /* Hiệu ứng hình tròn sáng rực bay lên */
        .bubbles-bg {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, #090a0f, #1b2735);
            overflow: hidden;
            z-index: -1;
        }
        .bubble {
            position: absolute;
            bottom: -60px;
            background: rgba(255, 255, 255, 0.9);
            border-radius: 50%;
            box-shadow: 0 0 15px rgba(255, 255, 255, 0.8), 0 0 30px rgba(59, 130, 246, 0.6);
            animation: riseUp linear infinite;
        }

        .bubble:nth-child(1) { width: 18px; height: 18px; left: 10%; animation-duration: 5s; animation-delay: 0s; }
        .bubble:nth-child(2) { width: 30px; height: 30px; left: 25%; animation-duration: 8s; animation-delay: 2s; }
        .bubble:nth-child(3) { width: 14px; height: 14px; left: 40%; animation-duration: 4s; animation-delay: 1s; }
        .bubble:nth-child(4) { width: 24px; height: 24px; left: 55%; animation-duration: 7s; animation-delay: 3s; }
        .bubble:nth-child(5) { width: 35px; height: 35px; left: 70%; animation-duration: 9s; animation-delay: 0s; }
        .bubble:nth-child(6) { width: 18px; height: 18px; left: 85%; animation-duration: 6s; animation-delay: 4s; }
        .bubble:nth-child(7) { width: 26px; height: 26px; left: 95%; animation-duration: 7.5s; animation-delay: 1.5s; }

        @keyframes riseUp {
            0% {
                transform: translateY(0) scale(1);
                opacity: 0;
            }
            30% {
                opacity: 1;
            }
            100% {
                transform: translateY(-110vh) scale(1.3);
                opacity: 0;
            }
        }

        .bio-container {
            width: 100%;
            max-width: 400px;
            text-align: center;
            background: rgba(255, 255, 255, 0.04);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 24px;
            padding: 40px 20px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.6);
            z-index: 1;
        }
        .avatar {
            width: 90px;
            height: 90px;
            border-radius: 50%;
            background: linear-gradient(45deg, #3b82f6, #8b5cf6);
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 36px;
            font-weight: bold;
            margin: 0 auto 20px auto;
            border: 2px solid rgba(255, 255, 255, 0.2);
            box-shadow: 0 4px 20px rgba(59, 130, 246, 0.5);
        }
        h1 {
            font-size: 22px;
            margin-bottom: 8px;
            font-weight: 600;
        }
        p {
            color: #94a3b8;
            font-size: 14px;
            margin-bottom: 25px;
        }
        .links {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        /* Nút bấm viền nét đứt */
        .link-btn {
            display: block;
            background: rgba(255, 255, 255, 0.06);
            color: #ffffff;
            padding: 14px 20px;
            border-radius: 12px;
            text-decoration: none;
            font-weight: 500;
            font-size: 15px;
            border: 2px dashed rgba(255, 255, 255, 0.4);
            transition: all 0.3s ease;
        }
        
        .link-btn:hover {
            background: rgba(24, 119, 242, 0.2);
            border-color: #1877f2;
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(24, 119, 242, 0.3);
        }

        .footer {
            margin-top: 25px;
            font-size: 12px;
            color: #64748b;
        }
    </style>
</head>
<body>

    <div class="bubbles-bg">
        <div class="bubble"></div>
        <div class="bubble"></div>
        <div class="bubble"></div>
        <div class="bubble"></div>
        <div class="bubble"></div>
        <div class="bubble"></div>
        <div class="bubble"></div>
    </div>

    <div class="bio-container">
        <div class="avatar">NP</div>
        <h1>Nhat Phan</h1>
        <p>Roblox Script Developer</p>

        <div class="links">
            <a href="https://www.facebook.com/pnphan01/" target="_blank" class="link-btn">📘 Facebook: Nhat Phan</a>
        </div>

        <div class="footer">
            © 2026 Nhat Phan. All rights reserved.
        </div>
    </div>

</body>
</html>
