1. Giới thiệu dự án
Tên dự án: Ứng dụng trí tuệ nhân tạo trong thiết kế website portfolio cá nhân
Mục tiêu: Tạo giao diện UI/UX bằng sự hỗ trợ của AI 
Vai trò: Designer + chỉnh sửa + tối ưu kết quả AI
2. Công cụ AI đã sử dụng
ChatGPT (tạo ý tưởng + prompt + code HTML/CSS)
Canva
3. Ví dụ Prompt đã dùng
Prompt tạo layout UI:

Thiết kế một trang portfolio UI/UX hiện đại cho một sinh viên tên “Nguyễn Anh Thơ”, phong cách nữ tính, dễ thương, màu pastel (hồng + xanh dương gradient), bố cục gọn gàng, thân thiện.
Trang web gồm các section:
HERO: tên lớn “Nguyễn Anh Thơ”, tagline “UI/UX Designer tương lai | Đam mê thiết kế & sáng tạo”, nền gradient hồng xanh, cảm giác trẻ trung, nổi bật.
ABOUT ME: khối nội dung bo góc, nền trắng, mô tả ngắn về người học UI/UX và 3D, phong cách tối giản.
PROJECTS: 2 card dự án (UI App Design, 3D Character), mỗi card có tiêu đề, mô tả ngắn và vai trò, hiệu ứng hover nâng nhẹ.
GALLERY: lưới 3 hình project, card bo góc, shadow nhẹ, có caption bên dưới từng ảnh.
SKILLS: chia 2 cột, một bên kỹ năng (HTML, CSS, Photoshop, Illustrator, Blender), một bên mức độ đánh giá sao.
CONTACT: thông tin email, số điện thoại, nút “Liên hệ ngay” dạng button bo tròn màu hồng.
Phong cách UI:
Bo góc mềm (rounded corners)
Shadow nhẹ hiện đại
Hiệu ứng hover mượt
Typography dùng font Poppins
Responsive layout (desktop trước, mobile sau)
Cảm giác dễ thương nhưng vẫn chuyên nghiệp

Prompt tạo ảnh minh họa trên Canva:

Ảnh 1: Thiết kế website portfolio hiện đại, giao diện người dùng/trải nghiệm người dùng (UI/UX), bố cục gọn gàng và tối giản, nền trắng và xám nhạt, kiểu chữ trang nhã, bố cục dạng lưới, khoảng cách mượt mà, các phần tương tác (giới thiệu, dự án, liên hệ), thẻ hiệu ứng kính, đổ bóng tinh tế, thẩm mỹ công nghệ cao cấp, thiết kế web đáp ứng, mô hình kiểu Figma, độ phân giải 4K, chi tiết cực cao, giới thiệu nhà thiết kế chuyên nghiệp.
Ảnh 2: Thiết kế UI/UX ứng dụng di động phong cách dễ thương Gen Z, màu pastel nhẹ nhàng, icon vui nhộn, giao diện mềm mại bo tròn, sticker UI, phong cách, bố cục chat app và mạng xã hội, thiết kế hiện đại, Figma mockup, bố cục ngang 16:9, hiển thị toàn giao diện, 4k
Ảnh 3: Thiết kế UI/UX desktop cho phần mềm sáng tạo hoặc game studio, giao diện hiện đại, hiệu ứng neon nhẹ, bảng điều khiển, thư viện dự án, thanh công cụ bên trái, phong cách sci-fi nhưng gọn gàng, UI chuyên nghiệp như phần mềm Adobe hoặc game engine, bố cục ngang 16:9, full desktop screen, 4k

4. Quá trình chỉnh sửa kết quả AI
Thêm mục Gallery dưới mục Project
<!-- MY PROJECT GALLERY -->
<section>
    <h2>Các dự án của tôi 🖼️</h2>

    <div class="gallery">

        <div class="img-card">
            <img src="https://via.placeholder.com/400x250" alt="Project 1">
            <p>Dự án 1</p>
        </div>

        <div class="img-card">
            <img src="https://via.placeholder.com/400x250" alt="Project 2">
            <p>Dự án 2</p>
        </div>

        <div class="img-card">
            <img src="https://via.placeholder.com/400x250" alt="Project 3">
            <p>Dự án 3</p>
        </div>

    </div>
</section>

5. Ý tưởng thiết kế tổng thể
Phong cách: Đơn giản, dễ thương
Màu chủ đạo: Hồng, xanh da trời, trắng
Bố cục: Đối xứng

