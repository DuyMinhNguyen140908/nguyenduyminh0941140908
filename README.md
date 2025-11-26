# CHUYÊN ĐỀ TIN HỌC TỔ 3

## Mục Lục

1. Visual Studio Code & GitHub.
2. Hướng dẫn tải & sử dụng Visual Studio Code và GitHub.
3. Cách tải GitHub Desktop.
4. Cách liên kết Visual Studio Code và GitHub.
5. Cách tải dự án của bản thân từ Visual Studio Code lên Github.
6. Lấy các dự án của người khác từ Github về và tải Visual Studio Code.
7. Cách tạo và tham gia vào dự án mã nguồn mở.

---

## 1. Visual Studio Code & GitHub

### 1.1 Visual Studio Code (VS Code)

* **Giới thiệu:** Một trình soạn thảo mã nguồn **miễn phí** và **mã nguồn mở** do Microsoft phát triển. Nó phổ biến với khả năng hỗ trợ nhiều ngôn ngữ lập trình, và chạy được trên các nền tảng như Windows, macOS và Linux.
* **Dùng vào việc gì:**
    * Viết và chỉnh sửa mã nguồn (code)
    * Chạy và debug chương trình
    * Cài đặt nhiều tiện ích mở rộng (extensions)
* **Ưu điểm:**
    * Miễn phí, nhẹ
    * Hỗ trợ đa nền tảng (Windows, macOS, Linux)
    * Kho tiện ích mở rộng phong phú
    * Giao diện dễ tùy chỉnh
* **Nhược điểm:**
    * Cần cài thêm extension để hỗ trợ đầy đủ
    * Tốn tài nguyên khi mở nhiều dự án lớn
* **Độ thông dụng:**
    * Rất phổ biến trong giới lập trình
    * Được cộng đồng hỗ trợ mạnh mẽ

### 1.2 GitHub

* **Giới thiệu:** GitHub là một dịch vụ lưu trữ và quản lý mã nguồn dựa trên web, sử dụng hệ thống kiểm soát phiên bản Git.
* **Dùng vào việc gì:**
    * Lưu trữ dự án, mã nguồn
    * Quản lý phiên bản mã nguồn
    * Làm việc nhóm, đóng góp mã
    * Triển khai (deploy) website
    * Thảo luận và đánh giá
* **Ưu điểm:**
    * Miễn phí (gói cơ bản)
    * Hỗ trợ làm việc nhóm tốt
    * Nhiều công cụ tích hợp (Issues, Actions, Pull Request)
* **Nhược điểm:**
    * Cần làm quen với Git để sử dụng hiệu quả
    * Một số tính năng nâng cao cần trả phí
* **Độ thông dụng:**
    * Phổ biến nhất thế giới cho lập trình viên và dự án mã nguồn mở

---

## 2. Hướng dẫn tải & sử dụng Visual Studio Code và GitHub

### 2.1 Tải Visual Studio Code

1. Truy cập trang chủ Visual Studio Code. 
2. Bấm vào **Download**
2. Bấm vào **Download**  
   <img width="1756" src="https://github.com/user-attachments/assets/1dee1d40-d2eb-451f-a8d0-b4938f7a3cda" />
3. Chọn phiên bản phù hợp với hệ điều hành (Windows, Linux, Mac).
![alt text](image-1.png)
4. Tải xuống và cài đặt bình thường. 
![alt text](image-2.png)
![alt text](image-3.png)
### 2.2 Sử dụng Visual Studio Code

* **Mở VS Code.**
![alt text](image-4.png)
* **Tạo hoặc mở thư mục dự án:**
    * **Bước 1:** Chọn **File** > **New Folder** (hoặc **File** > **New Workspace** tùy phiên bản).
    * **Bước 2:** Tạo một thư mục mới cho dự án của bạn và đặt tên cho nó.
    * **Bước 3:** Sau khi tạo thư mục, bạn có thể mở nó bằng cách chọn **File** > **Open Folder** và chọn thư mục vừa tạo.
* **Cài đặt các extension cần thiết.**
![alt text](image-5.png)
* **Viết mã, chạy thử, debug.**

### 2.3 Tạo tài khoản GitHub

1. Vào trang chủ GitHub. 

![alt text](image-6.png)

2. Đăng ký tài khoản.
![alt text](image-7.png)
3. Xác minh email.

### 2.4 Sử dụng GitHub cơ bản

* **Tạo repository:**
    * **Bước 1:** Đăng nhập GitHub → nhấn nút **New** hoặc vào [https://github.com/new](https://github.com/new).
    * **Bước 2:** Điền thông tin:
        * `Repository name`: tên dự án
        * `Description`: mô tả (không bắt buộc)
        * Chọn **Public** hoặc **Private**
        * Chọn **Add README** nếu muốn có file README mặc định
        * Nhấn **Create repository**
    * **Tạo repository từ Git trên máy:**
        ```bash
        git init
        git remote add origin [https://github.com/username/repo.git](https://github.com/username/repo.git)
        git branch -M main
        git push -u origin main
        ```
* **Commit, push mã nguồn:**
    ```bash
    git add .
    git commit -m "Mô tả thay đổi"
    git push
    ```
    * `git add .`: Chọn toàn bộ file để commit
    * `git commit -m "..."`: Ghi lại thay đổi với một thông điệp
    * `git push origin main`: Đẩy mã lên nhánh main
* **Tạo nhánh, merge nhánh:**
    * **Tạo và chuyển sang nhánh mới:**
        ```bash
        git branch feature-login
        git checkout feature-login
        ```
    * **Merge nhánh vào main:**
        * Chuyển về main:
            ```bash
            git checkout main
            ```
        * Merge:
            ```bash
            git merge feature-login
            ```
        * Push lên Github:
            ```bash
            git push
            ```
* **Tạo issue và pull request:**
    * **Issue:**
        * **Bước 1:** Vào mục **Issues** của repository
        * **Bước 2:** Chọn **New Issue**
            * Điền `Title`: tiêu đề vấn đề
            * Điền `Description`: mô tả chi tiết
        * **Bước 3:** Nhấn **Submit new issue**
    * **Pull request:**
        * **Bước 1:** Push nhánh mới lên GitHub
        * **Bước 2:** Vào tab **Pull requests** → **New pull request**
        * **Bước 3:** Chọn:
            * `base`: nhánh nhận (thường là main)
            * `compare`: nhánh chứa thay đổi
        * **Bước 4:** Nhấn **Create pull request**
        * **Bước 5:** Viết mô tả và gửi

---

## 3. Cách tải GitHub Desktop

1. Mở trang GitHub Desktop.
2. Chọn phiên bản tương ứng.
3. Tải xuống, chạy file cài đặt.
4. Đăng nhập tài khoản GitHub.
5. Kết nối repository để quản lý mã nguồn qua giao diện.

### 3.1. Clone repository từ GitHub về máy

* **Bước 1:** Mở GitHub Desktop → **File** → **Clone repository**
* **Bước 2:** Chọn repository bạn muốn làm việc
* **Bước 3:** Nhấn **Clone**
* → GitHub Desktop sẽ tải toàn bộ project về máy và quản lý nó bằng giao diện.

### 3.2. Add repository có sẵn trong máy

* **Bước 1:** Mở GitHub Desktop → **Add an existing repository**
* **Bước 2:** Chọn thư mục chứa mã nguồn
* **Bước 3:** GitHub Desktop sẽ quản lý Git trong thư mục đó

---

## 4. Liên kết VSCode với GitHub

* **B1:** Bấm vào hình đầu người (**Accounts**).
* **B2:** Chọn **“Sign in with GitHub”**.
![alt text](image-8.png)
* **B3:** Bấm **“Continue”**.
![alt text](image-9.png)
* **B4:** Đăng nhập bằng email.
* **B5:** Bấm **“Authorize Visual Studio Code”**.
![alt text](image-10.png)

---

## 5. Tải từ VSCode lên GitHub

* **B1:** Làm như hình.
![alt text](image-11.png)
* **B2:** Đặt tên tùy ý.
![alt text](image-12.png)
* **B3:** Bấm **“Commit”**.
![alt text](image-13.png)
* **B4:** Bấm **“Sync Changes”**.
![alt text](image-14.png)

---

## 6. Tải từ GitHub về VSCode

* **B1:** Bấm **“Clone Repository”**.
![alt text](image-15.png)
* **B2:** Sao chép URL của repository chứa file cần tải về máy.
![alt text](image-16.png)
* **B3:** Nhập URL đã sao chép.
![alt text](image-17.png)
* **B4:** Chọn nơi lưu trữ khi tải về và bắt đầu tải.

### Lưu ý:

* Nếu repository không phải của mình thì nên **“Fork”** trước khi tải về máy.
* **Các bước Fork như sau:**
    * **B1:** Bấm **“Fork”**.
    ![alt text](image-18.png)
    * **B2:** Đặt tên và bấm **“Create fork”**.
    ![alt text](image-19.png)

---

## 7. Cách tạo và tham gia vào dự án mã nguồn mở

### 7.1. Cách tạo

* **B1 & B2:** Bấm vào dấu **`+`** trên thanh công cụ và Chọn **“New repository”**.
![alt text](image-20.png)
* **B3:** Đặt tên và nhập mô tả.
![alt text](image-21.png)
* **B4:** Chọn chế độ **“Public”**.
* **B5:** Bấm **“Create repository”**.
![alt text](image-22.png)

### 7.2. Cách tham gia

* **B1:** **Fork** repository muốn tham gia và thực hiện những chỉnh sửa mong muốn.
* **B2:** Bấm vào **“Pull request”**.
![alt text](image-23.png)
* **B3:** Bấm **“New pull request”**.
![alt text](image-24.png)
* **B4:** Bấm **“Create pull request”** để so sánh thay đổi.
![alt text](image-25.png)
* **B5:** Đặt tên cho phần `title` và bấm **“Create pull request”** để gửi yêu cầu đóng góp.
![alt text](image-26.png)
