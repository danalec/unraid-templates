# Unraid Docker Templates

Repositório público de templates de containers Docker personalizados para o Unraid.

## Remotos e Espelhamento
* **Principal (Origem):** Forgejo local (`http://192.168.0.10:3000/danalec/unraid-templates`)
* **Backup/Espelho:** GitHub (`https://github.com/danalec/unraid-templates`) — *Sincronizado automaticamente via Push Mirror a cada commit*.

## Como Adicionar este Repositório ao seu Unraid

1. No Unraid, vá na aba **Settings** > **Docker**.
2. No campo **Template repositories**, adicione a URL:
   ```text
   https://github.com/danalec/unraid-templates
   ```
   *(Ou a URL do Forgejo local: `http://192.168.0.10:3000/danalec/unraid-templates`)*
3. Clique em **Save**.
4. Na aba **Docker**, clique em **Add Container** e selecione o template desejado na lista suspensa **Template**.

## Templates Disponíveis

| Container | Descrição | Rede Padrão | Porta Web |
| :--- | :--- | :--- | :--- |
| **Bootimus** | Servidor PXE/TFTP/HTTP boot com Web UI | bridge | 8086 (Admin), 8889 (PXE HTTP) |
| **Ollama** | Servidor de inferência LLM local | br0 (192.168.0.14) | 11434 |
| **Open-WebUI** | Interface web estilo ChatGPT integrada ao Ollama | br0 (192.168.0.13) | 8080 |
| **A-Eye** | Catálogo e busca inteligente de fotos com IA local | br0 (192.168.0.15) | 8000 |
| **SearXNG** | Metabuscador privativo e sem rastreamento | br0 (192.168.0.20) | 80 |
| **qbit-ok-proxy** | Proxy de compatibilidade de autenticação qBittorrent 5.x | bridge | 8081 |
| **Tamari** | Gerenciador de receitas culinárias | bridge | 4888 |
| **Scoop-Alts-Scheduler** | Agendador de sincronização do bucket Scoop | bridge | — |
