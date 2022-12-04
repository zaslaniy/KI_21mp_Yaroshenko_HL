# KI_21mp_Yaroshenko_HL

#Лабораторна 1 Docker
Після встановлення Docker на комп'ютер, запускаємо його через додаток.
#Завдання 1:
Pull docker image “hello-world”.:
- `docker pull hello-world`
- `docker run hello-world`

Create docker-compose.yaml for container deploying.:
Створюємо в папці C:\Users\User\Documents\5 курс\1 сем\HL\lab_1 файл docker-compose.yaml
Deploy container and test the result.:
- `cd C:\Users\User\Documents\5 курс\1 сем\HL\lab_1`
- `docker-compose -f docker-compose.yaml up`

#Завдання 2:
task_2 :
- `cd docker_lab/task_2`
- `sudo docker-compose up`

task_3 :
- `cd docker_lab/task_3`
- `sudo docker-compose up`

task_4 :
- `cd docker_lab/task_4`
- `sudo docker-compose up --scale json_server=3 --scale lite_server=3`

task_5 :
- `cd docker_lab/task_1`
- `cat resulst.txt`

## Lab 2 (Jmeter)

- task1.jmx -> summary1.csv
- task2.jmx -> summary2.csv
- task3.jmx -> aggregate3.csv
- task4.jmx -> aggregate4.csv

## Lab 3 (Mongo)

- docker-compose up -d
- sudo sh init_rs.sh
- (wait several seconds)
- docker-compose exec router01 sh -c “mongo < .scripts/init-router.js”
- run all generate_data.ipynb
- cp mongo_lab/rides.csv mongo_lab/data/
- sudo sh import_and_query_data.sh
- docker-compose down -v --rmi all --remove-orphans

## Lab 4 (Hadoop)

- Hadoop.pdf - step by step protocol
- ProcessUnits.java - fixed Java code
- result.txt - results of requests (step 10)
- sample.txt - input data for requests 

## Lab 5 (Spark)

1. Correctly install spark (https://phoenixnap.com/kb/install-spark-on-ubuntu)
2. start-master.sh --webui-port 8001
3. apt install python3-pip
4. pip3 install pyspark, geopy, faker, numpy
5. download London.csv
6. spark-submit data_generation.py
7. spark-submit main.py
