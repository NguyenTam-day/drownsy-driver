1. Mở dự án

Giải nén file ZIP, mở thư mục dự án bằng VS Code. Mở Terminal và chuyển vào thư mục chứa chương trình:

cd .\drownsy-detect

2. Tạo và kích hoạt môi trường ảo

Chỉ cần tạo môi trường ảo ở lần đầu tiên:

py -m venv .venv
.\.venv\Scripts\Activate.ps1

Nếu PowerShell chặn chạy script, nhập lệnh sau rồi kích hoạt lại:

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass

3. Cài thư viện

Cài các thư viện được khai báo trong requirements.txt:

python -m pip install --upgrade pip
python -m pip install -r requirements.txt

4. Chạy chương trình

Đảm bảo terminal đang ở thư mục drownsy-detect, môi trường (.venv) đã được kích hoạt và hai file mô hình best.pt vẫn còn trong thư mục runs tương ứng. Sau đó chạy:

python .\DrowsinessDetector.py

5. Dừng chương trình

Kill terminal
