FROM python:3.8-slim-buster

RUN npm install -g npm@9.1.3

WORKDIR /python-docker

COPY requirements.txt requirements.txt
COPY products.json products.json
RUN pip3 install -r requirements.txt

COPY . .

CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]
