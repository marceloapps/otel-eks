## otel-eks

Precisa de um cluster kubernetes criado pra poder testar os deploys desse repositório.
O coletor do open telemetry é a distro da AWS e vai como daemonset pra receber uma cópia por node do cluster, imagino que uma cópia por node do cluster seja suficiente pra monitorar todos os pods sem capotar, mas isso pode ser revisto e transformado em Deployment.

O example-app ainda não ta rolando... é um trabalho em progresso

O docker-compose funciona pra poder subir um jaeger-all-in-one local na máquina e tentar configurar o exporter do coletor pra mandar pro jaeger local.
Também está nos planos tentar fazer um jogo com o appdynamics, é preciso validar ainda se o appdy no Brasil já aceita receber dados do open telemetry.

Isso aí =)
