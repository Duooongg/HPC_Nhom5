HPC_Nhom5
TÍNH TOÁN HIỆU NĂNG CAO VỚI THUẬT TOÁN QAOA

ỨNG DỤNG GIẢI BÀI TOÁN MAXCUT**

Đồ án Bài tập lớn môn Tính toán Hiệu năng Cao (HPC)

Nhóm sinh viên: Nhóm 

Giảng viên hướng dẫn: TS. Hà Mạnh Đào
Đơn vị: Trường Công nghệ Thông tin và Truyền thông – Đại học Công nghiệp Hà Nội

1. Giới thiệu đề tài

Trong những năm gần đây, tính toán lượng tử đã nổi lên như một hướng tiếp cận đầy tiềm năng nhằm giải quyết các bài toán tối ưu phức tạp mà các phương pháp tính toán cổ điển gặp nhiều hạn chế về thời gian và tài nguyên. Đặc biệt, các thuật toán lượng tử lai (hybrid quantum–classical) cho phép kết hợp ưu điểm của mô hình lượng tử và tính toán cổ điển, mở ra khả năng ứng dụng thực tiễn trong bối cảnh phần cứng lượng tử còn nhiều giới hạn.

Trong số các thuật toán lượng tử lai, Quantum Approximate Optimization Algorithm (QAOA) được xem là một trong những phương pháp tiêu biểu để giải các bài toán tối ưu tổ hợp thuộc lớp NP-hard. QAOA tận dụng mạch lượng tử tham số kết hợp với bộ tối ưu cổ điển nhằm tìm nghiệm gần tối ưu trong không gian nghiệm lớn.

Bài toán MaxCut là một bài toán tối ưu đồ thị quan trọng, có nhiều ứng dụng trong phân chia mạng, thiết kế mạch, phân cụm dữ liệu và mô hình hóa các hệ vật lý. Tuy nhiên, khi kích thước đồ thị tăng lên, việc tìm nghiệm tối ưu bằng các phương pháp cổ điển trở nên tốn kém về mặt tính toán. Do đó, việc nghiên cứu và đánh giá hiệu năng của QAOA trong việc giải bài toán MaxCut cho các đồ thị kích thước vừa là một hướng tiếp cận hiện đại, phù hợp với lĩnh vực tính toán hiệu năng cao (HPC).

2. Mục tiêu nghiên cứu
2.1. Nghiên cứu lý thuyết

Tìm hiểu tổng quan về tính toán lượng tử và mô hình thuật toán lượng tử lai.

Nghiên cứu nguyên lý hoạt động của thuật toán QAOA, bao gồm:

Cost Hamiltonian và Mixing Hamiltonian.

Vai trò của các tham số 
𝛾, 𝛽 và số lớp 𝑝
Phân tích bài toán MaxCut dưới góc độ tối ưu hóa và biểu diễn Hamiltonian.

Nghiên cứu các phương pháp cổ điển giải MaxCut, đặc biệt là:

Thuật toán heuristic (Greedy, Local Search).

Thuật toán xấp xỉ Goemans–Williamson (GW).

2.2. Triển khai và đánh giá thực nghiệm

Triển khai thuật toán QAOA giải bài toán MaxCut trên nền tảng mô phỏng lượng tử.

Đánh giá hiệu năng và chất lượng nghiệm của QAOA với các kích thước đồ thị từ 20 đến 50 đỉnh.

So sánh kết quả QAOA với các phương pháp cổ điển thông qua các tiêu chí:

Giá trị MaxCut đạt được.

Tỷ lệ xấp xỉ (approximation ratio).

Thời gian thực thi và khả năng mở rộng.

3. Đặc điểm kỹ thuật
3.1. Mô hình và thuật toán

Thuật toán chính: Quantum Approximate Optimization Algorithm (QAOA).

Bài toán ứng dụng: MaxCut trên đồ thị ngẫu nhiên Erdos–Renyi.

Phương pháp so sánh:

Thuật toán heuristic cổ điển (Greedy / Local Search).

Thuật toán xấp xỉ Goemans–Williamson (GW).

3.2. Môi trường thực nghiệm

Ngôn ngữ lập trình: Python.

Thư viện và công cụ:

Qiskit (qiskit, qiskit-aer, qiskit-optimization).

NetworkX (xây dựng và xử lý đồ thị).

NumPy, Matplotlib (xử lý số liệu và trực quan hóa).

Môi trường chạy: Google Colab / máy tính cá nhân.

Phần cứng: CPU đa lõi, khai thác mô hình lai lượng tử – cổ điển (quantum–classical hybrid).

3.3. Định hướng HPC

Mặc dù thuật toán QAOA được mô phỏng trên phần cứng cổ điển, bài toán vẫn mang đặc trưng của tính toán hiệu năng cao do:

Không gian nghiệm tăng theo cấp số mũ theo số đỉnh.

Chi phí tính toán tăng theo số lớp QAOA và số vòng lặp tối ưu.

Khả năng mở rộng và song song hóa trong các thành phần tối ưu cổ điển.

Việc đánh giá QAOA trong bối cảnh này giúp làm rõ tiềm năng của các thuật toán lượng tử trong tương lai khi được triển khai trên phần cứng lượng tử thực hoặc các hệ thống HPC lai.
