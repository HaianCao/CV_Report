# Report — Build & Run

This folder contains the LaTeX source for the Computer Vision report. The main entry is `main.tex` and the compiled output is `main.pdf` in this folder.

Prerequisites
- Windows: MiKTeX (pdfLaTeX + Biber) installed.
- (Optional) Perl + `latexmk` on PATH for convenient single-command builds.

# Báo cáo: Nhận diện tuổi từ ảnh khuôn mặt người

Thư mục này chứa mã nguồn LaTeX cho báo cáo môn Thị giác Máy tính. Nội dung hiện là khung báo cáo (skeleton) gồm các chương, phần mở đầu, phụ lục và file tài nguyên (hình ảnh, file bib).

Tóm tắt
- Mục tiêu: tài liệu mẫu cho báo cáo môn, cấu trúc theo yêu cầu môn học và dễ chỉnh sửa để thêm nội dung thực nghiệm.
- Trạng thái: khung báo cáo hoàn chỉnh và có thể biên dịch; nội dung chi tiết (kết quả, phân tích) cần được bổ sung.

Tác giả và nhóm
- Giảng viên hướng dẫn: TS. Cao Văn Chung
- Thành viên:
	- Cao Hải An — 23001818
	- Đặng Thế Anh — 23001821
	- Đỗ Minh Đức — 23001864

Cấu trúc chính của thư mục
- `main.tex` — file chính (entry point) của báo cáo.
- `preamble.tex` — gói lệnh, định dạng trang và thiết lập chung.
- `conver_page.tex` — trang bìa.
- `thankyou.tex`, `abstract.tex` — trang cảm ơn và tóm tắt.
- `chapters/` — các chương `chapter1.tex` ... `chapter5.tex` và `appendix.tex`.
- `images/` — hình minh họa sử dụng trong báo cáo.
- `thesis.bib` — cơ sở dữ liệu tham khảo (BibLaTeX).

Ghi chú ngắn
- README này chỉ là mô tả dự án; các hướng dẫn biên dịch đã được loại bỏ khỏi README theo yêu cầu. Nếu cần tài liệu hướng dẫn build riêng, mình sẽ tạo file `BUILD.md` hoặc script `build.ps1`.
- File `.gitignore` đã được thêm để bỏ các file tạm do LaTeX sinh ra.
