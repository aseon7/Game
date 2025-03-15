<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form Pertanyaan Pilihan Ganda</title>
    <style>
        body {
            font-family: Arial, sans-serif;
        }
        .question {
            margin-bottom: 20px;
        }
        .result {
            display: none;
            margin-top: 20px;
            padding: 10px;
            background-color: #d4edda;
            color: #155724;
            border: 1px solid #c3e6cb;
            border-radius: 5px;
        }
    </style>
</head>
<body>

    <h1>Form Pertanyaan Pilihan Ganda</h1>

    <form id="quizForm">
        <div class="question">
            <p>1. Apa ibukota Indonesia?</p>
            <label><input type="radio" name="q1" value="a"> Jakarta</label><br>
            <label><input type="radio" name="q1" value="b"> Bandung</label><br>
            <label><input type="radio" name="q1" value="c"> Surabaya</label><br>
        </div>

        <div class="question">
            <p>2. Siapa presiden pertama Indonesia?</p>
            <label><input type="radio" name="q2" value="a"> Soeharto</label><br>
            <label><input type="radio" name="q2" value="b"> Soekarno</label><br>
            <label><input type="radio" name="q2" value="c"> Jokowi</label><br>
        </div>

        <button type="submit">Submit</button>
    </form>

    <div id="result" class="result">
        <p>Selamat! Semua jawaban Anda benar.</p>
        <a href="halaman_lain.html">Lanjut ke halaman berikutnya</a>
    </div>

    <script>
        document.getElementById('quizForm').addEventListener('submit', function(event) {
            event.preventDefault(); // Mencegah form submit secara default

            // Jawaban yang benar
            const correctAnswers = {
                q1: 'a', // Jawaban benar untuk pertanyaan 1
                q2: 'b'  // Jawaban benar untuk pertanyaan 2
            };

            // Ambil jawaban dari form
            const userAnswers = {
                q1: document.querySelector('input[name="q1"]:checked')?.value,
                q2: document.querySelector('input[name="q2"]:checked')?.value
            };

            // Cek apakah semua jawaban benar
            const allCorrect = Object.keys(correctAnswers).every(key => userAnswers[key] === correctAnswers[key]);

            if (allCorrect) {
                document.getElementById('result').style.display = 'block';
            } else {
                alert('Maaf, ada jawaban yang salah. Silakan coba lagi.');
            }
        });
    </script>

</body>
</html>
