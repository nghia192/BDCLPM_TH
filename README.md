# 🏦 Selenium Automation Testing - ParaBank

## 📌 Giới thiệu dự án
Dự án tự động hóa kiểm thử (Automation Test) cho hệ thống website ngân hàng trực tuyến ParaBank. Đây là đồ án môn học Bảo đảm chất lượng phần mềm, được thực hiện bởi nhóm sinh viên nhằm mục đích kiểm tra các chức năng cốt lõi của hệ thống ngân hàng.

🔗 **Website Test Target:** [ParaBank Demo](https://parabank.parasoft.com/parabank/index.htm)

## 🛠 Công nghệ & Kỹ thuật sử dụng
* **Ngôn ngữ lập trình:** C#
* **Công cụ Automation:** Selenium WebDriver
* **Test Framework:** NUnit
* **Design Pattern:** Page Object Model (POM)
* **Quản lý Test Data:** JSON / CSV / Excel

## 📁 Cấu trúc dự án (Page Object Model)
Dự án được tổ chức chặt chẽ theo mô hình POM, phân tách rõ ràng giữa giao diện, logic test và dữ liệu:

```text
Selenium_Project/
├── 📂 Pages/             # Chứa các class đại diện cho từng trang web (Locators & Actions)
│   ├── LoginPage.cs     
│   ├── TransferFundsPage.cs
│   └── RegisterPage.cs  
├── 📂 Tests/             # Chứa các Test Scripts gọi các method từ thư mục Pages
│   ├── LoginTests.cs    
│   └── TransferTests.cs 
├── 📂 Utilities/         # Chứa các file cấu hình và tiện ích dùng chung
│   └── DriverFactory.cs 
└── 📂 TestData/          # Chứa dữ liệu đầu vào cho các test case
    └── users.json
