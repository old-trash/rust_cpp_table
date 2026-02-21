## Аналогии в языках Rust и C++

## Фундаментальные типы

| Rust | C++ | Пример Rust | Пример C++ | Комментарий |
|------|-----|-------------|------------|-------------|
| `i32` | `std::int32_t` | `let x: i32 = 1;` | `const std::int32_t x = 1;` | Остальные типы по аналогии: `u32`, `i8`, ...<br>https://doc.rust-lang.ru/book/ch03-02-data-types.html |
| `()` | Возвращаемый `void` | `fn f() -> () {}` | `void f() {}` | Пустой кортеж в Rust - это и тип, и значение, а `void` в C++ - отсутствие типа<br>https://doc.rust-lang.ru/book/ch03-02-data-types.html#Кортежи |

## Изменяемость

| Rust | C++ | Пример Rust | Пример C++ | Комментарий |
|------|-----|-------------|------------|-------------|
| `let` | `const` | `let x = 1;` | `const auto x = 1;` | В Rust переменные неизменяемы по умолчанию<br>https://doc.rust-lang.ru/book/ch03-01-variables-and-mutability.html |
| `let mut` | | `let mut x = 1;` | `auto x = 1;` | |

## Указатели

| Rust | C++ | Пример Rust | Пример C++ | Комментарий |
|------|-----|-------------|------------|-------------|
| `Box<T>` | `std::unique_ptr<const T>` | | | Только чтение<br>https://doc.rust-lang.ru/book/ch15-01-box.html |
| `Rc<T>` (однопоточный)<br>`Arc<T>` (атомарный счётчик ссылок) | `std::shared_ptr<const T>` (атомарный счётчик) | | | Только чтение |


Полезные ссылки:
* https://www.programming-idioms.org/cheatsheet/Cpp/Rust
* https://rust-unofficial.github.io/patterns/
