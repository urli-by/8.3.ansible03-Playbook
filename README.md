# Elasticsearch & Kibana & Filebeat installation playbook

## Before run playbook you need to prepare an environment:
    `triple servers in cloud`

## Change ip of servers
    `you need to change ip addresses of servers in inventory/hosts.yml`
## Run playbook:
    `ansible-playbook -i inventory/prod.yml site.yml`

1. Установка Elasticsearch

   Версию можно указать в `group_vars/all.yml`.

2. Установка Kibana

   Версию можно указать в `group_vars/all.yml`.

3. Установка filebeat

   Версию можно указать в `group_vars/all.yml`.

Возможна установка отдельных компонентов с помощью тегов:

   `--tags filebeat` - установка JAVA

   `--tags elastic` - установка Elasticsearch

   `--tags kibana` - установка Kibana