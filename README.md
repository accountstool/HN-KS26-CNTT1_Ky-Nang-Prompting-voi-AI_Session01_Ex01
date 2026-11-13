
## Phần 1. Bóc tách 2 điểm sai trong báo cáo của Nam

- Sai lầm 1, cho rằng "AI bị hỏng phần mềm hoặc máy chủ bị lỗi": không có gì hỏng cả, đây là hành vi đúng bản chất của LLM. Theo Lesson 01, LLM hoạt động theo cơ chế Next Token Prediction, đọc câu hỏi rồi đoán token tiếp theo dựa trên xác suất các chuỗi ký tự gặp trong giai đoạn Pre-training, phép cộng với nó chỉ là một chuỗi ký tự cần đoán tiếp, không phải bài toán để thực thi thuật toán
- Sai lầm 2, cho rằng "hàng trăm tỷ tham số chắc chắn phải có bộ vi xử lý tính chính xác 100%": tham số là trọng số dùng để tính xác suất từ tiếp theo, không phải đơn vị tính toán số học của máy tính, tham số nhiều chỉ giúp dự đoán từ khéo hơn chứ không biến LLM thành máy tính bỏ túi

## Phần 2. Prompt chuẩn kích hoạt công cụ tính toán

```text
Hãy luôn dùng công cụ tính toán Python cho mọi câu hỏi liên quan tới số học, tuyệt đối không tự nhẩm kết quả trong đầu.
Chạy code Python để tính: 15480 + 28750
Chỉ trả về kết quả chính xác do code thực thi, kèm một dòng giải thích ngắn.
```
