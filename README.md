==========================================
🧩 I. Khởi tạo và cấu hình ban đầu
==========================================
| Lệnh                                                 | Mục đích                                      |
| ---------------------------------------------------- | --------------------------------------------- |
| `git --version`                                      | Kiểm tra phiên bản Git                        |
| `git config --global user.name "Tên của bạn"`        | Đặt tên người dùng cho Git                    |
| `git config --global user.email "email@example.com"` | Đặt email người dùng                          |
| `git config --list`                                  | Xem toàn bộ cấu hình Git hiện tại             |
| `git init`                                           | Tạo repository Git mới trong thư mục hiện tại |

==========================================
🧰 II. Làm việc với repository
==========================================
| Lệnh                              | Mục đích                                                          |
| --------------------------------- | ----------------------------------------------------------------- |
| `git status`                      | Xem trạng thái file (thay đổi, thêm mới, xóa, v.v.)               |
| `git add <tên_file>`              | Thêm file cụ thể vào khu vực chuẩn bị commit                      |
| `git add .`                       | Thêm tất cả file thay đổi                                         |
| `git commit -m "Nội dung commit"` | Ghi lại thay đổi vào lịch sử Git                                  |
| `git log`                         | Xem lịch sử commit                                                |
| `git diff`                        | Xem nội dung thay đổi giữa hai phiên bản                          |
| `git restore <file>`              | Hủy thay đổi chưa commit trong file                               |
| `git reset --hard HEAD`           | Trở về trạng thái commit gần nhất (xóa sạch thay đổi chưa commit) |

==========================================
🌐 III. Kết nối với GitHub (remote repository)
==========================================
| Lệnh                                  | Mục đích                      |
| ------------------------------------- | ----------------------------- |
| `git remote add origin <url>`         | Thêm liên kết đến GitHub repo |
| `git remote -v`                       | Xem danh sách remote hiện tại |
| `git remote set-url origin <url_mới>` | Đổi URL remote (HTTPS ↔ SSH)  |

==========================================
🚀 IV. Đồng bộ hóa (Push & Pull)
==========================================
| Lệnh                      | Mục đích                                       |
| ------------------------- | ---------------------------------------------- |
| `git push -u origin main` | Đẩy (push) commit đầu tiên lên GitHub          |
| `git push`                | Đẩy các commit mới                             |
| `git pull`                | Lấy thay đổi mới nhất từ GitHub về             |
| `git fetch`               | Tải thông tin mới từ GitHub (nhưng chưa merge) |

==========================================
🧭 V. Làm việc với nhánh (branch)
==========================================
| Lệnh                                                     | Mục đích                                  |
| -------------------------------------------------------- | ----------------------------------------- |
| `git branch`                                             | Xem danh sách các nhánh                   |
| `git branch <tên_nhánh>`                                 | Tạo nhánh mới                             |
| `git switch <tên_nhánh>` hoặc `git checkout <tên_nhánh>` | Chuyển sang nhánh khác                    |
| `git merge <tên_nhánh>`                                  | Hợp nhất (merge) nhánh vào nhánh hiện tại |
| `git branch -d <tên_nhánh>`                              | Xóa nhánh                                 |

==========================================
🧹 VI. Dọn dẹp và quản lý file
==========================================
| Lệnh                          | Mục đích                                          |
| ----------------------------- | ------------------------------------------------- |
| `git rm <file>`               | Xóa file khỏi repo (và hệ thống file)             |
| `git mv <file_cũ> <file_mới>` | Đổi tên hoặc di chuyển file                       |
| `git clean -f`                | Xóa các file chưa được theo dõi (untracked files) |

==========================================
💾 VII. .gitignore (rất quan trọng)
==========================================
Tạo file .gitignore để loại trừ file không cần đẩy lên GitHub, ví dụ:
build*/
*.pro.user
*.obj
*.exe
*.dll
*.o
*.log

==========================================
🧠 VIII. Một vài mẹo hữu ích
==========================================
| Mẹo                          | Lệnh                       |
| ---------------------------- | -------------------------- |
| Xem commit gần nhất          | `git show`                 |
| Quay lại commit cũ           | `git checkout <mã_commit>` |
| Quay lại nhánh chính         | `git switch main`          |
| Xem ai sửa file gần đây      | `git blame <file>`         |
| Nén lịch sử commit (cho gọn) | `git rebase -i HEAD~3`     |

==========================================
💡 Quy trình cơ bản hằng ngày
 ==========================================
git status          # Kiểm tra trạng thái
git add .           # Thêm file mới/thay đổi
git commit -m "Cập nhật giao diện chính"
git pull            # Lấy thay đổi mới nhất
git push            # Đẩy code lên GitHub



