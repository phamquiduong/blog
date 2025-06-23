## Với Windows 8.1 trở lên không kích hoạt được virtual environment của Python

![image](/python-khong-bat-duoc-venv/media.png)

### Ví dụ về lỗi
```bash
PS C:\django\admin\code_snippets\Django_Blog> venv/Scripts/activate
File C:\django\admin\code_snippets\Django_Blog\.venv\Scripts\activate.ps1 cannot be loaded because the execution of scripts is disabled on this system. Please see "get-help about_signing" for more details.
At line:1 char:22
+ venv/Scripts/activate <<<<
    + CategoryInfo          : NotSpecified: (:) [], PSSecurityException
    + FullyQualifiedErrorId : RuntimeException
```

<br>

### Cách khắc phục
- Các bạn chuột phải vào biểu tượng Start menu chọn **PowerShell Admin** (Hoặc **Terminal Admin** trên bản Windows 11 22H2)

- Nếu có hộp thoại xuất hiện, nhấn chọn Yes để cấp quyền Adminstrator

- Dán lệnh này vào powershell và nhấn Enter
  ```bash
  Set-ExecutionPolicy Unrestricted -Force
  ```
