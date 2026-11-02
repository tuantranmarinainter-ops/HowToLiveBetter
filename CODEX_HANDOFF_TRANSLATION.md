# CODEX HANDOFF — Hoàn tất dịch sách chương 16, 17, 19

Ngày giao việc: 2026-11-02. Repository: https://github.com/tuantranmarinainter-ops/HowToLiveBetter. **Nhánh duy nhất được phép sửa:** `dich-tieng-viet`. Mục tiêu là **thực thi toàn bộ**, không chỉ lập kế hoạch: hoàn tất 3 chương, kiểm định, commit riêng và push.

## Khởi động
1. `git fetch origin && git switch dich-tieng-viet && git pull --ff-only origin dich-tieng-viet`; không ghi đè công việc chưa commit của người khác.
2. Đọc đầy đủ `book-vi/01-dung-chet-som.md`, `book-vi/08-dung-tu-hai-minh.md` (thuật ngữ luật trong comment), `book-vi/13-tinh-huong-khan-cap.md` (thuật ngữ y khoa), `book-vi/18-nuoi-con-co-dang-khong.md`.
3. `git clone --depth 1 https://github.com/cuongphamISB/HowToLiveBetter /tmp/ref-cuong`. Bản này là tham khảo CC BY 4.0 **cũ**, không phải nguồn sự thật. Lấy `book/` của repo này (bản mới nhất) làm gốc. Đối chiếu **từng câu** từng mục gốc; tuyệt đối không lấy số liệu cũ từ bản tham khảo.

## Công việc — làm đúng thứ tự, QA rồi commit/push từng chương
1. `book/16-得了慢性病之后怎么活.md` → `book-vi/16-song-chung-benh-man-tinh.md`; 14 mục `###`, 84 dòng `- `. Tham khảo `/tmp/ref-cuong/book/16-benh-man-tinh.md` (9 mục cũ; 5 mục cần dịch mới).
2. `book/17-家里有老人.md` → `book-vi/17-trong-nha-co-nguoi-gia.md`; 13 mục, 78 dòng. Tham khảo `/tmp/ref-cuong/book/17-nguoi-cao-tuoi.md` (9 mục cũ; 4 mục dịch mới).
3. `book/19-在职离职和工伤.md` → `book-vi/19-di-lam-nghi-viec-tai-nan-lao-dong.md`; 24 mục, 144 dòng. Tham khảo `/tmp/ref-cuong/book/19-lao-dong.md` (18 mục cũ; 6 mục dịch mới).

Không sửa các file trong `book/`. Chương 00–15 và 18 đã có trên nhánh, không cần dịch lại. Không sửa nội dung khác ngoài phạm vi yêu cầu.

## Chuẩn dịch bắt buộc
- Dịch **toàn bộ** nguyên tác từng mục, không tóm tắt hoặc bỏ đoạn, số liệu, nghiên cứu, điều kiện ngoại lệ, nguồn, ghi chú, cảnh báo.
- Văn phong ngắn, tự nhiên, rõ ý theo ba chương mẫu; giữ Markdown, anchors, HTML comments, số mục, thứ tự bullet, **mọi URL và DOI nguyên trạng**, tên bài báo khoa học gốc.
- Nhãn: `Chi phí`, `Nói dễ hiểu`, `Lợi ích`, `Cấp độ bằng chứng`, `Nguồn`, `Ghi chú`, comment `Nhãn chi phí`. Không dùng `Hiểu đơn giản`, `Bằng chứng`, `cost:`.
- Định dạng số: 0,25 và 178.000; từ 1 triệu trở lên ghi theo đơn vị (lần đầu kèm số chính xác nếu cần). Không sửa chữ số trong URL, DOI, hotline, số văn bản, mã vụ án. Tiền giữ **nhân dân tệ**, không đổi sang VNĐ.
- `见第 X 节第 Y 条（…）` → `xem Chương X, mục Y (…)`. `争议` phải hiện là **Tranh cãi** ở đầu phần Ghi chú. Phân biệt `可以` và `应当`, `以下` và `以上`; giữ phủ định `别/不要`.
- Tên luật Trung Quốc dịch tiếng Việt, giữ số điều, lần đầu của chương kèm tên gốc trong ngoặc; không còn chữ Hán ngoài tên sách và tên luật được giữ có chủ đích.
- Ch16–17: **tuyệt đối chính xác tên thuốc, liều, chỉ số xét nghiệm, lịch tái khám**; không biến nội dung nghiên cứu thành lời khuyên cá nhân. Ch17 bảo toàn chi tiết giám hộ, di chúc, bảo hiểm dài hạn, tiền đặt cọc viện dưỡng lão.
- Ch19 thuật ngữ: `加班费`=tiền làm thêm giờ; `带薪年休假`=phép năm có lương; `试用期`=thời gian thử việc; `经济补偿 N`=trợ cấp thôi việc N; `代通知金`=tiền thay báo trước (N+1); `赔偿金 2N`=tiền bồi thường 2N; `工伤认定`=công nhận tai nạn lao động; `劳动能力鉴定`=giám định khả năng lao động; `竞业限制`=hạn chế cạnh tranh; `劳务派遣`=cho thuê lại lao động.
- Thủ tục, mức tiền, thời hạn Trung Quốc: bổ sung `*Ghi chú cho người Việt:*` nói rõ chỉ thuộc Trung Quốc. Chỉ nêu luật tương đương ở Việt Nam nếu có cơ sở xác thực; **không bịa**.
- Đầu **từng file** ghi nguyên văn: 
  `> Bản dịch tiếng Việt từ 《高性价比人生指南》 của eternity4719 — https://github.com/eternity4719/HowToLiveBetter`
  
  `Tham khảo một phần bản dịch CC BY 4.0 của cuongphamISB: https://github.com/cuongphamISB/HowToLiveBetter`

## QA trước khi commit mỗi chương
- Đếm `^### `: 14/13/24; đếm `^- `: 84/78/144 theo chương 16/17/19. Tự đối chiếu với gốc nếu gốc vừa được cập nhật.
- Trích URL từ gốc và bản dịch; **không URL gốc nào thiếu**, không sửa DOI. Số URL độc nhất tại thời điểm bàn giao xấp xỉ 47/43/46; số đếm chỉ là tham chiếu.
- Đối chiếu 6 bullet mỗi mục, cả `Lợi ích` và `Nói dễ hiểu`, con số, phần nguồn, phủ định, mức bằng chứng với bản gốc **hiện tại**.
- Quét chữ Hán sót (ngoại lệ hợp lệ ở tiêu đề sách và tên luật gốc); soát Markdown, thuật ngữ pháp lý/y tế, ghi chú địa phương.
- Có thể viết script QA trong workspace nhưng không cần commit script nếu không được yêu cầu. **QA cấu trúc không thay thế QA ngữ nghĩa**.

## Ghi Git và báo cáo
- Sau khi xong **mỗi chương**, stage đúng file đích, tạo 1 commit riêng, push lên `origin/dich-tieng-viet`, xác nhận file và SHA trên remote. Không force push, không gộp chương.
- Lặp lại đến khi đủ 3 chương, không dừng ở prototype hay báo cáo.
- Trả bảng cuối: file, KB, mục gốc/dịch, số mục dùng lại/viết mới, số bullet, URL gốc/giữ lại, QA PASS/FAIL, commit SHA và trạng thái push; nêu blocker thật, không báo hoàn thành khi chưa làm.
- Kết thúc kiểm tra `book-vi/` đã có đủ file 00–19.

**DoD:** Đủ 3 file chương 16,17,19, dịch đầy đủ theo bản gốc mới nhất, QA chính xác, 3 commit riêng đã push và xác nhận trên remote.
