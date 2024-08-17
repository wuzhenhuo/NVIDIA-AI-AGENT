# NVIDIA-AI-AGENT
## 项目名称：AI-AGENT夏季训练营 — RAG智能对话机器人
报告日期：2024年8月18日
项目负责人：吳振

项目概述:
第一部分為該項目應用於本公司開發的元宇宙平台《明日劇場》的技術手冊搜索。使用NVIDIA NIM 平台microsoft/phi-3-small-128k-instruct小模型做rag檢索，使用NV-Embed-QA模型做檢索。
以本產品技術手冊作為文檔，未來擬結合Gradio開發客戶應答機器人。

第二部分為視覺識別機器人
kosmosui.py
pip install openai chainlit matplotlib
export NVIDIA_API_KEY=
chainlit run kosmosui.py  

技术方案与实施步骤:
microsoft/phi-3-small-128k-instruct小模型做檢索，輕量化，便於安裝。

项目成果与展示：
![image](https://github.com/wuzhenhuo/NVIDIA-AI-AGENT/blob/main/pic.png)


问题与解决方案：
1.模型過期提示，根據vs的提示替換新模型。
2.需要執行一次第10模塊，後面可以重讀已經保存的向量存儲。
