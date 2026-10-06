# Cấu trúc báo cáo Lab 2

Báo cáo Lab 2 dùng trực tiếp nội dung và hình ảnh của bài 2, không chia file theo
từng exercise.

- `main.tex`: file LaTeX gốc, nạp `source/content/bai_2.tex`.
- `preamble.tex`: trang bìa và thông tin sinh viên.
- `source/content/bai_2.tex`: toàn bộ nội dung của Lab 2.
- `source/picture/bai_2/`: toàn bộ hình ảnh của Lab 2.
- `assets/`: tài nguyên trình bày dùng chung của mẫu báo cáo.

Nguồn đồng bộ:

- `D:\Study\Lab VXL\[LATEX]MCU_LAB\source\content\bai_2.tex`
- `D:\Study\Lab VXL\[LATEX]MCU_LAB\source\picture\bai_2\`

Build báo cáo:

```powershell
latexmk -pdf -outdir=build main.tex
```
