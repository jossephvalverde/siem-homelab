# Home Lab de Detección de Amenazas (Wazuh + MITRE ATT&CK)

Laboratorio personal para simular técnicas de ataque en un entorno aislado y construir detecciones documentadas con un SIEM.

> ⚠️ Todo el laboratorio corre en una red interna aislada y sobre máquinas propias. Ninguna técnica se ejecuta contra sistemas de terceros.

## Objetivo
- Desplegar un SIEM (Wazuh) con telemetría de endpoints (agentes + Sysmon).
- Simular técnicas de MITRE ATT&CK de forma controlada.
- Documentar cada técnica: ejecución, telemetría generada, detección y mejoras.

## Arquitectura
Ver [`docs/arquitectura.md`](docs/arquitectura.md) y el diagrama en [`diagramas/`](diagramas/).

| Rol | Sistema | Función |
|---|---|---|
| SIEM | RedHat 8 + Wazuh | Recolección, análisis y dashboards |
| Víctima | Windows 10/11 + Sysmon + agente Wazuh | Endpoint monitorizado |
| Atacante | Kali Linux 2025.3 | Simulación de ataques |
| Objetivo vulnerable | Metasploitable | Práctica de escaneo/explotación |

## Hardware / virtualización
- Host: i5-10400F, 16 GB RAM
- Hipervisor: Oracle VirtualBox
- Red: red interna aislada (`lab-net`) + host-only para el dashboard

## Progreso
- [ ] Fase 0: Repositorio y estructura
- [ ] Fase 1: Infraestructura base
- [ ] Fase 2: Telemetría (agentes + Sysmon)
- [ ] Fase 3: Ataques y detecciones
- [ ] Fase 4: Informe final y matriz de cobertura ATT&CK

## Write-ups
| ID ATT&CK | Técnica | Write-up | Detección |
|---|---|---|---|
| | | | |

## Estructura del repositorio
```
docs/           Documentación de instalación y arquitectura
configs/        Configuraciones (Wazuh, Sysmon)
detections/     Reglas de detección (Wazuh, Sigma)
writeups/       Un documento por técnica simulada
diagramas/      Diagramas de red y arquitectura
evidencias/     Capturas de pantalla
```

## Aprendizajes
_(se completa al final de cada fase)_
