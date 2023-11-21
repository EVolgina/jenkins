# Подготовка к выполнению
- Создать два VM: для jenkins-master и jenkins-agent.
  ![vm](https://github.com/EVolgina/jenkins/blob/jen/vm.PNG)
- Установить Jenkins при помощи playbook.
- Запустить и проверить работоспособность.
  ![pl](https://github.com/EVolgina/jenkins/blob/jen/start.PNG)
  ![1](https://github.com/EVolgina/jenkins/blob/jen/user.PNG)
- Сделать первоначальную настройку.
  ![ag](https://github.com/EVolgina/jenkins/blob/jen/lern.PNG)
  ![agent](https://github.com/EVolgina/jenkins/blob/jen/agent1.PNG)
   - Сдела агента. 
# Основная часть
- Сделать Freestyle Job, который будет запускать molecule test из любого вашего репозитория с ролью.
   ![rel](https://github.com/EVolgina/jenkins/blob/jen/zad1.PNG)
- Сделать Declarative Pipeline Job, который будет запускать molecule test из любого вашего репозитория с ролью.
  ![rr](https://github.com/EVolgina/jenkins/blob/jen/za1-2.PNG)
- Перенести Declarative Pipeline в репозиторий в файл Jenkinsfile.
  ![3](https://github.com/EVolgina/jenkins/blob/jen/zad1-3.PNG)
- Создать Multibranch Pipeline на запуск Jenkinsfile из репозитория.
- Создать Scripted Pipeline, наполнить его скриптом из pipeline.
- Внести необходимые изменения, чтобы Pipeline запускал ansible-playbook без флагов --check --diff, если не установлен параметр при запуске джобы (prod_run = True). По умолчанию параметр имеет значение False и - запускает прогон с флагами --check --diff.
- Проверить работоспособность, исправить ошибки, исправленный Pipeline вложить в репозиторий в файл ScriptedJenkinsfile.
- Отправить ссылку на репозиторий с ролью [clickhouse-role](https://github.com/EVolgina/clickhouse-role/tree/main/roles/clickhouse) и Declarative Pipeline и Scripted Pipeline.
- Сопроводите процесс настройки скриншотами для каждого пункта задания!!
