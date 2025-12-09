<p align="center">
  <img src="assets_github/get_next_line.png" width="320" />
</p>
<h3 align="center">
  <em>Reading a line from a file descriptor is far too tedious.</em>
</h3>

---

## ⚠️ Disclaimer

- **Full Portfolio:** This repository focuses on this specific project. You can find my entire 42 curriculum 👉 [here](https://github.com/Overtekk/42).
- **Subject Rules:** I strictly follow the rules regarding 42 subjects; I cannot share the PDFs, but I explain the concepts in this README.
- **Archive State:** The code is preserved exactly as it was during evaluation (graded state). I do not update it, so you can see my progress and mistakes from that time.
- **Academic Integrity:** I encourage you to try the project yourself first. Use this repo only as a reference, not for copy-pasting. Be patient, you will succeed.

## 📂 Purpose

The goal of this project is to create a function that reads a line ending with a newline character (`\n`) from a file descriptor, regardless of its size.

This project introduces a highly specific and important concept in C: **Static Variables**.
We need to read a file content, but we don't know the length of the lines or the file itself. Since we read by "chunks" (defined by a buffer size), we often read too much data. The challenge is to "remember" this extra data for the next function call without using global variables.
It's also teach you the wonderful world of leaks and segfault 🏊‍♂️.

## 🐨 Status

Completed on **12/11/2025** without bonus.
<p align="left">
  <img src="assets_github/get_next_line_score.png" width="150" />
  &nbsp;&nbsp;
  <img src="assets_github/get_next_line_Moulinette.png" width="400" />
</p>

## 🔷 Usage

### First, clone this repository.
```bash
https://github.com/Overtekk/so_long.git
```

### I have provided a complete `main` to test your get_next_line. You can run it using this command *(don't forget to define a `BUFFER_SIZE` if needed, though my code handles 3 by default)*:
```bash
cc -Wall -Werror -Wextra main/main.c get_next_line.c get_next_line_utils.c
```
### The fist test is **interactive***. You can choose which file you want to test using:
```bash
./a.out main/simple_test.text
```
### I've provided a lot of `.txt` files to test. Alongside, inside the main, there are 2 more tests you need to uncomment. The first test checks an invalid FD. The second one calls an empty file twice. I will not tell you why those tests exist. It's up to you to learn and try.

---
