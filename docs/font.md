# Bạn có đang sử dụng đúng phông chữ không?

Phông chữ tiếng Trung và Tiếng Nhật

Mặc định máy tính/điện thoại của bạn sẽ hiển thị chữ Kanji theo phông chữ tiếng Trung. Chữ Kanji trong Tiếng Nhật trông hơi khác một chút và sẽ khá vấn đề nếu bạn học Kanji kiểu tiếng Trung thay vì kiểu chữ Nhật.

Kiểm tra xem trình duyệt của bạn hiện có đang sử dụng phông chữ Tiếng Nhật không

Một ký tự trông khác biệt rõ rệt giữa phông chữ Tiếng Nhật và tiếng Trung là [直](https://jisho.org/search/%E7%9B%B4%20%23kanji) được sử dụng trong từ [直す](https://jpdb.io/search?q=%E7%9B%B4%E3%81%99) (naosu) nghĩa là chữa bệnh, chữa lành, sửa chữa.

![](img/font2.png)
_Naosu in a Chinese font (DengXian)_

![](img/font3.png)
_Naosu in a Japanese font (IPAex Gothic)_

Nếu 直 của bạn trông giống như hình ảnh thứ hai, thì bạn đang dùng font Tiếng Nhật, nếu không thì nhớ đổi phông chữ nha.

## Windows 10

++win+i++ để mở **Settings** > **Apps** > **Optional features** > **Add a feature** > Search **"Japanese supplemental fonts"** và **Install**  

??? tip "Cho người dùng nâng cao: Powershell"
	Tải phông chữ thông qua **Windows Powershell (Administrator)**:
	```powershell
	Get-WindowsCapability -Online -Name Language.Fonts.Jpan~~~und-JPAN* | Add-WindowsCapability -Online
	```  
	Không cần khởi động lại máy.
??? question "Also have Chinese supplemental fonts already installed?"
	You will need to set your locale to Japanese (Japan).
	!!! abstract "Setting Japanese locale"
		1. Open the Run dialog box by pressing ++windows+r++
		2. Type `intl.cpl` and press ++enter++
		3. Click on the *Administrative* tab, go to *Change system locale...* and select **Japanese (Japan)** and click OK.
		

Bây giờ nếu bạn đang sử dụng trình duyệt dựa trên Chrome (VD: Google Chrome, Brave), hãy chọn Menu :material-dots-vertical: > **Settings** > chọn **Appearance** ở bên trái > **Customize fonts**. Đây là nơi bạn cần đặt phông chữ của mình.

Phông chữ tiêu chuẩn: Meiryo UI

Phông chữ Serif: Yu Mincho

Phông chữ Sans-serif: Meiryo

Monospace: MS Gothic

Nếu bạn đang sử dụng Firefox thì nó đã được làm sẵn cho bạn

## macOS

Bạn chỉ cần thêm Tiếng Nhật làm ngôn ngữ trong Tùy chọn hệ thống.

 > System Preferences, sau đó chọn "Language & Region". Bấm vào "General", sau đó "Add a language" và chọn "Japanese 日本語"

## Linux

Cần có locale `ja_JP.UTF-8`. Nếu không thì bỏ dấu thăng ở dòng `#ja_JP.UTF-8 UTF-8` trong `/etc/locale.gen` và chạy:

```bash
sudo locale-gen
```

Bây giờ hãy cài đặt gói [noto-fonts-cjk](https://archlinux.org/packages/extra/any/noto-fonts-cjk/).


!!! info "Nhắc nhỏ"
    Phần còn lại của bài viết sẽ không được dịch nên bạn cần đọc ở trang gốc bằng Tiếng Anh