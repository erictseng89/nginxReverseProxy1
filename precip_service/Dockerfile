# A set of instructions for docker to run
# Alpine is a lightweight linux distro
FROM python:3.7-alpine

WORKDIR /app

# requiements.txt will contain a list of apps that pip will install
COPY requirements.txt . 

RUN pip install -r requirements.txt

# copies files into container?
COPY . .

EXPOSE 5002

CMD ["python", "precip_server.py"]