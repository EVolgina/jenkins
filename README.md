# Подготовка к выполнению
- Создать два VM: для jenkins-master и jenkins-agent.
  ![vm](https://github.com/EVolgina/jenkins/blob/jen/vm.PNG)
- Установить Jenkins при помощи playbook.
- Запустить и проверить работоспособность.
  ![pl](https://github.com/EVolgina/jenkins/blob/jen/start.PNG)
  ![](https://github.com/EVolgina/jenkins/blob/jen/user.PNG)
- Сделать первоначальную настройку.
  ![agenr](https://github.com/EVolgina/jenkins/blob/jen/agent1.PNG)
  ![rel](https://github.com/EVolgina/jenkins/blob/jen/restatr.PNG)
  - Сдела, VM агента постоянно выклбчается и получает новый IP. Уже создала 2 новых агента, но они не включаются.
  Перезапускала службы и не помогло. Дальше выполнить задание не могу. Помогите разобраться.
# Основная часть
- Сделать Freestyle Job, который будет запускать molecule test из любого вашего репозитория с ролью.
- Сделать Declarative Pipeline Job, который будет запускать molecule test из любого вашего репозитория с ролью.
- Перенести Declarative Pipeline в репозиторий в файл Jenkinsfile.
- Создать Multibranch Pipeline на запуск Jenkinsfile из репозитория.
- Создать Scripted Pipeline, наполнить его скриптом из pipeline.
- Внести необходимые изменения, чтобы Pipeline запускал ansible-playbook без флагов --check --diff, если не установлен параметр при запуске джобы (prod_run = True). По умолчанию параметр имеет значение False и - запускает прогон с флагами --check --diff.
- Проверить работоспособность, исправить ошибки, исправленный Pipeline вложить в репозиторий в файл ScriptedJenkinsfile.
- Отправить ссылку на репозиторий с ролью и Declarative Pipeline и Scripted Pipeline.
- Сопроводите процесс настройки скриншотами для каждого пункта задания!!
