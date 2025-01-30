<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>نموذج تسجيل الدخول</title>
</head>
<body>

    <h1>تسجيل الدخول</h1>
    <form id="loginForm">
        <label for="email">البريد الإلكتروني:</label>
        <input type="email" id="email" required><br><br>

        <label for="password">كلمة المرور:</label>
        <input type="password" id="password" required><br><br>

        <button type="submit">تسجيل الدخول</button>
    </form>

    <script>
        document.getElementById('loginForm').addEventListener('submit', function(event) {
            event.preventDefault(); // منع الإرسال الافتراضي
            const email = document.getElementById('email').value;
            const password = document.getElementById('password').value;
            
            // هنا يمكنك إرسال البيانات إلى الخادم الخاص بك باستخدام API
            alert(`تم إرسال البيانات:\nالبريد الإلكتروني: ${email}\nكلمة المرور: ${password}`);
        });
    </script>

</body>
</html>
