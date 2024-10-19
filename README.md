## [Download Latest Version](https://github.com/hocdev2024/EnterpriseG/archive/refs/heads/main.zip)
# Đọc kỹ phần quan trọng của README này
</div>

<div align="center">
  <img src="https://github.com/xLSX285/EnterpriseG/assets/129116755/0eaff5b7-caa8-48e4-898f-cc38254712d6" alt="Image Description">
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

> Run this command in Powershell if Build.ps1 is not starting. **Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass**
> 
Once the reconstruction process is complete, you will find the new `install.wim` file in the same folder where you placed the original install.wim file. (**Please note:** your original `install.wim` file has been overwritten and cannot be restored!)
To proceed, you can create a new ISO using AnyBurn or any similar software. If you have already created a bootable Windows installation USB drive, simply copy the new `install.wim` file and replace the existing one located in the `sources` directory of your USB drive.
>
<div align="center">
  
# Config.ini

</div>

## ActivateWindows

- `true`: Activate Windows via KMS38 `Default`
- `false`: Windows wont be activated

## RemoveEdge

- `true`: Bring your own web browser `Default`
- `false`: Microsoft Edge remains installed

<div align="center">
  
# Known "issues" with Enterprise G reconstruction
</div>

- Inplace upgrade might get undone/reverted on some builds of Windows (e.g 19041 -> 22000/22621.) (looking for a fix)
- Windows might not be activated on 26100 installs due to the new setup in 24H2 (Workaround: Use previous setup or activate windows using MAS afterwards)
- No ARM64 or 32 Bit support. This project only covers X86_64/AMD64 (64 Bit PCs support only)
<div align="center">

# Important
I'm not actively maintaining this project. I'll push some commits here and there to ensure support for future Windows builds and some optimizations, that's it. This project requires some knowledge. No support will be provided.

THIS PROJECT DOES NOT DEBLOAT WINDOWS. It replaces Windows Pro with the Windows Enterprise G SKU used by various government entities. Enterprise G comes with some product policies applied by default, such as a disabled Windows Defender antivirus and reduced telemetry.

While some parts of the Chinese government, for example, use this exact edition of Windows, they have additional modifications that are not available to the general public.

If you're actually interested in running the exact same version as them, you're better off Googling "Windows 10 Enterprise G CMGE_V2020-L.1207" – there are leaks circulating around.

You shouldn't be using this daily, unless you really want to. This is just for fun.
</div>
