<!DOCTYPE html>
<html lang="id">
    <title>Pelatihan UMKM Syariah</title>
    <link rel="style.css" href=""/>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Pelatihan Syariah</title>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-100">
    <nav class="bg-gradient-to-r from-blue-600 to-indigo-800 p-4 flex justify-between items-center text-white">
        <div class="text-xl font-bold">Pelatihan UMKM Syariah</div>
        <input type="text" placeholder="Cari pelatihan" class="px-3 py-1 rounded-md text-black">
        <div>
            <a href="#" class="px-4 py-2 bg-blue-500 rounded-md">Login</a>
        </div>
    </nav>

    <div class="flex justify-center items-center h-screen">
        <div class="bg-white p-6 rounded-lg shadow-lg w-96">
            <h2 class="text-xl font-bold mb-4 text-center">Login</h2>
            <button class="w-full bg-red-500 text-white py-2 rounded-lg">G+ Masuk dengan Google</button>
            <div class="text-center my-3 text-gray-500">atau</div>

            <form id="loginForm">
                <input type="email" id="email" placeholder="Email" class="w-full px-3 py-2 border rounded-lg mb-3" required>
                <input type="password" id="password" placeholder="Password" class="w-full px-3 py-2 border rounded-lg mb-3" required>
                <div class="flex items-center mb-3">
                    <input type="checkbox" id="captcha" class="mr-2"> <label for="captcha">I'm not a robot</label>
                </div>
                <button type="submit" class="w-full bg-blue-500 text-white py-2 rounded-lg">Login</button>
            </form>
            <p class="text-center mt-3">Belum punya akun? <a href="#" class="text-blue-500">Daftar</a></p>
        </div>
    </div>

    <footer class="bg-blue-900 text-white text-center p-3 fixed bottom-0 w-full">
        “Dan Allah menghalalkan jual beli dan mengharamkan riba.” (QS. al-Baqarah [2]: 275)
    </footer>

    <script>
        document.getElementById('loginForm').addEventListener('submit', function(event) {
            event.preventDefault();
            let email = document.getElementById('email').value;
            let password = document.getElementById('password').value;
            let captcha = document.getElementById('captcha').checked;
            
            if (!captcha) {
                alert('Harap centang CAPTCHA!');
                return;
            }

            alert('Login berhasil! Email: ' + email);
        });
    </script>
</body>
</html>
