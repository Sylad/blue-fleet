# blue-fleet

Surveillance des machines du réseau maison (Big-Blue, mini-blue, dark-blue, NAS) :
statut, OS, charge, mémoire, uptime, puis une fiche par machine (WSL, processus,
disques, températures, GPU).

Données : le Prometheus du chart monitoring de dark-blue, alimenté par
windows_exporter, node-exporter et une sonde blackbox. Application NestJS +
React/TanStack, déployée sur le k3s de dark-blue par ArgoCD.

Accès réservé au réseau local (ou Cloudflare Access + PIN) : la liste des
machines et de leurs processus est une cartographie du réseau, jamais publique.

Plan : `.cadence/raf.yaml` (cadence).
