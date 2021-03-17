# hello-metrics

Self-configurated grafana instance (demo)

Automatic setup one datasource - **prometheus:9090**

Automatic setup two targets - **prometheus:9090** and **node-exporter:9100**

### Requirements

* Ubuntu >=16
* Docker
* Docker-compose
* Any web browser

### How to run

1. Run containers

    ```bash
    docker-compose down --volumes
    docker-compose up -d
    ```

2. Open http://localhost:3000/

3. Sing in. Login = admin, password = admin

4. Skip password changing

5. Find "Node Exporter Full" dashboard

### What's next

1. Create or import new dashboard
2. Export it to JSON config
3. Save it to file in **.deploy/grafana/dashboards** directory. Filename should not contain spaces!
