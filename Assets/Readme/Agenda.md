# Agenda Phát Triển Game Week 3

## 1. Tìm Thêm 5 Characters Cho Game

- Nghiên cứu và chọn 5 nhân vật mới để thêm vào game.
- Tìm kiếm các nhân vật có phong cách và khả năng phù hợp với lối chơi của game.
- Đảm bảo rằng các nhân vật này được tối ưu hóa cho hiệu suất.

## 2. Gắn Animation Chạy (Run) Vào Cho 5 Characters Mới

- Gắn animation chạy mặc định vào từng nhân vật mới.
- Kiểm tra xem các animation có tương thích và hoạt động mượt mà trên các nhân vật.

## 3. Lần Lượt Gắn 3 Animation Chạy Khác Nhau Vào Animator

- Gắn ba animation chạy khác nhau vào hệ thống Animator của Unity.
- Thiết lập các transition (chuyển cảnh) giữa các animation để tạo sự linh hoạt cho các hành động của nhân vật.
- Kiểm tra tính đồng nhất giữa các animation trong quá trình chuyển tiếp.

## 4. Tìm Kiếm 2 Website Khác Ngoài Unity Store Cung Cấp Asset

- Tìm và đánh giá thêm 2 trang web cung cấp asset để làm phong phú nguồn tài nguyên cho dự án.
- Một số trang web có thể tham khảo bao gồm:
  - **CGTrader**: Chuyên cung cấp asset 3D.
  - **TurboSquid**: Một trang web uy tín với nhiều asset cho các dự án game và phim.
- Xem xét độ tương thích của các asset với Unity và dự án hiện tại.

### Open Game Art
### Kenney

## 5. Hỏi AI Cách Sử Dụng Nav Mesh Obstacle

- Tìm hiểu cách sử dụng **NavMesh Obstacle** để chặn đường hoặc tạo vật cản cho các nhân vật điều hướng (navigation) trong game.
- Xem xét cách thiết lập các thuộc tính như "carving" để nhân vật tránh hoặc phản ứng linh hoạt với vật cản.
- Kiểm tra và điều chỉnh hệ thống **NavMesh** cho phù hợp với các vật cản mới.

### Trong Unity, Nav Mesh Obstacle là một thành phần (component) được sử dụng để tạo ra các chướng ngại vật động ảnh hưởng đến quá trình tìm đường (pathfinding) của các agent (nhân vật hoặc đối tượng di chuyển) trên NavMesh. Khi một đối tượng có thành phần Nav Mesh Obstacle được đặt trong cảnh, nó sẽ chặn đường đi của agent hoặc khiến chúng phải đi vòng qua chướng ngại vật đó.

### Các Chế Độ Chính của Nav Mesh Obstacle
- Carve (Cắt)
Mô tả: Khi chế độ này được bật, Nav Mesh Obstacle sẽ cắt bỏ phần NavMesh nằm dưới chướng ngại vật, tạo ra một lỗ hổng trên NavMesh.
Ứng dụng: Phù hợp cho các chướng ngại vật tĩnh hoặc di chuyển chậm, như cửa mở hoặc các vật thể di chuyển nhẹ.
Ưu điểm: Agent sẽ tự động tìm đường đi xung quanh vùng bị cắt mà không cần cập nhật NavMesh thủ công.
- Non-Carving (Không Cắt)
Mô tả: Trong chế độ này, Nav Mesh Obstacle không cắt bỏ NavMesh. Thay vào đó, các agent sẽ nhận biết và điều chỉnh đường đi của mình để tránh chướng ngại vật mà không thay đổi NavMesh.
Ứng dụng: Thích hợp cho các chướng ngại vật di động hoặc khi bạn không muốn NavMesh thay đổi liên tục.
Ưu điểm: Tiết kiệm hiệu suất vì không cần cập nhật NavMesh liên tục khi chướng ngại vật di chuyển.
### Cách Sử Dụng Nav Mesh Obstacle
1. Thêm Nav Mesh Obstacle vào Đối Tượng:
Chọn đối tượng trong Hierarchy mà bạn muốn thêm chướng ngại vật.
Trong Inspector, nhấn "Add Component".
Tìm kiếm "Nav Mesh Obstacle" và thêm nó vào đối tượng.
2. Cấu Hình Các Thuộc Tính:
Shape (Hình dạng): Chọn hình dạng của chướng ngại vật (Box, Capsule, hoặc Mesh).
Size (Kích thước): Điều chỉnh kích thước phù hợp với đối tượng.
Carve: Bật hoặc tắt chế độ cắt tùy thuộc vào nhu cầu của bạn.
Movement (Di chuyển): Nếu chướng ngại vật di động, bạn có thể cấu hình các tùy chọn liên quan đến di chuyển.

### Kết Luận:
Nav Mesh Obstacle là một công cụ mạnh mẽ trong Unity giúp bạn quản lý các chướng ngại vật động, tạo ra môi trường linh hoạt và sống động cho các agent trong trò chơi. Bằng cách hiểu và sử dụng đúng các chế độ và thuộc tính của Nav Mesh Obstacle, bạn có thể tối ưu hóa quá trình tìm đường và nâng cao trải nghiệm người chơi.