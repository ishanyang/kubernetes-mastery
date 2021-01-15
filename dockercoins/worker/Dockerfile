FROM python:alpine
RUN pip install -i https://pypi.tuna.tsinghua.edu.cn/simple redis
RUN pip install -i https://pypi.tuna.tsinghua.edu.cn/simple requests
COPY worker.py /
CMD ["python", "worker.py"]
