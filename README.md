# traffic-light-detection
## Tập dữ liệu được sử dụng trong chương trình.
Mô hình sử dụng đầu vào là những hình ảnh về đèn giao thông gồm các hình ảnh được chú thích thủ công và bán tự động hỗn hợp được thu thập từ cả Udacity Simulator và ros bags được cung cấp để đào tạo.
Bộ dữ liệu bao gồm các hình ảnh đến từ 4 nguồn:
Bạn có thể tham chiếu đến [dataset](https://drive.google.com/drive/folders/1NXqHTnjVC1tPjAB5DajGc30uWk5VPy7C).

The udacity simulator:
![image](https://user-images.githubusercontent.com/122681319/228896815-ad819b84-4fc6-432b-9588-acfd391cfaae.png)

Tệp túi đào tạo có video về đèn giao thông do Udacity cung cấp dưới dạng đào tạo:
![image](https://user-images.githubusercontent.com/122681319/228896837-269334fb-a8c5-4475-9e60-eba80fb86416.png)

Tệp túi đèn giao thông chỉ có video về đèn giao thông, được ghi lại trên địa điểm thử nghiệm Carla:
![image](https://user-images.githubusercontent.com/122681319/228896899-2f93829e-8deb-46f2-8e08-121bd0208443.png)

Tệp loop bag có video về một vòng lặp hoàn chỉnh, được ghi lại trên trang web thử nghiệm Carla:
![image](https://user-images.githubusercontent.com/122681319/228896978-256bd963-76da-4d7a-b3f3-a77b0b51addd.png)

### Thống kê dữ liệu đèn giao thông

|       Dataset         | Samples | Training | Evaluation |
|:----------------------|:-------:|:--------:|-----------:|
|  Simulator            |  422    |    316   |    106     |
|  Carla Training       |  1411   |    1058  |    353     |
|  Carla Testing        |  254    |    N/A   |    N/A     |
|  Carla Extra          |  304    |    N/A   |    N/A     |
|  Sim + Carla          |  1833   |    1374  |    459     |
|  Sim + Carla + Extra  |  2137   |    1709  |    428     |

## Quy trình kiểm thử
Sử dụng mô hình SSD-MobileNet V2 cùng với [TensorFlow Object Detection API](https://github.com/TensorFlow/models/tree/master/research/object_detection).
![image](https://user-images.githubusercontent.com/122681319/228903409-b8d0cb20-b22f-4d2a-9b02-aed00ffaf88f.png)

## Chạy chương trình
Kết quả:

![image](https://user-images.githubusercontent.com/122681319/228903884-0b39b0ab-1717-41e2-b0ec-942b79541e0c.png)
![image](https://user-images.githubusercontent.com/122681319/228903935-faa1512a-4a84-4eb8-a877-274dc73d8d2c.png)

## Đánh giá mô hình
![image](https://user-images.githubusercontent.com/122681319/228908221-ab5575b9-bfac-4e1b-b25c-b7ffb7fe51f2.png)


