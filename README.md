# Nacho-Proyecto
# DataSafe Recovery (DSR)

## Descripción del proyecto

DataSafe Recovery (DSR) es un proyecto de infraestructura destinado a
ofrecer servicios de copias de seguridad, replicación, monitorización y
recuperación ante desastres para pequeñas y medianas empresas de la
provincia de Valencia.

El proyecto plantea una infraestructura virtualizada, segmentada
mediante VLAN y protegida mediante firewall, VPN y acceso administrativo
seguro.

**Alumno:** Nacho Herrero Llopis

**Ciclo:** 2.º CFGS Administración de Sistemas Informáticos en Red

**Código del proyecto:** IF_ASIR_02_NHL

---

## Objetivo de la infraestructura

El objetivo de DataSafe Recovery es diseñar una infraestructura segura,
automatizada y preparada para la continuidad del negocio.

La infraestructura permitirá:

- Realizar copias de seguridad y restauraciones.
- Mantener la continuidad de los servicios.
- Replicar información importante.
- Monitorizar el estado de los sistemas.
- Proteger los servicios mediante firewall.
- Separar los servicios públicos de los sistemas internos.
- Facilitar la administración segura de los servidores.
- Automatizar la configuración mediante Ansible.
- Reducir la superficie de ataque mediante VLAN.

La infraestructura se divide en cuatro VLAN:

- VLAN 10: Gestión y control.
- VLAN 20: DMZ expuesta.
- VLAN 30: Servicios internos.
- VLAN 40: Red de datos.

---

## Tecnologías utilizadas

- Proxmox VE
- pfSense
- Ansible
- Debian 12
- VLAN 802.1Q
- Prometheus
- Grafana
- Nextcloud
- PostgreSQL/MySQL
- Git


## Estructura del repositorio

DataSafe-Recovery/
│
├── playbooks/
│   └── site.yml
│
├── roles/
│   ├── seguridad/
│   │   └── .gitkeep
│   ├── monitorizacion/
│   │   └── .gitkeep
│   ├── servicios_web/
│   │   └── .gitkeep
│   └── firewall/
│       └── .gitkeep
│
├── variables/
│   └── vault.yml
│
├── plantillas/
│   └── nginx_grafana.conf.j2
│
├── inventario/
│   └── inventory.ini
│
├── documentacion/
│   └── arquitectura.md
│
└── README.md
