# STM32 Lab 2 -- Timer Interrupt

Repository chứa firmware, file mô phỏng và báo cáo cho 10 exercise của Lab 2,
sử dụng vi điều khiển STM32F103C6.

## Quy ước branch

- `main`: cấu hình dùng chung và toàn bộ báo cáo LaTeX.
- `exercise/01` đến `exercise/10`: firmware và Proteus của từng exercise.
- Chỉ cập nhật report trên `main`; không sửa report trực tiếp ở branch exercise.

Khi làm một bài, firmware được commit trên branch `exercise/NN`. Sau đó chuyển về
`main` để cập nhật file `report/source/content/exercise_NN.tex` tương ứng.

## Build firmware

```powershell
cmake --preset Debug
cmake --build --preset Debug -j 4
```

Firmware được giữ trong Git:

- `build/Debug/LAB_2.elf`
- `build/Debug/LAB_2.hex`

Các file build trung gian khác không được commit.

## Build báo cáo

```powershell
cd report
latexmk -pdf -outdir=build main.tex
```

File kết quả: `report/build/main.pdf`.

## Tài liệu bài thực hành

Đề bài gốc: `VXL_VDK_Lab_2_Timer.pdf` ở thư mục cha. Nội dung trong report chỉ là
khung tóm tắt yêu cầu; lời giải sẽ được bổ sung khi thực hiện từng exercise.
