# Notes

Damit das image gepullt werden kann, muss vorher mit folgendem command aus der
Datei .docker/config.json ein image pull secret erstellt werden:

```bash
k create secret generic regcred --from-file=.dockerconfigjson=.docker/config.json --type=kubernetes.io/dockerconfigjson -n fzimmermann
```
