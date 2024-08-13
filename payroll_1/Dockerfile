FROM ubuntu:latest

RUN apt-get update
RUN apt-get install -y python3
RUN apt-get install -y python3-pip
RUN apt-get install -y python3-flask
RUN apt-get install -y sqlite3

#ADD templates __pycache__ payslip test.db static app.py templates /opt
ADD https://github.com/MeEisenheim/PayrollSystem.git /opt
ENTRYPOINT FLASK_APP=/opt/Lintech-Payroll--main/python -payroll/payroll_1/app.py flask run --host=0.0.0.0
