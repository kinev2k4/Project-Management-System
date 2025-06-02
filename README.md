# Project-Management-System

## Link to the doc details:
https://docs.google.com/document/d/1v8Hhvg7agoV_2iu6Pxr31Bn6ZDjXOrTPwgtXoPIujq0/edit?tab=t.0#heading=h.iflr7xhk0rfi

## Project Structure:
```plaintext
project-management-system/
│
├── public/
│   ├── index.html
│   └── favicon.ico
│
├── src/
│   ├── assets/                  // Chứa hình ảnh, CSS/SCSS, fonts,...
│   │   ├── images/
│   │   └── styles/
│   │       └── main.scss
│   │
│   ├── components/              // Các component giao diện dùng chung
│   │   ├── common/              // Component chung: Button, Input, Modal,...
│   │   │   ├── Button.jsx
│   │   │   └── Input.jsx
│   │   │
│   │   └── layout/              // Layout dùng chung: Header, Sidebar, Footer,...
│   │       ├── Header.jsx
│   │       ├── Sidebar.jsx
│   │       └── Footer.jsx
│   │
│   ├── contexts/                // Context API cho trạng thái chung (auth, project, v.v.)
│   │   ├── AuthContext.jsx
│   │   └── ProjectContext.jsx
│   │
│   ├── hooks/                   // Các custom hook
│   │   ├── useAuth.js
│   │   └── useProject.js
│   │
│   ├── pages/                   // Các trang chính của ứng dụng
│   │   ├── Leader/              // Trang của Leader (Admin)
│   │   │   ├── StaffManagement.jsx         // LD-ADM01: Quản lý nhân viên
│   │   │   ├── ProjectManagement.jsx       // LD-ADM02: Quản lý dự án
│   │   │   ├── TaskManagement.jsx          // LD-ADM03: Quản lý nhiệm vụ
│   │   │   ├── ResourceManagement.jsx      // LD-ADM04: Quản lý tài nguyên
│   │   │   ├── NotificationManagement.jsx  // LD-ADM05: Quản lý thông báo
│   │   │   ├── SupportManagement.jsx       // LD-ADM06: Quản lý hỗ trợ
│   │   │   ├── SecurityManagement.jsx      // LD-ADM07: Quản lý bảo mật
│   │   │   ├── ProjectProgress.jsx         // LD-ADM08: Theo dõi tiến độ dự án
│   │   │   ├── ProjectMemberManagement.jsx // LD-ADM09: Quản lý thành viên dự án
│   │   │   └── ProjectTimeline.jsx         // LD-ADM10: Quản lý khung thời gian dự án
│   │   │
│   │   └── Staff/               // Trang của Staff
│   │       ├── Registration.jsx            // ST-REG01: Trang đăng ký tài khoản
│   │       ├── Login.jsx                   // ST-LOG01: Trang đăng nhập
│   │       ├── ProjectCreation.jsx         // ST-PRJ01: Tạo dự án mới
│   │       ├── ProjectManagement.jsx       // ST-PRJ02: Quản lý dự án đã tạo
│   │       ├── TaskManagement.jsx          // ST-PRJ03: Quản lý nhiệm vụ
│   │       ├── ResourceManagement.jsx      // ST-PRJ04: Quản lý tài nguyên dự án
│   │       ├── ProjectProgress.jsx         // ST-PRJ05: Theo dõi tiến độ dự án (Gantt, Kanban)
│   │       ├── MemberManagement.jsx        // ST-PRJ06: Quản lý thành viên dự án
│   │       ├── TeamCommunication.jsx       // ST-PRJ07: Giao tiếp nhóm (chat, video call,…)
│   │       ├── AlertSettings.jsx           // ST-ALRT01: Cài đặt cảnh báo
│   │       ├── ProjectReport.jsx           // ST-RPT01: Báo cáo dự án
│   │       ├── Support.jsx                 // ST-SPT01: Yêu cầu hỗ trợ
│   │       └── AccountManagement.jsx       // ST-ACC01: Quản lý tài khoản cá nhân
│   │
│   ├── routes/                  // Định nghĩa các route sử dụng react-router-dom hoặc tương tự
│   │   ├── AppRoutes.jsx
│   │   └── PrivateRoute.jsx
│   │
│   ├── services/                // Các dịch vụ kết nối API, xử lý logic nghiệp vụ
│   │   ├── api.js               // Cấu hình axios hoặc fetch API
│   │   ├── authService.js
│   │   ├── projectService.js
│   │   ├── taskService.js
│   │   └── notificationService.js
│   │
│   ├── utils/                   // Các hàm tiện ích (format ngày tháng, validate,…)
│   │   ├── formatDate.js
│   │   └── validation.js
│   │
│   ├── store/                   // Nếu sử dụng Redux: actions, reducers, store,...
│   │   ├── actions/
│   │   │   ├── authActions.js
│   │   │   └── projectActions.js
│   │   ├── reducers/
│   │   │   ├── authReducer.js
│   │   │   └── projectReducer.js
│   │   └── store.js
│   │
│   ├── App.jsx                  // File chính của ứng dụng
│   └── index.jsx                // Entry point, render App vào DOM
│
├── package.json
├── README.md
└── .gitignore
```
