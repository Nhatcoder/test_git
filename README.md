📌 1. Các lệnh Git cơ bản (phải nhớ)
✔ Khởi tạo / clone repo

git init – tạo repo mới

git clone <url> – clone repo từ remote

✔ Trạng thái, thêm, commit

git status – xem trạng thái file

git add . – thêm tất cả file

git add <file> – thêm từng file

git commit -m "message" – commit nhanh

git commit -am "message" – add + commit file đã từng commit

✔ Push & Pull

git push – đẩy code lên remote

git pull – kéo code mới về

git fetch – lấy thông tin commit mới nhưng KHÔNG merge

📌 3. Undo / sửa lỗi nhanh
✔ Bỏ thay đổi chưa add
git restore <file>

✔ Bỏ thay đổi đã add (trong staging)
git restore --staged <file>

✔ Quay về commit trước
git reset --hard HEAD~1
12345
✔ Tạo commit 21321 mới để revert
git revert <commit_id>

✔ Lấy lại file đã xóa
git checkout HEAD -- <file>

📌 5. Các lỗi Git hay gặp & cách sửa
❌ "Authentication failed"

→ Sai token hoặc chưa add SSH key.

❌ "fatal: not a git repository"

→ Quên git init.

❌ "Merge conflict"

→ Mở file, sửa → git add . → git commit.

❌ "Updates were rejected" (push không được)

→ Branch bị out-of-date
→ Fix:

git pull --rebase
git push

Nếu muốn mình làm một sheet PDF ôn Git toàn bộ để bạn lưu, mình làm luôn cho — hoặc bạn hỏi phần nào muốn ôn kỹ, mình giảng sâu + ví dụ thực tế. 🚀