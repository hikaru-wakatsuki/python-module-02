*This project has been created as part of the 42 curriculum by hwakatsu.*

# Garden Guardian

## Description / 説明

### English
Garden Guardian is a Python project about exception handling in smart-agriculture style programs. Its goal is to build simple but resilient monitoring logic that validates sensor-like inputs, distinguishes different failure types, uses custom exceptions, guarantees cleanup with `finally`, raises explicit errors when data is invalid, and integrates those ideas into a small garden-management system.

This repository contains six exercises:

- `ex0/ft_first_exception.py`: temperature validation with basic `try/except`
- `ex1/ft_different_errors.py`: examples of multiple built-in error types
- `ex2/ft_custom_errors.py`: custom garden-related exception classes
- `ex3/ft_finally_block.py`: cleanup logic with `finally`
- `ex4/ft_raise_errors.py`: explicit validation using `raise`
- `ex5/ft_garden_management.py`: integration of custom errors, cleanup, and recovery in a `GardenManager`

From the code in this repository, the project demonstrates:

- validation of agricultural-style numeric input
- handling of `ValueError`, `ZeroDivisionError`, `FileNotFoundError`, and `KeyError`
- inheritance-based custom exception design with `GardenError`, `PlantError`, and `WaterError`
- guaranteed cleanup behavior through `finally`
- defensive validation and recovery logic inside a small management class

### 日本語
Garden Guardian は、スマート農業風のプログラムを題材に例外処理を学ぶ Python プロジェクトです。目的は、センサー入力のような値の検証、異なる障害種別の判別、custom exception の利用、`finally` による確実な後始末、無効データに対する `raise`、そしてそれらを小さな garden management system に統合することです。

このリポジトリには 6 つの exercise があります。

- `ex0/ft_first_exception.py`: 基本的な `try/except` を使った温度検証
- `ex1/ft_different_errors.py`: 複数の built-in error の実例
- `ex2/ft_custom_errors.py`: garden 向け custom exception クラス
- `ex3/ft_finally_block.py`: `finally` を使った cleanup
- `ex4/ft_raise_errors.py`: `raise` を使った明示的な検証
- `ex5/ft_garden_management.py`: custom errors、cleanup、recovery を統合した `GardenManager`

このリポジトリの実装では、次の内容が確認できます。

- 農業データ風の数値入力検証
- `ValueError`、`ZeroDivisionError`、`FileNotFoundError`、`KeyError` の処理
- `GardenError`、`PlantError`、`WaterError` による継承ベースの custom exception 設計
- `finally` による確実な cleanup 動作
- 小さな管理クラス内での defensive validation と recovery ロジック

## Instructions / 実行方法

### English

Requirements:

- Python 3.10 or later
- No external dependencies

Run each exercise from the repository root:

```bash
python3 ex0/ft_first_exception.py
python3 ex1/ft_different_errors.py
python3 ex2/ft_custom_errors.py
python3 ex3/ft_finally_block.py
python3 ex4/ft_raise_errors.py
python3 ex5/ft_garden_management.py
```

Optional lint check:

```bash
flake8 ex0 ex1 ex2 ex3 ex4 ex5
```

There is no compilation or installation step. The project uses only Python standard language features and built-in exception types.

### 日本語

必要環境:

- Python 3.10 以上
- 外部依存関係なし

リポジトリのルートで、各 exercise は次のように実行できます。

```bash
python3 ex0/ft_first_exception.py
python3 ex1/ft_different_errors.py
python3 ex2/ft_custom_errors.py
python3 ex3/ft_finally_block.py
python3 ex4/ft_raise_errors.py
python3 ex5/ft_garden_management.py
```

任意の lint チェック:

```bash
flake8 ex0 ex1 ex2 ex3 ex4 ex5
```

コンパイルやインストールは不要です。このプロジェクトは Python 標準の言語機能と built-in exception を使っています。

## Features / 主な内容

### English

- Input parsing and validation with graceful fallback behavior
- Separation of different built-in exception categories
- Custom exception hierarchies for domain-specific errors
- `finally` blocks to guarantee cleanup actions
- Explicit `raise`-based validation for plant health rules
- A small `GardenManager` that combines validation, watering, cleanup, and recovery

### 日本語

- 入力解析と、失敗時も継続できる検証処理
- built-in exception の種類ごとの分離処理
- ドメイン固有エラーのための custom exception 階層
- cleanup を保証する `finally` ブロック
- 植物状態のルール検証を行う `raise` ベースの処理
- 検証、給水、cleanup、recovery を組み合わせた小さな `GardenManager`

## Usage Overview / 使い方の概要

### English

- `ex0` introduces simple conversion and range validation.
- `ex1` shows how different failures map to different exception types.
- `ex2` and `ex4` focus on making errors more explicit and domain-specific.
- `ex3` focuses on cleanup guarantees.
- `ex5` combines all major concepts into one flow.

### 日本語

- `ex0` は単純な変換と範囲検証を扱います。
- `ex1` は失敗の種類ごとに異なる exception になることを示します。
- `ex2` と `ex4` は、エラーをより明示的かつドメイン固有にする点に焦点があります。
- `ex3` は cleanup の保証に焦点があります。
- `ex5` は主要な概念を 1 つの流れに統合しています。

## Resources / 参考資料

### English

Classic references related to the topic:

- [Python Documentation: Errors and Exceptions](https://docs.python.org/3/tutorial/errors.html)
- [Python Documentation: Built-in Exceptions](https://docs.python.org/3/library/exceptions.html)
- [Python Documentation: Classes](https://docs.python.org/3/tutorial/classes.html)
- [Python Documentation: try Statement](https://docs.python.org/3/reference/compound_stmts.html#the-try-statement)
- [Real Python: Python Exceptions](https://realpython.com/python-exceptions/)
- [Real Python: Raising Exceptions in Python](https://realpython.com/python-raise-exception/)
- [flake8 Documentation](https://flake8.pycqa.org/)

AI usage in this project:

- AI was used for documentation support and README drafting.
- It was used to inspect the repository structure, summarize the purpose of each exercise, and provide bilingual English/Japanese wording.

### 日本語

この課題に関連する代表的な参考資料:

- [Python Documentation: Errors and Exceptions](https://docs.python.org/3/tutorial/errors.html)
- [Python Documentation: Built-in Exceptions](https://docs.python.org/3/library/exceptions.html)
- [Python Documentation: Classes](https://docs.python.org/3/tutorial/classes.html)
- [Python Documentation: try Statement](https://docs.python.org/3/reference/compound_stmts.html#the-try-statement)
- [Real Python: Python Exceptions](https://realpython.com/python-exceptions/)
- [Real Python: Raising Exceptions in Python](https://realpython.com/python-raise-exception/)
- [flake8 Documentation](https://flake8.pycqa.org/)

このプロジェクトにおける AI の利用:

- AI はドキュメント補助と README 作成支援に使用しました。
- リポジトリ構造の確認、各 exercise の目的要約、英語と日本語の文章作成に利用しました。

## Notes / 補足

### English
This project emphasizes defensive programming and clear failure handling rather than complex agricultural logic. The main objective is to show that a program can keep behaving predictably even when operations fail.

### 日本語
このプロジェクトは複雑な農業ロジックよりも、防御的プログラミングと明確な障害処理を重視しています。主目的は、処理が失敗してもプログラムが予測可能に動き続けられることを示す点です。
