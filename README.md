# 2A202600608-Nguyen-Quang-Anh-Day15

## TRACK DECISION MEMO – Day 15

* **Họ tên:** Nguyễn Quang Anh
* **Pathway:** C (Lớp C401)

---

### ◽ ĐỊNH HƯỚNG – vài job/role mình hướng tới + kỹ năng mỗi job đòi hỏi (từ JD thật + report)
* **Job:** AI Engineer / GenAI Developer $\rightarrow$ **kỹ năng cần:** Prompt engineering, RAG, LLM orchestration (LangChain/LangGraph), evaluation frameworks (Ragas/DeepEval), python/asyncio.
* **Job:** MLOps / LLMOps Engineer $\rightarrow$ **kỹ năng cần:** CI/CD pipeline automation, LLM serving/inference optimization, vector databases, Docker, model deployment & monitoring.
* **Job:** AI Product Developer $\rightarrow$ **kỹ năng cần:** Streamlit UI/UX development, telemetry tracking (Token, Cost, Latency), API integration, rapid prototyping.

### ◽ ĐỐI CHIẾU BẢN THÂN – từ Phase 1
* **Những việc mình đã làm được (liệt kê tự do, không giới hạn):**
  * Thiết kế và phát triển **Multi-Judge Consensus Engine** (`engine/llm_judge.py`) gọi song song các mô hình Judge LLM độc lập để đánh giá tự động, tính độ đồng thuận và giải quyết xung đột điểm số.
  * Xây dựng **Async Runner** (`engine/runner.py`) dùng `asyncio.Semaphore` để chạy benchmark song song tốc độ cao và kiểm soát tốt Rate Limits.
  * Phát triển giao diện **Streamlit UI** chuyên nghiệp, tích hợp CSS/JS injection để tối ưu giao diện premium, hiển thị đo lường **telemetry thời gian thực** (Tokens, Cost, Steps, Latency).
  * Xây dựng quy trình làm sạch dữ liệu (**cleaning rules**) và kiểm định chất lượng tự động sử dụng **Pydantic Model schema validation** trước khi nạp vào vector database.
  * Thiết kế bộ dữ liệu **Golden Dataset** (50+ test cases) bao phủ factual, multi-document, edge cases, out-of-context, và adversarial prompts.
  * Cài đặt cơ chế **Offline Fallback Mode** giúp pipeline CI/CD chạy ổn định 100% không bị ảnh hưởng bởi lỗi mạng hay hạn ngạch API trả phí.
* **Loại công việc cho mình năng lượng, muốn làm tiếp:**
  * Lập trình các hệ thống Agentic AI phức tạp, thiết kế giải thuật điều phối (orchestration) và tối ưu hóa hiệu năng/tốc độ xử lý song song (asyncio).
  * Xây dựng UI/UX cho AI application, trực quan hóa metrics và telemetry thu thập từ mô hình.
  * Thiết lập và tối ưu hóa hệ thống đánh giá tự động (AI Evaluation Factory) và các luồng CI/CD cho AI.

### ◽ KỸ NĂNG MÌNH ĐỊNH PHÁT TRIỂN TỚI
* **Các kỹ năng:** AI Orchestration Frameworks nâng cao (LangGraph, AutoGen), LLMOps & Guardrails (NeMo Guardrails, Llama Guard), Vector Search Optimization (Cohere Rerank, BGE-Reranker, Hybrid Search).
* **Gap lớn nhất + thứ mình sẽ build để cho thấy tiến bộ:**
  * **Gap:** Kinh nghiệm thực tế trong việc deploy, scale các ứng dụng LLM trong môi trường enterprise lớn và xử lý các vấn đề bảo mật an toàn thông tin (Adversarial attacks / Prompt injection) một cách toàn diện.
  * **Thứ sẽ build:** Một hệ thống RAG nâng cao có tích hợp bộ lọc ngữ nghĩa (Guardrails), cơ chế Reranking (Cohere Reranker), Semantic Cache (Redis) và giám sát chất lượng liên tục (Continuous Monitoring).

### ◽ QUYẾT ĐỊNH TRACK
* **Track chọn:** `T3 AI Engineering`
  * **Vì:** Đây là thế mạnh cốt lõi của tôi (đã thể hiện qua việc tự tay lập trình Agentic RAG, Multi-Judge consensus engine, async runner, và tối ưu hóa code Python). Tôi đam mê phát triển logic ứng dụng thông minh và giải quyết các bài toán kỹ thuật thực tế hơn là tập trung thuần vào hạ tầng dữ liệu (Data & Infra) hay quản lý sản phẩm (AI Product).
* **Track cân nhắc nhưng KHÔNG chọn + lý lẽ mạnh nhất cho nó:**
  * `T2 Data & Infrastructure`: Dù tôi đã làm việc tốt với Data Pipeline (clean data, validate schema bằng Pydantic), việc tập trung hoàn toàn vào hạ tầng lưu trữ và quản lý data pipelines có phần khô khan, ít cơ hội được trực tiếp phát triển và tối ưu các mô hình Agentic AI/LLM năng động.
* **Dấu hiệu sẽ khiến mình xem lại lựa chọn:**
  * Nếu thị trường dịch chuyển mạnh sang hướng auto-train/fine-tune tự động mà không cần nhiều đến lập trình logic Agent, hoặc nếu tôi phát hiện bản thân có cơ hội và khả năng tối ưu hóa tài nguyên phần cứng lớn ở mức infrastructure tốt hơn.

### ◽ ĐỊNH HƯỚNG & CHUẨN BỊ (ghi mở – có gì ghi nấy)
* **Định hướng tiếp theo · những thứ cần chuẩn bị · plan nếu có · câu hỏi còn mở:**
  * **Định hướng tiếp theo:** Nắm vững các mô hình Agentic RAG phức tạp hơn (Multi-Agent Systems) và cách tích hợp chúng vào môi trường cloud-native.
  * **Chuẩn bị:** Nghiên cứu tài liệu của LangGraph và thực hành xây dựng các supervisor agent; tham gia các thử thách bảo mật ứng dụng LLM.
  * **Plan:** Xây dựng một dự án cá nhân áp dụng đầy đủ Agentic RAG với Multi-Agent Supervisor, Guardrails, Semantic Cache và publish kết quả benchmark lên GitHub.
  * **Câu hỏi còn mở:** Làm sao để dung hòa tối ưu giữa độ trễ (perceived latency) của user khi gọi Multi-Agent và độ chính xác của câu trả lời trong môi trường sản xuất thực tế?
