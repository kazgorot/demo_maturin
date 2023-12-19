```bash
pipx install maturin

cargo new --lib <name>
```
1) update `Cargo.toml`
2) create pyproject.toml with maturin build-system
or just `maturin new [OPTIONS] <PATH>`
3) add `#[pymodule] and #[pyfunction]` in src/lib.rs


```bash
python -c 'import guessing_game;guessing_game.guess_the_number()'
Guess the number!
Please input your guess.
100
You guessed: 100
Too big!
Please input your guess.
50
You guessed: 50
Too big!
Please input your guess.
25
You guessed: 25
Too small!
Please input your guess.
30
You guessed: 30
You win!
```