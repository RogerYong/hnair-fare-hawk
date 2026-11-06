FROM python:3.12-slim
ENV PYTHONUNBUFFERED=1 TZ=Asia/Shanghai PIP_INDEX_URL=https://mirrors.aliyun.com/pypi/simple/
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
COPY requirements.txt /tmp/requirements.txt
RUN pip install --no-cache-dir -r /tmp/requirements.txt
WORKDIR /app
