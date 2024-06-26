FROM Python:3.12

WORKDIR /app

COPY requirments.txt .

RUN pip install -r requirments.txt

COPY . .

EXPOSE 13001

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "13001", "--reload"]