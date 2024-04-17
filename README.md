### Prometheus 접속
- 로컬 호스트와 실행된 해당 포트로 접근하면 Prometheus UI로 접근가능

### Grafana
- 로컬 호스트와 실행된 해당 포트로 접근
  - login (compose yaml 참고) 하고 Prometheus 로 접근
  - 현재 docker-compose 기반의 container로 실행했으니 `http://[container-name]:[container-port]` 로 접근

### docker-componse 실행 옵션
- `docker-compose -f docker-compose-with-exporter.yml up -d`
  - `-f` : 해당 옵션을 지정하지 않으면 `docker-compose.yml` 을 읽는다.
  - `up -d` : 백그라운드로의 실행을 의미한다.

### Grafana에 Redis-export 대시보드 확인하기
- 해당 프로젝트의 json 파일을 Grafana의 대시보드에 추가하면 볼 수 있다.
