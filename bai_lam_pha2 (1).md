# BÀI LÀM PHA 2 – HACKATHON 02

  

-  **Mã đề:** 04

-  **Họ tên:** Nguyễn Hồng Quân

-  **Lớp:** CNTT2

-  **Link repository Pha2:**https://github.com/hcuanne/HN-KS26-CNTT2_PromptAI_H02_Pha1-Pha2

-  **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):** ChatGPT

  

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

  

## 4.2. Trích xuất tin nhắn đặt vé xe ra JSON

  

**KET QUA AI**

  

```text

[  
{  
"ma_tuyen": "SGDL",  
"ngay_di": "2026-12-22",  
"ve_nguoi_lon": 2,  
"ve_tre_em": 1,  
"loai_cho": "giuong",  
"ghi_chu": null  
},  
{  
"ma_tuyen": "SGNT",  
"ngay_di": "2027-01-02",  
"ve_nguoi_lon": 3,  
"ve_tre_em": 0,  
"loai_cho": null,  
"ghi_chu": "Một người đang mang thai 6 tháng"  
},  
{  
"ma_tuyen": "SGCT",  
"ngay_di": null,  
"ve_nguoi_lon": 4,  
"ve_tre_em": 0,  
"loai_cho": "ghe",  
"ghi_chu": "Bà nội đi xe lăn"  
}  
]
```

  

**Link trò chuyện:** https://chatgpt.com/share/6b079cb2-4dcc-83ec-87af-85fce8127d08

  

## 4.3. Báo giá bằng Chain-of-Thought

  

**KET QUA AI**

  

```text

B1. Tiền người lớn

8 × 320.000 = 2.560.000 đồng.

B2. Tiền trẻ em 

-   Trẻ từ 5 đến 10 tuổi (6, 7 và 9 tuổi): 3 × 320.000 × 75% = 720.000 đồng.
    
-   Trẻ dưới 5 tuổi (2 tuổi): 1 × 0 = 0 đồng.
    
-   Tổng tiền trẻ em: 720.000 + 0 = 720.000 đồng.
    

B3. Tổng tiền vé trước giảm

2.560.000 + 720.000 = 3.280.000 đồng.

B4. Mức giảm giá đoàn và tiền vé sau giảm

-   Đoàn có 8 người lớn nên được giảm 5%.
    
-   Tiền giảm: 3.280.000 × 5% = 164.000 đồng.
    
-   Tiền vé sau giảm: 3.280.000 − 164.000 = 3.116.000 đồng.
    

B5. Tiền phụ thu (không giảm)

2 × 100.000 = 200.000 đồng.

B6. Tổng tiền cần thanh toán

3.116.000 + 200.000 = 3.316.000 đồng.

[RESULT: 3.316.000 đồng]
```

  

**Link trò chuyện:**https://chatgpt.com/share/6b079e6b-3e44-83ec-bda5-a25ffbfe135e
  

### b) Kiểm tra kết quả AI

  

AI tính **đúng** cả 6 bước theo bảng giá và quy tắc. Tổng tiền đúng là **3.316.000 đồng**.
  

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

  

**KET QUA AI**

  

```text

{  
"loai_su_co": "sai_loai_xe",  
"so_khach": 3,  
"so_chang_bi_doi": 2,  
"tom_tat": "Nhà xe đổi giường nằm sang ghế ngồi ở cả hai chặng, ảnh hưởng 3 khách."  
}
```

  

**Link trò chuyện:**https://chatgpt.com/share/6b079ea7-aad8-83ec-8e75-20d55ce16c63

  

## 4.5. Prompt chấm bài theo Rubric

  

**KET QUA AI**

  

```text

| Tiêu chí | Điểm | Minh chứng | Đề xuất sửa |
|---|---|---|---|
| Đúng thông tin (50%) | 0/5 | Sai giá vé 350.000đ và chính sách đổi vé miễn phí trước 12 tiếng. | Giá vé 380.000đ/vé. Phí đổi vé 20%, tương đương 76.000đ/vé. |
| Đầy đủ (30%) | 2/3 | Trả lời cả hai câu hỏi nhưng chưa yêu cầu ngày đi và số lượng vé. | Mời khách cung cấp ngày khởi hành và số lượng vé để đặt chỗ. |
| Giọng điệu (20%) | 1/2 | Sử dụng từ ngữ suồng sã như “xe xịn lắm luôn”, “đổi free nha chị”. | Sử dụng ngôn ngữ lịch sự, chuyên nghiệp. |
| **Tổng điểm** | **3/10** | | |

**Tổng điểm: 3/10.**
```

  

**Link trò chuyện:**https://chatgpt.com/share/6b079f1c-0e28-83ec-a994-ab5b69593d12
