# zadanie1
Polecenie do zbudowania obrazu na platformy sprzętowe: linux/arm64, linux/amd64, z uwzględnieniem wykorzystania danych cache dla procesu budowania obrazu (punkt 2):
```bash
docker buildx build -f Dockerfile --platform linux/arm64,linux/amd64 --sbom --provenance=mode=max -t docker.io/1camile/zadanie1:zad1 --cache-to type=inline, --cache-from type=registry,ref=dpcker.io/1camile/zad1 --push .
```


Link do repo na dockerhub:  
https://hub.docker.com/r/1camile/zadanie1/tags
