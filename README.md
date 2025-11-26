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
   <img src="https://github.com/user-attachments/assets/1dee1d40-d2eb-451f-a8d0-b4938f7a3cda" alt="image1" width="1756" />
3. Chọn phiên bản phù hợp với hệ điều hành (Windows, Linux, Mac).
   <img src="https://github.com/user-attachments/assets/fd9b321e-efb4-45cf-b977-db41bed21271" alt="image2" width="1090" />
4. Tải xuống và cài đặt bình thường. 
   <img src="https://github.com/user-attachments/assets/6bf4bb1a-c9bb-44fd-938d-b635a6733965" alt="image3" width="430">
   <img src="https://github.com/user-attachments/assets/3487dd09-0a09-44d7-8152-78e8c7f8a2e8" alt="image4" width="692">
### 2.2 Sử dụng Visual Studio Code

* **Mở VS Code.**
   <img src="https://github.com/user-attachments/assets/fd700d65-afd2-492e-ae50-44188ea5bb39" alt="image5" width="1091">
* **Tạo hoặc mở thư mục dự án:**
    * **Bước 1:** Chọn **File** > **New Folder** (hoặc **File** > **New Workspace** tùy phiên bản).
    * **Bước 2:** Tạo một thư mục mới cho dự án của bạn và đặt tên cho nó.
    * **Bước 3:** Sau khi tạo thư mục, bạn có thể mở nó bằng cách chọn **File** > **Open Folder** và chọn thư mục vừa tạo.
* **Cài đặt các extension cần thiết.**
   <img src="https://github.com/user-attachments/assets/ff1935fb-0240-4d00-9a75-606a46463123" alt="image6" width="914">
* **Viết mã, chạy thử, debug.**
   
### 2.3 Tạo tài khoản GitHub
1. Vào trang chủ GitHub. 
   <img src="https://github.com/user-attachments/assets/da2d51a2-a55d-47d9-a9f5-d6cc643b8870" alt="image7" width="1905">
2. Đăng ký tài khoản.
   <img src="https://github.com/user-attachments/assets/d6d22710-ce68-4a7c-ad50-a5da2c580c06" alt="image8" width="749">
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
    <img src="https://github.com/user-attachments/assets/671dd1af-5d49-4179-951e-93c914639d38" alt="image9" width="1179">
* **B3:** Bấm **“Continue”**.
    <img src="https://github.com/user-attachments/assets/184ad5e3-12da-4ba1-86cb-6439f6a2a9ca" alt="image10" width="1340">  
* **B4:** Đăng nhập bằng email.
* **B5:** Bấm **“Authorize Visual Studio Code”**.
    <img src="https://github.com/user-attachments/assets/5c6491f8-a584-4853-9396-ef4ce540894f" alt="image11" width="906">

---

## 5. Tải từ VSCode lên GitHub

* **B1:** Làm như hình.
    <img src="https://github.com/user-attachments/assets/98e3632e-4f33-4dc5-bd56-e2a66753cf8b" alt="image12" width="1178">
* **B2:** Đặt tên tùy ý.
    <img src="https://github.com/user-attachments/assets/a00f5d41-d182-4b61-a729-6efd56ad509d" alt="image13" width="1180">
* **B3:** Bấm **“Commit”**.
    <img src="https://github.com/user-attachments/assets/2493a73e-b16e-4bef-9391-d43d5278577f" alt="image14" width="1180">
* **B4:** Bấm **“Sync Changes”**.
    <img src="https://github.com/user-attachments/assets/e72bf68a-bc09-4591-b90f-79338d1330f1" alt="image15" width="1183">

---

## 6. Tải từ GitHub về VSCode

* **B1:** Bấm **“Clone Repository”**.
    <img src="https://github.com/user-attachments/assets/89fd3a70-7d35-40da-9099-80b9f855404c" alt="image16" width="1182">
* **B2:** Sao chép URL của repository chứa file cần tải về máy.
    <img src="https://github.com/user-attachments/assets/607b85e7-3474-4266-a77b-74e3dbe526a0" alt="image17" width="1348">
* **B3:** Nhập URL đã sao chép.
    <img src="https://github.com/user-attachments/assets/d01968c7-056f-4e76-8f10-9e2913e4cb15" alt="image18" width="1189">
* **B4:** Chọn nơi lưu trữ khi tải về và bắt đầu tải.

### Lưu ý:

* Nếu repository không phải của mình thì nên **“Fork”** trước khi tải về máy.
* **Các bước Fork như sau:**
    * **B1:** Bấm **“Fork”**.
        <img src="https://github.com/user-attachments/assets/03ef901e-79eb-403f-b5ca-aa40179eb58e" alt="image19" width="1336">
    * **B2:** Đặt tên và bấm **“Create fork”**.
        <img src="https://github.com/user-attachments/assets/38cc7b70-3461-4c4c-94ac-a1ca41db80b6" alt="image20" width="833">
---

## 7. Cách tạo và tham gia vào dự án mã nguồn mở

### 7.1. Cách tạo

* **B1 & B2:** Bấm vào dấu **`+`** trên thanh công cụ và Chọn **“New repository”**.
    <img src="https://github.com/user-attachments/assets/5c838415-b6b7-4356-83ff-302e079d7b2a" alt="image21" width="1365">
* **B3:** Đặt tên và nhập mô tả.
    <img src="https://github.com/user-attachments/assets/98647022-8d72-4588-a003-cd6132902072" alt="image22" width="1363">
* **B4:** Chọn chế độ **“Public”**.
* **B5:** Bấm **“Create repository”**.
    <img src="https://github.com/user-attachments/assets/c12b1d4e-f9e5-450f-b343-76bc3b74feba" alt="image23" width="1363">

### 7.2. Cách tham gia

* **B1:** **Fork** repository muốn tham gia và thực hiện những chỉnh sửa mong muốn.
* **B2:** Bấm vào **“Pull request”**.
    <img src="https://github.com/user-attachments/assets/0df1842e-cbf0-4651-b14e-ca277645a49c" alt="image24" width="1365">
* **B3:** Bấm **“New pull request”**.
    <img src="https://github.com/user-attachments/assets/590d5937-d612-4a50-8687-f2c914998199" alt="image25" width="1363">
* **B4:** Bấm **“Create pull request”** để so sánh thay đổi.
    <img src="https://github.com/user-attachments/assets/58786d08-326f-41c5-b0de-9265ab54b084" alt="image26" width="1363">
* **B5:** Đặt tên cho phần `title` và bấm **“Create pull request”** để gửi yêu cầu đóng góp.
    <img src="https://github.com/user-attachments/assets/c89dbb0f-7c8a-47d7-8c04-2667deb51c3c" alt="image27" width="1359">
