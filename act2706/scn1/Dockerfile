FROM python:3.9-alpine
LABEL author="Sharath"
RUN adduser -D ssuser && mkdir /home/ssuser/sample
USER ssuser
WORKDIR /home/ssuser/sample
ADD . /home/ssuser/sample
RUN pip install -r requiremnets.txt
EXPOSE 5000
CMD ["python", "main.py"]