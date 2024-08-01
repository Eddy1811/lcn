FROM python:3.9
LABEL authors="FEEZ"
ENV FLASK_APP microblog.py
ENV CONTEXT PROD
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
COPY . ./microblog
WORKDIR ./microblog
EXPOSE 5000
CMD ["./boot.sh"]