**Iron Stack**  
*Protocolo de transporte P2P post-cuántico y anónimo*

**Iron Stack** es un stack de transporte UDP diseñado desde cero para operar en un escenario donde las computadoras cuánticas representan una amenaza real. Combina criptografía post-cuántica, enrutamiento cebolla, anonimato de red y ofuscación avanzada de tráfico en un solo protocolo coherente.

No es una VPN ni un proxy tradicional. Es una **infraestructura de transporte de bajo nivel** sobre la que se pueden construir aplicaciones y servicios que requieren privacidad y resistencia a adversarios sofisticados.

### El Problema
La mayoría de los sistemas de comunicación seguros actuales dependen de algoritmos criptográficos (RSA, ECDH, ECDSA) vulnerables a ataques cuánticos mediante el algoritmo de Shor. Además, sufren de filtración de metadatos, análisis de tráfico y dependencia de infraestructuras centralizadas.

Iron Stack fue creado para resolver estos problemas de forma integral.

### Arquitectura Principal

- **Criptografía Post-Cuántica**: Kyber-1024 (KEM) y Falcon (firmas), con diseño modular para futura migración.
- **Transporte**: UDP + BBR + Weighted Fair Queuing, multiplexación de streams, 0-RTT y entrega confiable.
- **Ghost Network**: Enrutamiento cebolla multi-hop (3-5 saltos) con pool de circuitos pre-construidos y celdas de tamaño fijo.
- **Anti-análisis de tráfico**: Tráfico de cobertura, segmentación aleatoria y Protocol Mimic (disfraz de TLS, QUIC y HTTP).
- **Ghost Rooms**: Salas cifradas de grupo con mensajería, transferencia de archivos y sistema de archivos virtual distribuido (VFS).
- **Modo Efímero**: Ejecución sin huella en disco, con hardening fuerte del kernel (landlock, seccomp, mlockall, etc.).
- **Cluster Gossip**: Descubrimiento distribuido con protección anti-Sybil y anti-clonación.

### Estado Actual

- Red funcional con múltiples nodos en entornos WAN.
- Construcción estable de circuitos y pools.
- Chat anónimo, transferencia de archivos y VFS distribuidos operativos.
- Modo efímero con medidas de seguridad avanzadas.

El sistema se encuentra en fase avanzada de desarrollo, acercándose a una versión beta cerrada.

### Oportunidad

Iron Stack representa una nueva capa de infraestructura pensada para la era post-cuántica. Puede servir como base para:
- Sistemas de comunicación anónima y resistente a censura
- Infraestructura distribuida para organizaciones con altos requisitos de privacidad
- Aplicaciones P2P seguras (chat, compartición de archivos, colaboración)
- Redes mesh resilientes

**Buscamos**  
Inversores técnicos, socios estratégicos y organizaciones interesadas en infraestructura de comunicaciones seguras y post-cuántica para colaborar en la siguiente etapa: estabilización final, auditoría externa y primeros despliegues productivos.

