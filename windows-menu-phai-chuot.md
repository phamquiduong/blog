## Đưa menu chuột phải của Windows 11 về Windows 10

![image](/windows-menu-phai-chuot/media.png)

### Các bước thực hiện
- Các bạn chuột phải vào biểu tượng Start menu chọn PowerShell (Hoặc Terminal trên bản Windows 11 22H2 trở về sau)

- Dán lệnh này vào powershell và nhấn Enter
  ```bash
  reg add "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32" /f /ve
  ```

- Khởi động lại máy

<br>

### Khôi phục lại như cũ
- Mở termninal lên và chạy lệnh
  ```bash
  reg.exe delete "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}" /f
  ```
