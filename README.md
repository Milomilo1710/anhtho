1. Giới thiệu dự án
Tên dự án: Ứng dụng trí tuệ nhân tạo trong thiết kế website portfolio cá nhân
Mục tiêu: Tạo giao diện UI/UX bằng sự hỗ trợ của AI 
Vai trò: Designer + chỉnh sửa + tối ưu kết quả AI
2. Công cụ AI đã sử dụng
ChatGPT (tạo ý tưởng + prompt + code HTML/CSS)
Canva
3. Ví dụ Prompt đã dùng


Hãy tạo một website portfolio cá nhân hiện đại dành cho một UI/UX Designer kết hợp 3D Designer với phong cách **glassmorphism**, màu chủ đạo là gradient xanh da trời  và hồng . Thiết kế cần mang cảm giác sáng tạo, mềm mại nhưng vẫn chuyên nghiệp, tập trung vào trải nghiệm người dùng (UX) và tính thẩm mỹ (UI). 

Yêu cầu bố cục gồm các phần sau:

1. Hero Section 

 Layout chia 2 cột: bên trái là nội dung, bên phải là ảnh chân dung (dạng dọc, bo góc, có viền gradient) 
Tiêu đề lớn (tên cá nhân) 
Subtitle: “UI/UX Designer • 3D Designer” 
Đoạn mô tả mang tính storytelling (thiết kế dựa trên cảm xúc người dùng, kết hợp logic và nghệ thuật)
Nút CTA: “Let’s Work Together”
Chiều cao full màn hình (100vh)

2. **About Section**

 Chia 2 card dạng glass (bo góc, blur nền)
Card 1: Giới thiệu bản thân (tư duy thiết kế, đam mê UX + 3D)
Card 2: Định hướng (trở thành Product Designer, tập trung vào giá trị sản phẩm và người dùng)
Hover effect nhẹ (nhấc card lên)

3. Strengths Section 

Danh sách các điểm mạnh dạng hàng ngang (glass card)
Bao gồm: UI/UX Design, 3D Modeling, Wireframe, Tools
Hiển thị dạng label + mô tả ngắn
Hover scale nhẹ

4. Projects Section

Tiêu đề chính ở giữa
Chia làm 2 nhóm:

  a. UI/UX:

  * 3 ảnh dọc đặt cạnh nhau
  * Hiệu ứng hover zoom ảnh

  b. 3D:

  * Layout sáng tạo:
    + 2 ảnh ngang phía trên
    + 1 ảnh lớn phía dưới (center)
  * Các card có bo góc + glass effect

5. **Skills Section**

* Thanh progress bar có animation load từ trái sang phải
* Các kỹ năng:

  * UI/UX Design (90%)
    + 3D Modeling (85%)
   Prototype (80%) 
 Màu thanh là gradient xanh → hồng 

6. Contact Section 

 Form gồm: Name, Email, Message 
Nút gửi dạng button bo tròn 
Layout căn giữa, đặt trong card glass 

7. Footer

Nội dung đơn giản (© Portfolio Designer) 

Yêu cầu kỹ thuật:

Sử dụng HTML + CSS thuần 
Font: Poppins (Google Fonts) 
Sử dụng hiệu ứng: 

  Glassmorphism (blur + border nhẹ) 
  Hover animation (scale, translate) 
  Image zoom 
  Progress bar animation 
 Responsive cơ bản 
 Code rõ ràng, dễ chỉnh sửa 

Mục tiêu tổng thể:
Tạo một portfolio mang đậm dấu ấn cá nhân, thể hiện sự kết hợp giữa trải nghiệm người dùng (UX)** và thẩm mỹ thị giác (UI + 3D), tạo cảm giác chuyên nghiệp nhưng vẫn sáng tạo và có “cảm xúc”. 

4. Quá trình chỉnh sửa kết quả AI:
a)Chỉnh sửa bố cục:

-Code trước đó:

-PHẦN HTML:

	<section class="projects-section">

    <h2 class="project-title">UI/UX</h2>

    <!-- HÀNG TRÊN -->
    <div class="projects-row top-row">
        ...
    </div>

    <!-- HÀNG DƯỚI -->
    <div class="projects-row bottom-row">
        ...
    </div>

</section>

-PHẦN CSS:

	.project-title{...}
.projects-row{...}
.vertical{...}
.horizontal{...}
.bottom-row .project-card:nth-child(2){...}
.bottom-row .project-card:nth-child(3){...}

-Code sau khi sửa:

-PHẦN HTML:

	<section class="projects-section">

    <!-- UI/UX -->
    <div class="project-block">
        <h2 class="project-label">UI/UX</h2>

        <div class="projects-top">
            <div class="project-card vertical glass"><img src="YOUR_PROJECT_1"></div>
            <div class="project-card vertical glass"><img src="YOUR_PROJECT_2"></div>
            <div class="project-card vertical glass"><img src="YOUR_PROJECT_3"></div>
        </div>
    </div>

    <!-- 3D -->
    <div class="project-block">
        <h2 class="project-label">3D</h2>

        <div class="projects-3d">

            <!-- hàng trên -->
            <div class="row-top">
                <div class="project-card horizontal glass"><img src="YOUR_PROJECT_4"></div>
                <div class="project-card horizontal glass"><img src="YOUR_PROJECT_5"></div>
            </div>

            <!-- ảnh dưới -->
            <div class="row-bottom">
                <div class="project-card big glass"><img src="YOUR_PROJECT_6"></div>
            </div>

        </div>
    </div>

</section>


-PHẦN CSS:

	/* PROJECTS NEW */
.projects-section{
    max-width:1200px;
    margin:auto;
}

/* BLOCK */
.project-block{
    margin-bottom:80px;
}

/* TITLE LEFT */
.project-label{
    font-size:32px;
    margin-bottom:25px;
    text-align:left;
}

/* UI/UX */
.projects-top{
    display:flex;
    gap:30px;
}

/* ẢNH DỌC */
.vertical{
    width:30%;
    height:420px;
}

/* 3D LAYOUT */
.projects-3d{
    display:flex;
    flex-direction:column;
    gap:25px;
}

/* HÀNG TRÊN */
.row-top{
    display:flex;
    gap:30px;
}

/* ẢNH NGANG */
.horizontal{
    flex:1;
    height:220px;
}

/* HÀNG DƯỚI */
.row-bottom{
    display:flex;
    justify-content:center;
}

/* ẢNH TO DƯỚI */
.big{
    width:60%;
    height:260px;
}

/* CARD */
.project-card{
    overflow:hidden;
    border-radius:20px;
    transition:0.4s;
}

.project-card img{
    width:100%;
    height:100%;
    object-fit:cover;
    transition:0.4s;
}

.project-card:hover img{
    transform:scale(1.08);
}

b)Thêm các link hình ảnh dưới mục Project:

-Code trước đó:

ảnh đại diện:

	<div class="hero-img">
        <img src="YOUR_IMAGE_LINK ">

ảnh dự án UI/UX:

	<div class="projects-top">
            <div class="project-card vertical glass"><img src="YOUR_PROJECT_1"></div>
            <div class="project-card vertical glass"><img src="YOUR_PROJECT_2"></div>
            <div class="project-card vertical glass"><img src="YOUR_PROJECT_3"></div>
        </div>

ảnh dự án 3D:

	 <div class="projects-3d">

            <!-- hàng trên -->
            <div class="row-top">
                <div class="project-card horizontal glass"><img src="YOUR_PROJECT_4"></div>
                <div class="project-card horizontal glass"><img src="YOUR_PROJECT_5"></div>
            </div>

            <!-- ảnh dưới -->
            <div class="row-bottom">
                <div class="project-card big glass"><img src="YOUR_PROJECT_6"></div>
            </div>


-Code sau khi sửa:

ảnh đại diện:

	<div class="hero-img">
        <img src="https://github.com/Milomilo1710/anhtho/blob/main/avatar.jpg?raw=true">

ảnh dự án UI/UX:

	<div class="projects-top">
            <div class="project-card vertical glass"><img src="https://github.com/Milomilo1710/anhtho/blob/main/Home.jpg?raw=true"></div>
            <div class="project-card vertical glass"><img src="https://github.com/Milomilo1710/anhtho/blob/main/Menu.jpg?raw=true"></div>
            <div class="project-card vertical glass"><img src="https://github.com/Milomilo1710/anhtho/blob/main/chi%20ti%E1%BA%BFt%20s%E1%BA%A3n%20ph%E1%BA%A9m.jpg?raw=true"></div>
        </div>

ảnh dự án 3D:

	 <div class="projects-3d">

            <!-- hàng trên -->
            <div class="row-top">
                <div class="project-card horizontal glass"><img src="https://github.com/Milomilo1710/anhtho/blob/main/Screenshot%202026-04-07%20152345.png?raw=true"></div>
                <div class="project-card horizontal glass"><img src="https://github.com/Milomilo1710/anhtho/blob/main/Screenshot%202026-04-07%20152750.png?raw=true"></div>
            </div>

            <!-- ảnh dưới -->
            <div class="row-bottom">
                <div class="project-card big glass"><img src="https://github.com/Milomilo1710/anhtho/blob/main/Screenshot%202026-04-07%20153134.png?raw=true"></div>
            </div>

5. Ý tưởng thiết kế tổng thể

Phong cách: Đơn giản, dễ thương

Màu chủ đạo: Hồng, xanh da trời

Bố cục: Đối xứng, ảnh dự án được bố trí xen kẽ

6. Video quá trình:

https://drive.google.com/drive/folders/1N9OFolssSGAIEMByTt4OCvfBd6dkZCDb?usp=sharing
