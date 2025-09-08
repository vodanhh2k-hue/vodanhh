<!DOCTYPE html>
<html>
<head>
    <title>Xóa nền ảnh bằng AI</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; padding: 20px; }
        #result { margin-top: 20px; }
        img { max-width: 300px; border: 1px solid #ddd; }
    </style>
</head>
<body>
    <h1>Xóa nền ảnh miễn phí</h1>
    <p>Tải lên ảnh để xóa nền tự động:</p>
    <input type="file" id="imageInput" accept="image/*">
    <button onclick="processImage()">Xóa nền</button>
    <div id="result"></div>

    <script>
        async function processImage() {
            const file = document.getElementById('imageInput').files[0];
            if (!file) return alert("Vui lòng chọn ảnh!");
