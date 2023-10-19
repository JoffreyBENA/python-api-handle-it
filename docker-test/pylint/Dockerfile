FROM python:3

COPY .pylintrc /

RUN pip install pylint 
RUN pip install pylint-json2html

CMD ["/bin/bash", "-c", "pylint /app/ > /app/reports/pylint/report.json; pylint-json2html -o /app/reports/pylint/report.html /app/reports/pylint/report.json"]