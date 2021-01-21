
FROM python:2.7-stretch

RUN apt-get update -y && apt-get install python-dev python3-dev apt-utils libsasl2-dev python-dev libldap2-dev libssl-dev -y

RUN pip install flask flask_httpauth flask_simpleldap python-dotenv

ADD student_age.py /

EXPOSE 5000
VOLUME ["/data"]

CMD [ "python", "./student_age.py" ]




curl -u toto:python -X GET http://localhost:3000/pozos/api/v1.0/get_student_ages

