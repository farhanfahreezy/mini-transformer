# Code Generation with Mini Transformer

## 📝 Task Description

Tugas ini berfokus pada **Code Generation**, yaitu menghasilkan potongan kode Python secara otomatis dari deskripsi soal dalam bahasa alami (Bahasa Inggris). Model yang digunakan adalah arsitektur **Transformer Decoder-Only** yang dilatih dari awal (_from scratch_) untuk memetakan deskripsi permasalahan menjadi solusi kode.

---

## 📊 Dataset

### Nama Dataset

**LeetCodeDataset**

### Sumber Dataset

Dataset ini tersedia secara publik di Hugging Face Datasets:  
🔗 [https://huggingface.co/datasets/newfacade/LeetCodeDataset](https://huggingface.co/datasets/newfacade/LeetCodeDataset)

### Deskripsi Singkat

LeetCodeDataset adalah kumpulan data berupa soal dan jawaban dari situs pemrograman **LeetCode**. Setiap entri dalam dataset berisi informasi terkait soal, metadata, serta potongan kode jawaban dalam bahasa Python.

### Statistik Dataset

- Jumlah entri: ±2.640 soal dan jawaban unik
- Bahasa soal: Inggris
- Bahasa jawaban: Python
- Format: JSON Lines (`.jsonl`)
- Jumlah kolom: 13 kolom
- Digunakan untuk pelatihan: `problem_description` dan `response`

### Contoh Data

```json
{
  "problem_description": "Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.",
  "response": "def twoSum(nums, target):\n    for i in range(len(nums)):\n        for j in range(i + 1, len(nums)):\n            if nums[i] + nums[j] == target:\n                return [i, j]"
}
```
