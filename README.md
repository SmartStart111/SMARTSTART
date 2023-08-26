# SMARTSTART
EARLYADOPTER
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>性格测试</title>
    <style>
        /* 基本样式 */
        body {
            font-family: Arial, sans-serif;
            padding: 20px;
        }

        .test-section {
            margin-bottom: 40px;
        }

        button {
            padding: 10px 15px;
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="test-section">
        <h2>Big Five 测试</h2>
        <!-- 示例问题，您可以添加更多 -->
        <p>问题 1: 你认为自己是一个外向的人吗?</p>
        <select id="bigFiveQ1">
            <option value="1">非常不同意</option>
            <option value="2">不同意</option>
            <option value="3">中立</option>
            <option value="4">同意</option>
            <option value="5">非常同意</option>
        </select>
        <!-- ... 更多问题 -->
        <button onclick="calculateBigFive()">提交</button>
        <p id="bigFiveResult"></p>
    </div>

    <div class="test-section">
        <h2>MBTI 测试</h2>
        <!-- 示例问题，您可以添加更多 -->
        <p>问题 1: 你喜欢在团队中工作还是独自工作?</p>
        <select id="mbtiQ1">
            <option value="E">团队中</option>
            <option value="I">独自</option>
        </select>
        <!-- ... 更多问题 -->
        <button onclick="calculateMBTI()">提交</button>
        <p id="mbtiResult"></p>
    </div>

    <script>
        // JavaScript逻辑部分，简化版评估用户答案
        function calculateBigFive() {
            var score = parseInt(document.getElementById("bigFiveQ1").value);
            // ... 添加更多问题的得分

            // 示例逻辑，您可以根据需要修改
            if (score > 3) {
                document.getElementById("bigFiveResult").innerText = "您是一个外向的人。";
            } else {
                document.getElementById("bigFiveResult").innerText = "您是一个内向的人。";
            }
        }

        function calculateMBTI() {
            var type = document.getElementById("mbtiQ1").value;
            // ... 考虑更多问题的答案

            // 示例逻辑
            if (type === "E") {
                document.getElementById("mbtiResult").innerText = "您是一个团队型的人。";
            } else {
                document.getElementById("mbtiResult").innerText = "您更喜欢独自工作。";
            }
        }
    </script>
</body>
</html>
