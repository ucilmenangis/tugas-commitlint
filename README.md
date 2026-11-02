# Tugas Commitlint

Tugas 2 Pertemuan 10 mata kuliah Standarisasi Coding: implementasi commitlint dan Husky.

* **Nama:** Muhammad Irfan Ar Rafi
* **NIM:** E41250682
* **Golongan:** B

## Isi
* `commitlint.config.js`: aturan Conventional Commits (type, subject huruf kecil, header maksimal 72 karakter).
* `.husky/commit-msg`: menjalankan commitlint setiap kali commit, commit yang tidak sesuai ditolak.
* `.husky/pre-commit`: menjalankan lint-staged, file `.js` yang di-stage dicek sintaksnya dengan `node --check`.

## Cara mencoba
```bash
npm install
echo "test" > test.txt
git add test.txt
git commit -m "update file"                                          # ditolak
git commit -m "feat(test): add test file for commitlint validation"  # diterima
```
