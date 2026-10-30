# Arquitectura del laboratorio

## Máquinas
| VM | SO | RAM | CPU | IP (lab-net) |
|---|---|---|---|---|
| wazuh-server | RedHat 8 | 4-5 GB | 2 | |
| win-victim | Windows 10/11 | 3-4 GB | 2 | |
| kali | Kali 2025.3 | 2 GB | 2 | |
| metasploitable | Metasploitable | 512 MB-1 GB | 1 | |

## Red
- Red interna `lab-net` (aislada): comunicación entre VMs.
- Adaptador host-only en wazuh-server: acceso al dashboard desde el host.
- NAT: solo temporal para actualizaciones.

## Diagrama
_(añadir en `diagramas/`)_
