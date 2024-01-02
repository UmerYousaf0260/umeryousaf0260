<h1 align="center">Hi 👋, I'm Umer Yousaf</h1>
<h3 align="center">A passionate frontend developer from Pakistan</h3>

    <h1>I'm a</h1>
    <h1 class="typing"></h1>

    <script>
        const text = ['Developer', 'Problem Solver', 'Mentor'];
        let wordCount = 0;
        let i = 0;
        let currentWord = '';
        let letter = '';

        (function type() {
            if (wordCount === text.length) {
                wordCount = 0;
            }

            currentWord = text[wordCount];
            letter = currentWord.slice(0, ++i);

            document.querySelector('.typing').textContent = letter;

            if (letter.length === currentWord.length) {
                wordCount++;
                i = 0;
            }

            setTimeout(type, 400);

        }());
    </script>
