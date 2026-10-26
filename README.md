# trungkienhelpme

Plugin hướng dẫn xây và nhân bản kênh infographic. Phiên bản 2.0.0.

## Nội dung

Giữ nguyên từng byte của cả 9 tệp từ nhan-ban-kenh-skill-v2.0.0.zip: SKILL.md, references, templates và checklists. Chỉ bổ sung manifest, cấu hình marketplace và tài liệu cài đặt ở ngoài thư mục skill.

## Cài đặt trong ứng dụng hỗ trợ marketplace

Kho này là repo marketplace theo định dạng OpenAI, có danh mục tại `.agents/plugins/marketplace.json` và plugin tại `plugins/trungkienhelpme`.

Với Codex CLI có hỗ trợ lệnh plugin, thêm địa chỉ GitHub của kho này:

```bash
codex plugin marketplace add <URL_GITHUB_CUA_KHO_NAY>
```

Sau khi thêm marketplace, mở ChatGPT desktop, chọn nguồn trungkienhelpme-marketplace trong Plugins và cài trungkienhelpme. Thay phần trong dấu <> bằng URL GitHub thật sau khi kho được đăng. Nếu phiên bản CLI chưa hỗ trợ lệnh này, kiểm tra `codex plugin --help` và cập nhật ứng dụng.

Trong ChatGPT Workspace, quản trị viên có thể nhập marketplace từ GitHub thông qua phần quản lý Plugins. Quyền cài đặt phụ thuộc cấu hình Workspace.

Đưa mã nguồn lên GitHub không tự xuất bản plugin lên danh mục công khai của ChatGPT và không đảm bảo mọi tài khoản ChatGPT web cá nhân đều có thể cài trực tiếp bằng link kho.

## Sử dụng

Sau khi cài, mở chat mới, chọn plugin trungkienhelpme và nhập:

> Giúp tôi xây một kênh infographic mới. Hãy hướng dẫn từng bước.

Hoặc:

> Tôi muốn xây kênh infographic về mẹ bỉm, đăng Facebook, mục tiêu chia sẻ kiến thức và sau này làm affiliate.

## Cập nhật

Cập nhật mã nguồn trong kho rồi tăng phiên bản plugin khi phát hành. Người dùng cập nhật marketplace theo ứng dụng đang sử dụng. Kho GitHub này và bản plugin riêng tư đã tạo trước đó là hai nguồn phân phối riêng; thay đổi trong kho không tự cập nhật bản riêng tư.

## Tài liệu chính thức

- https://developers.openai.com/plugins/build/plugins
- https://learn.chatgpt.com/docs/plugins

## Tải thủ công lên GitHub

Tạo kho Public tên trungkienhelpme. Giải nén gói rồi tải README.md, marketplace.json, SOURCE_SHA256.json và thư mục plugins lên gốc kho. Nên đưa cả thư mục .agents lên bằng Git hoặc GitHub Desktop vì trình tải qua web có thể bỏ qua thư mục ẩn. Không chỉ tải tệp ZIP lên kho.

Nếu kho thiếu .agents, nhập URL trực tiếp của marketplace.json khi ứng dụng hỗ trợ nguồn marketplace bằng URL. Cấu hình chuẩn khuyến nghị vẫn là .agents/plugins/marketplace.json.
