# docker-kubernetes_cloud-weekend-2026-08
Conteúdos da apresentação "Docker e Kubernetes: dicas e truques para descomplicar sua vida ao trabalhar com containers!".

## Algumas dicas e truques

### Dashboards Grafana + Prometheus monitorando clusters Kubernetes

Dashboards gratuitos: **https://github.com/dotdc/grafana-dashboards-kubernetes**

![Grafana x Prometheus x Kubernetes](img/grafana-prometheus-01.png)

### Dashboards with Grafana

Nova funcionalidade no Portal do Azure.

Listando os clusters/containers registrados:

```bash
kubectl config get-contexts
```

Configurando o uso de um cluster via kubectl:

```bash
kubectl config use-context <context-name>
```

Link: **https://github.com/ahmetb/kubectx**

### Docker MCP Catalog (MCP Servers seguros)

Link: **https://hub.docker.com/mcp**

![Docker MCP Catalog](img/docker-mcp-catalog-01.png)

Utilizando o MCP Server de Kubernetes no VS Code

```json
{
	"servers": {
		"kubernetes": {
			"type": "stdio",
			"command": "npx",
			"args": ["mcp-server-kubernetes"],
			"description": "Kubernetes cluster management and operations"
		}
	},
}
```

### Escalabilidade com KEDA

Link: 

### Scanning de vulnerabilidades com Triy

Link: **https://trivy.dev/**

Exemplo: **https://github.com/renatogroffe/trivy_operator-aks-managed_prometheus** 