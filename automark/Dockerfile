FROM python:3.11-slim
WORKDIR /check
RUN pip install requests psycopg2-binary
<<<<<<< HEAD
COPY sanity_check.py autotest.py run_tests.sh ./
RUN chmod +x run_tests.sh
CMD ["./run_tests.sh"]
=======
COPY sanity_check.py ./
CMD ["python", "sanity_check.py"]
>>>>>>> stats-feature
