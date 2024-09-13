# InstallerBackhaul
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Copy to Clipboard Example</title>
    <style>
        .code-container {
            position: relative;
            background-color: #f4f4f4;
            padding: 15px;
            border-radius: 8px;
            margin-bottom: 20px;
            border: 1px solid #ddd;
        }

        .copy-btn {
            position: absolute;
            top: 10px;
            right: 10px;
            background-color: #007bff;
            color: white;
            border: none;
            padding: 5px 10px;
            border-radius: 5px;
            cursor: pointer;
        }

        pre {
            margin: 0;
            font-family: monospace;
            white-space: pre-wrap; /* Preserve whitespace formatting */
        }
    </style>
</head>
<body>

    <div class="code-container">
        <button class="copy-btn" onclick="copyCode()">Copy</button>
        <pre id="code">bash &lt;(wget -qO- https://raw.githubusercontent.com/PixelShellGIT/InstallerBackhaul/main/InstallerBackhaul.sh)</pre>
    </div>

    <script>
        function copyCode() {
            var codeElement = document.getElementById("code");
            var range = document.createRange();
            range.selectNode(codeElement);
            window.getSelection().removeAllRanges();
            window.getSelection().addRange(range);
            document.execCommand("copy");
            window.getSelection().removeAllRanges();
            alert("Code copied to clipboard!");
        }
    </script>

</body>
</html>



لطفاً با استار دادن از پروژه حمایت کنید. 🌟
