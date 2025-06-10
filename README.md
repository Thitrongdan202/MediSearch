# MedicineSearch

## Hướng Dẫn Cài Đặt

1. **Tạo và Kích Hoạt Môi Trường Python**
   - Đảm bảo bạn đã cài đặt Python 3.13.
   - Tạo môi trường ảo:
     ```
     python3.13 -m venv venv
     ```
   - Kích hoạt môi trường ảo:
     - Trên macOS/Linux:
       ```
       source venv/bin/activate
       ```
     - Trên Windows:
       ```
       venv\Scripts\activate
       ```

2. **Cài Đặt Các Thư Viện Cần Thiết**
   - Cài đặt các thư viện cần thiết bằng lệnh sau:
     ```
     pip install -r requirements.txt
     ```

3. **Di Chuyển Models**
   - Chạy lệnh sau để khởi tạo cơ sở dữ liệu:
      ```
      python manage.py migrate
      ```

4. **Khởi Tạo Cơ Sở Dữ Liệu và Vector Hóa Dữ Liệu**
   - Chạy lệnh sau để khởi tạo cơ sở dữ liệu và vector hóa dữ liệu:
      ```
      python vectorize.py
      ```

5. **Thiết Lập Biến Môi Trường**
   - Thêm khóa gemini vào file .env:
      ```
      GEMINI_KEY="KHOA_GEMINI_CUA_BAN"
      ``` 

6. **Chạy Dự Án**
   - Khởi động ứng dụng FastAPI bằng lệnh:
     ```
     python manage.py runserver
     ```

   - Kiểm tra liên kết này: http://127.0.0.1:8000/search/