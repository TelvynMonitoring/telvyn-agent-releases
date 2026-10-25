# Telvyn Agent — releases

Binários, instalador e guias de instalação do Telvyn Agent. O código-fonte é mantido em repositório privado.

## Instalação (Linux)

```bash
curl -fsSL https://raw.githubusercontent.com/TelvynMonitoring/telvyn-agent-releases/main/packaging/install.sh \
  | ISPWATCH_INGEST_URL='https://<SEU_PORTAL>' ISPWATCH_INGEST_TOKEN='<SEU_INGEST_TOKEN>' sudo -E bash
```

O comando completo, com o token e o endereço do seu ambiente, é gerado no portal Telvyn.

- Releases: pacotes `linux-amd64` e `linux-arm64`, com `.sha256`, e o pacote dos agentes de linguagem.
- Guias por linguagem: [`docs/`](docs/).
- Imagem: `ghcr.io/telvynmonitoring/telvyn-agent`; chart Helm: `oci://ghcr.io/telvynmonitoring/charts/ispwatch-agent`.
