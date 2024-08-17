# NVIDIA-AI-AGENT
## 项目名称：AI-AGENT夏季训练营 — RAG智能对话机器人
报告日期：2024年8月18日
项目负责人：吳振

项目概述:  

第一部分為該項目應用於本公司開發的元宇宙平台《明日劇場》的技術手冊搜索。使用NVIDIA NIM 平台microsoft/phi-3-small-128k-instruct小模型做rag檢索，使用NV-Embed-QA模型做檢索。
以本產品技術手冊作為文檔，未來擬結合Gradio開發客戶應答機器人。

環境搭建：  
VS，安裝.NET Inatall Tool.
配置環境：
```
# 1.創建python 3.8（以上）虛擬環境
conda create --name ai_endpoint python=3.8
# 2.進入虛擬環境
conda activate ai_endpoint.
# 3.安裝nvidia_ai_endpoint工具
pip install langchain-nvidia-ai-endpoints
# 4.安裝jupyter lab
pip install jupyterlab
# 5 安裝langchain_core
pip install langchain_core
# 6 安裝langchain
pip install langchain
# 7 安裝matplotlib
pip install matplotlib
# 8 安裝Numpy
pip install numpy
# 9 安裝faiss,
pip install faiss-cpu==1.7.2
# 10 安裝openai庫
pip instal openai
# 利用jupyter lab打開可見
jupyter-lab
```
第二部分為視覺識別機器人  
使用NVIDIA NIM 平台microsoft/kosmos-2多模态模型,使用vs.
具体代码见kosmosui.py，具体执行步骤：
```
1.pip install openai chainlit matplotlib  
2.export NVIDIA_API_KEY=  
3.chainlit run kosmosui.py
``` 

技术方案与实施步骤:
microsoft/phi-3-small-128k-instruct小模型做檢索，輕量化，便於安裝。

项目成果与展示：
![image](https://github.com/wuzhenhuo/NVIDIA-AI-AGENT/blob/main/pic.png)
功能演示:  
![image](https://github.com/wuzhenhuo/NVIDIA-AI-AGENT/blob/main/pic2.jpg)

问题与解决方案：
1.模型過期提示，根據vs的提示替換新模型。
2.需要執行一次第10模塊，後面可以重讀已經保存的向量存儲。
