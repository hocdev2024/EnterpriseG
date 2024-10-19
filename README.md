## [Download Latest Version](https://github.com/hocdev2024/EnterpriseG/archive/refs/heads/main.zip)
# Đọc kỹ phần quan trọng của README này
</div>

<div align="center">
  <img src="https://github.com/user-attachments/assets/55913650-be14-4352-986d-edf6ded3381d" alt="Image Description">
</div>

<div align="center">
  
# Làm thế nào để Reconstruct Enterprise G
</div>

[![Quy trình Reconstruct Enterprise G](https://img.youtube.com/vi/)](https://www.youtube.com/watch?v=n-bu1me3Vc4 "EnterpriseG Reconstruction Process")

`Tất cả những gì bạn cần cung cấp là:`
- Windows 10/11 Pro en-US install.wim image không có bản cập nhật (XXXXX.1)

> [**UUP Dump**](https://uupdump.net/) có thể tạo Windows Pro ISO ở định dạng en-US mà không cần cập nhật (bỏ chọn Include updates).
> 
**Mẹo hay:** Nếu bạn tạo ISO mới bằng UUP Dump, hãy đặt `AppsLevel` thành **1** bên trong `ConvertConfig.ini` trên bản dựng 22621 trở lên, điều này sẽ chỉ cài đặt Windows Security và Microsoft Store dưới dạng các ứng dụng được cài đặt sẵn! Ngoài ra, trên 26100 trở lên, việc đặt `SkipEdge` thành **1** sẽ không cài đặt sẵn Microsoft Edge hoặc Webview.
> 
Các bản dựng được hỗ trợ: 
- [17763](https://uupdump.net/download.php?id=6ce50996-86a2-48fd-9080-4169135a1f51&pack=en-us&edition=professional) (1809), [19041](https://uupdump.net/download.php?id=a80f7cab-84ed-43f4-bc6b-3e1c3a110028&pack=en-us&edition=professional) (2004), [22000](https://uupdump.net/download.php?id=6cc7ea68-b7fb-4de1-bf9b-1f43c6218f6f&pack=en-us&edition=professional) (21H2), [22621](https://uupdump.net/download.php?id=356c1621-04e7-4e66-8928-03a687c3db73&pack=en-us&edition=professional) (22H2 & 23H2) & [26100](https://uupdump.net/download.php?id=3d68645c-e4c6-4d51-8858-6421e46cb0bb&pack=en-us&edition=professional) (24H2)


`Cách bắt đầu:`
1. Tải 1 trong các bản ISO bên trên rồi để vào thư mục chạy ứng dụng
2. Chỉnh sửa options.json nếu bạn am hiểu hoặc thiết lập bằng ứng dụng
3. Chạy **EnterpriseG.exe** nó sẽ tìm kiếm các tệp iso và hỏi bạn có muốn giải nén không

>
<div align="center">
  
# options.json

</div>

## Activate Windows

- `true`: Kích hoạt Windows thông qua KMS38
- `false`: Windows sẽ không được kích hoạt

## Remove Edge

- `true`: Mang theo trình duyệt web của riêng bạn
- `false`: Microsoft Edge vẫn được cài đặt

<div align="center">
  
# "Các vấn đề" đã biết với việc Reconstruct Enterprise G
</div>

- Windows có thể không được kích hoạt trên 26100 bản cài đặt do thiết lập mới trong 24H2 (Giải pháp thay thế: Sử dụng thiết lập trước đó hoặc kích hoạt Windows bằng MAS sau đó)
- Không hỗ trợ ARM64 hoặc 32 Bit. Dự án này chỉ bao gồm X86_64/AMD64 (chỉ hỗ trợ PC 64 Bit)
<div align="center">

# Quan trọng
DỰ ÁN NÀY KHÔNG LÀM GIẢM BỀN WINDOWS. Nó thay thế Windows Pro bằng Windows Enterprise G SKU được nhiều cơ quan chính phủ sử dụng. Enterprise G đi kèm với một số chính sách sản phẩm được áp dụng theo mặc định, chẳng hạn như phần mềm diệt vi-rút Windows Defender bị vô hiệu hóa và giảm dữ liệu đo từ xa

Ví dụ, trong khi một số bộ phận của chính phủ Trung Quốc sử dụng phiên bản Windows này, họ vẫn có những sửa đổi bổ sung không dành cho công chúng.

Nếu bạn thực sự muốn chạy phiên bản giống hệt như họ, tốt hơn hết bạn nên tìm kiếm trên Google "Windows 10 Enterprise G CMGE_V2020-L.1207" – hiện đang có thông tin rò rỉ
</div>
