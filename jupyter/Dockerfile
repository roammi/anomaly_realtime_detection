# For more information, please refer to https://aka.ms/vscode-docker-python
FROM python:3.8-slim

RUN mkdir src

WORKDIR /src

# Install pip requirements
COPY requirements.txt .
RUN python -m pip install -r requirements.txt

EXPOSE 8080

CMD ["jupyter", "notebook", "--no-browser", "--allow-root", "--ip=0.0.0.0", "--port=8080"]