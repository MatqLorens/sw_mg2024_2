# CI/CD Pipeline for Docker Images

## Część obowiązkowa – Docker Scout
Workflow używa **Docker Scout** do skanowania obrazów pod kątem podatności. Obraz jest przesyłany do GHCR tylko wtedy, gdy nie zawiera krytycznych lub wysokich zagrożeń.

## Część nieobowiązkowa – Trivy
Workflow wykorzystuje **Trivy** jako narzędzie open-source do skanowania obrazów Docker oraz generuje dane **SBOM** i provenance.

### Uruchomienie
1. Workflow można uruchomić ręcznie (`workflow_dispatch`) lub poprzez push tagu `v*`.
2. Wszystkie obrazy są dostępne w GHCR: `ghcr.io/<USER>/server`.

### Wymagania
- Utworzenie **secrets** z `GITHUB_TOKEN` dla autoryzacji GHCR.

