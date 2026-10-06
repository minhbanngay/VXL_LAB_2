# Cấu trúc báo cáo Lab 2

Báo cáo của cả 10 exercise được quản lý tập trung trên branch `main`.

- `main.tex`: file LaTeX gốc.
- `preamble.tex`: trang bìa và thông tin sinh viên.
- `source/content/exercise_01.tex` đến `exercise_10.tex`: nội dung từng bài.
- `source/picture/ex01/` đến `ex10/`: ảnh Proteus và ảnh kết quả từng bài.

Không cập nhật report trên các branch `exercise/NN`. Sau khi hoàn thành firmware
của một bài, chuyển về `main` rồi bổ sung lời giải, mã nguồn và hình ảnh vào file
exercise tương ứng.

Build báo cáo:

```powershell
latexmk -pdf -outdir=build main.tex
```
