# dmz-lab

Laboratorio de redes en Cisco Packet Tracer donde configuré una DMZ (Zona Desmilitarizada) con NAT y ACLs.

---

## ¿De qué trata?

La idea del laboratorio es simular una red de empresa donde hay un servidor web que tiene que ser accesible desde internet, pero sin que eso ponga en riesgo la red interna. Para eso se arma una zona separada llamada DMZ donde vive el servidor.

Se usó un router Cisco 2911 como firewall central con tres interfaces:
- Una para la red interna (LAN)
- Una para la DMZ
- Una para la red externa (internet simulado)

---

## Qué se configuró

- **IPs estáticas** en todos los dispositivos
- **NAT estático** para que el servidor de la DMZ sea accesible desde la red externa
- **ACLs** para controlar el tráfico:
  - Solo se permite HTTP (puerto 80) desde internet al servidor
  - El servidor no puede iniciar conexiones hacia la red interna

---

## Estructura del repositorio

```
dmz-lab/
├── README.md
├── DMZ_PROJECT.pka          ← archivo de Packet Tracer
├── informe/
│   └── Informe_DMZ_Laboratorio.md
└── evidencias/
    ├── topologia.png
    ├── running_config.png
    ├── show_acl_nat.png
    ├── pings.png
    ├── web_browsers.png
    └── check_results.png
```

---

## Resultado

La actividad fue completada al 100% en Packet Tracer.
