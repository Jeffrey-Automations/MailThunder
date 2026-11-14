# 測試覆蓋度：MailThunder

測量日期：2026-10-28。數字來自這台 Windows 機器上的一次實測，不是估計，也不是只數檔案。

| 項目 | 內容 |
|---|---|
| 直譯器 | 3.11.9 |
| 直譯器說明 | 專案 .venv |
| 工具 | coverage 7.15.0，`coverage run --branch` |
| 測量範圍 | `je_mail_thunder` |
| 測試路徑 | `test` |
| 命令 | `python -m coverage run --branch --source=je_mail_thunder -m pytest test` |
| 敘述覆蓋 | 95.37%（3622 / 3798） |
| 分支覆蓋 | 94.19%（859 / 912） |
| 測試結果 | 689 passed, 3 warnings in 19.76s |
| 耗時 | 20.9 秒 |

敘述覆蓋是執行到的敘述數除以全部敘述數。分支覆蓋是執行到的分支數除以全部分支數。兩者分開算，沒有把分支混進敘述百分比。

## 覆蓋較低的檔案

只列這次測量裡敘述覆蓋最低的檔案，最多 12 個。

| 檔案 | 敘述覆蓋 | 已覆蓋 / 敘述 |
|---|---:|---:|
| `je_mail_thunder/__main__.py` | 0.0% | 0 / 37 |
| `je_mail_thunder/imap/imap_wrapper.py` | 54.03% | 67 / 124 |
| `je_mail_thunder/studio/__main__.py` | 60.61% | 20 / 33 |
| `je_mail_thunder/utils/json_format/json_process.py` | 73.91% | 17 / 23 |
| `je_mail_thunder/utils/socket_server/mail_thunder_socket_server.py` | 81.25% | 26 / 32 |
| `je_mail_thunder/smtp/smtp_wrapper.py` | 87.59% | 127 / 145 |
| `je_mail_thunder/core/rfc822.py` | 92.31% | 72 / 78 |
| `je_mail_thunder/utils/logging/loggin_instance.py` | 92.86% | 39 / 42 |
| `je_mail_thunder/utils/lazy_instance/lazy_instance.py` | 93.1% | 27 / 29 |
| `je_mail_thunder/utils/project/create_project_structure.py` | 96.23% | 51 / 53 |
| `je_mail_thunder/utils/oauth2/oauth2.py` | 96.4% | 134 / 139 |
| `je_mail_thunder/templates/loader.py` | 97.26% | 71 / 73 |
