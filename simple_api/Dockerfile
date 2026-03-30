FROM python:3.13-slim
LABEL maintainer="KODJI KANKA Paul"
COPY requirements.txt student_age.py /
RUN apt update -y && apt install build-essential python3-dev libsasl2-dev libldap2-dev libssl-dev -y
RUN pip3 install -r /requirements.txt
VOLUME ["/data"]
EXPOSE 5000
CMD [ "python3", "./student_age.py" ]
