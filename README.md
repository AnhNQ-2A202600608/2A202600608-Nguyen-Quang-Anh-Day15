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
* **Track chọn:** `T2 AI Infrastructure`
  * **Vì:** Đây là hướng đi phù hợp nhất với thế mạnh và định hướng phát triển của tôi. Tôi đã có kinh nghiệm thực tế qua các bài Lab trong việc thiết kế data pipeline, viết quy tắc làm sạch dữ liệu (cleaning rules) và validate schema tự động bằng Pydantic ở Day 10. Ngoài ra, việc thiết lập Async Runner để tối ưu hóa hiệu năng, kiểm soát Rate Limits và xây dựng cơ chế Offline Fallback cho AI Evaluation Factory ở Day 14 cũng củng cố năng lực của tôi trong việc vận hành và đảm bảo hệ thống AI chạy ổn định. Tôi muốn tập trung phát triển sâu vào MLOps, thiết kế hạ tầng dữ liệu và tối ưu hóa deployment/monitoring.
* **Track cân nhắc nhưng KHÔNG chọn (hoặc xếp làm ưu tiên thứ hai) + lý lẽ mạnh nhất cho nó:**
  * `T3 AI Applications Building`: Tôi đã cân nhắc rất nhiều về track này vì tôi rất thích lập trình các ứng dụng AI cụ thể như Chatbot, RAG, Agentic workflow và phát triển UI/UX Streamlit. Tuy nhiên, tôi nhận thấy rằng một hệ thống AI muốn chạy tốt và tin cậy thì hạ tầng dữ liệu và khả năng vận hành hệ thống bên dưới (AI Infrastructure/MLOps) mới là nền móng quan trọng nhất cần được ưu tiên hàng đầu.
* **Dấu hiệu sẽ khiến mình xem lại lựa chọn:**
  * Nếu trong tương lai công việc vận hành hạ tầng trở nên quá tự động hóa và bão hòa, hoặc khi tôi thấy bản thân có nhu cầu trực tiếp thiết kế các giải pháp ứng dụng AI tương tác trực tiếp với người dùng cuối nhiều hơn là tối ưu hệ thống phía sau.



### ◽ ĐỊNH HƯỚNG & CHUẨN BỊ (ghi mở – có gì ghi nấy)
* **Định hướng tiếp theo · những thứ cần chuẩn bị · plan nếu có · câu hỏi còn mở:**
  * **Định hướng tiếp theo:** Nắm vững các mô hình Agentic RAG phức tạp hơn (Multi-Agent Systems) và cách tích hợp chúng vào môi trường cloud-native.
  * **Chuẩn bị:** Nghiên cứu tài liệu của LangGraph và thực hành xây dựng các supervisor agent; tham gia các thử thách bảo mật ứng dụng LLM.
  * **Plan:** Xây dựng một dự án cá nhân áp dụng đầy đủ Agentic RAG với Multi-Agent Supervisor, Guardrails, Semantic Cache và publish kết quả benchmark lên GitHub.
  * **Câu hỏi còn mở:** Làm sao để dung hòa tối ưu giữa độ trễ (perceived latency) của user khi gọi Multi-Agent và độ chính xác của câu trả lời trong môi trường sản xuất thực tế?
