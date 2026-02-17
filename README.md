# Day 1:

- work flow trigger khi nào :
  workflow được trigger theo điều kiện ở khối lệnh on. Các trường hợp trigger có khá nhiều nhưng được chia làm 3 nhóm:
  - Nhóm 1 liên quan đến code: ví dụ push code, pull rq vào 1 nhánh chỉ định, merge code
  - Nhóm 2 liên quan thời gian: schedule
  - Nhóm 3 thủ công: workflow_dispatch , workflow gọi đến nhau
  - Nhóm 4 release/tag: trigger khi có release, tag theo pattern quy định
    ...

- Runner là gì?:
  - Runner là máy ảo để thực thi các câu lệnh trong tệp cấu hình, có thể dùng loại github-hosted (mặc định) hoặc self host. Loại mặc định thì có giới hạn of course

- Nếu 1 step fail thì chuyện gì xảy ra?
  - Một workflow có thể gồm nhiều job các job chạy song song, mỗi job lại có thể gồm nhiều step
  - Khi 1 step fail thì jobs đó fail và cả workflow đó fail

- Log xem ở đâu?
  - Có thể xem log trực tiếp trên github repo
- YAML indent sai sẽ thế nào?
  - Yaml indent sai dẫn đến sai cú pháp

# Day 2

- Syntax github workflows : [workflow syntax](https://docs.github.com/en/actions/reference/workflows-and-actions/workflow-syntax)
- Events types: [Event Type](https://docs.github.com/en/actions/reference/workflows-and-actions/events-that-trigger-workflows)
- Official actions: [official actions](https://github.com/orgs/actions/repositories)
