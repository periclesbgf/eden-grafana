# eden-grafana

Este projeto utiliza Docker Compose para subir três containers:
- **Grafana**: Dashboard para visualização dos logs.
- **Loki**: Sistema de agregação e consulta de logs.
- **Promtail**: Agente que coleta logs do host e os envia para o Loki.

## Como Usar

1. **Configure o Datasource:**
   Edite o arquivo `grafana/provisioning/datasources/loki-datasource.yaml` e ajuste a URL para o endereço da sua máquina Linux (por exemplo, `http://192.168.1.100:3100`).

2. **Suba os Containers:**
   No terminal, execute:
   ```bash
   docker-compose up -d

3. **Acesse o Grafana:**
    No navegador, abra a seguinte URL: http://localhost:3000.

    As credenciais padrão do Grafana são:
    - Usuário: admin
    - Senha: admin