<h1 align="center">Álvaro Hermosilla Alameda</h1>

<p align="center">
  <strong>Administración de Sistemas & Redes (ASIR)</strong> · DevOps & Cloud · Ciberseguridad · Full-Stack Developer
</p>

<p align="center">
  <a href="https://aha-portfolio.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio"></a>
  <a href="https://es.linkedin.com/in/%C3%A1lvaro-hermosilla-alameda-587526339"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:alvaro.hermosilla.alameda@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

---

## Sobre mí

Administro y automatizo la infraestructura sobre la que corren las aplicaciones: entornos **Linux** y **Windows Server**, redes, virtualización, contenedores y despliegue reproducible. Curso el **CFGS en Administración de Sistemas Informáticos en Red (ASIR)**, y mi Trabajo de Fin de Grado —**SysAgent**— es una infraestructura híbrida de dos nodos administrada por un agente de IA con un modelo de lenguaje local.

Vengo del desarrollo web (**CFGS en Desarrollo de Aplicaciones Web**) y sigo construyendo full-stack con React / Next.js, Node.js / NestJS y .NET. Esa doble formación es lo que más me define: administro sistemas entendiendo el código que corre sobre ellos, y escribo código sabiendo dónde se va a desplegar y qué superficie de ataque expone.

La **ciberseguridad** (ethical hacking y análisis forense digital) atraviesa las dos facetas: endurecimiento por defecto, privilegio mínimo y trazabilidad como requisito, no como añadido.

**En qué aporto valor:**

- Administración de entornos Linux y Windows Server: endurecido de SSH, cortafuegos con denegación por defecto, LVM, virtualización y direccionamiento.
- Redes privadas y acceso remoto seguro: túneles WireGuard, segmentación e identidad criptográfica revocable por dispositivo.
- Automatización y despliegue reproducible: Ansible, Docker y Docker Compose, scripting en Python y Bash, y CI/CD.
- Bases de datos en producción: MariaDB y PostgreSQL, replicación maestro-réplica, copias de seguridad y modos degradados.
- Desarrollo full-stack con API REST documentada (Swagger), autenticación JWT, rate limiting y cabeceras de seguridad (Helmet, HSTS).
- Seguridad aplicada al ciclo de vida del código: detección de secretos, revisión de dependencias y buenas prácticas OWASP.

<details>
<summary><b>🇬🇧 Read in English</b></summary>

<br>

I administer and automate the infrastructure applications run on: **Linux** and **Windows Server** environments, networking, virtualisation, containers and reproducible deployment. I am currently studying **Network Systems Administration (ASIR, higher vocational degree)**, and my final-year project —**SysAgent**— is a hybrid two-node infrastructure managed by an AI agent running a local language model.

I come from web development (**Web Application Development, DAW**) and still build full-stack with React / Next.js, Node.js / NestJS and .NET. That dual background is what defines me most: I administer systems understanding the code that runs on them, and I write code knowing where it will be deployed and what attack surface it exposes.

**Cybersecurity** (ethical hacking and digital forensics) runs through both sides: hardening by default, least privilege and traceability as a requirement rather than an afterthought.

**Where I add value:**

- Linux and Windows Server administration: SSH hardening, default-deny firewalls, LVM, virtualisation and IP addressing.
- Private networks and secure remote access: WireGuard tunnels, segmentation and per-device revocable cryptographic identity.
- Automation and reproducible deployment: Ansible, Docker and Docker Compose, Python and Bash scripting, and CI/CD.
- Databases in production: MariaDB and PostgreSQL, primary–replica replication, backups and degraded modes.
- Full-stack development with documented REST APIs (Swagger), JWT authentication, rate limiting and security headers (Helmet, HSTS).
- Security across the code lifecycle: secret detection, dependency review and OWASP best practices.

</details>

---

## Formación

- **CFGS Administración de Sistemas Informáticos en Red (ASIR)** — IES Valle Inclán, Torrejón de Ardoz (Madrid) · 2025–2027 · *en curso* — TFG: **SysAgent**
- **CFGS Desarrollo de Aplicaciones Web (DAW)** — IES Isidra de Guzmán, Alcalá de Henares (Madrid) · 2023–2025 · *Graduado* — TFG: **ConnectToPlay**

---

## Proyectos destacados · Featured projects

### SysAgent — Trabajo de Fin de Grado (ASIR) · 🚧 en desarrollo

Infraestructura híbrida de dos nodos —uno doméstico y uno en la nube— administrada mediante órdenes en lenguaje natural desde el móvil. Un modelo de lenguaje local interpreta la orden, selecciona una herramienta de un catálogo cerrado, la ejecuta con privilegios mínimos y registra el resultado en una base de datos replicada fuera del domicilio.

*Hybrid two-node infrastructure managed through natural-language commands from a phone. A local LLM interprets the command, picks a tool from a closed catalogue, executes it under least privilege and logs the result to an off-site replicated database.*

- **Red sin puertos abiertos** — túnel WireGuard en topología hub-and-spoke con el concentrador en el VPS.
- **Inferencia local sobre GPU** — `llama3.1:8b` vía Ollama: 52 tokens/s y 1,3 s de respuesta con el modelo residente en VRAM.
- **Datos como frontera de seguridad** — MariaDB en replicación maestro-réplica; la réplica sirve el histórico de auditoría en modo degradado de solo lectura.
- **Diagnóstico con método** — cuelgue intermitente de arranque (35 %) aislado a un módulo del initramfs sobre 140 arranques y verificado en ambos sentidos; decisiones registradas en ADRs y bitácora por sesión.
- **Seguridad por defecto** — SSH solo por clave ed25519, UFW con denegación por defecto, identidad criptográfica revocable por dispositivo y hook de pre-commit con gitleaks.

`Ubuntu Server 24.04 LTS` `VirtualBox` `Docker` `Ansible` `WireGuard` `Ollama` `Python 3.12` `FastAPI` `MariaDB 11` `Termux` `Netdata`

> Repositorio privado hasta la defensa · *Private repository until the thesis defence.*

### Desarrollo web · Web development

| Proyecto | Descripción | Stack |
|---|---|---|
| **[Portfolio](https://github.com/DevAlvaroHA/portfolio)** · [demo](https://aha-portfolio.vercel.app/) | Portfolio full-stack con contenido dinámico servido desde PostgreSQL, API documentada y hardening de seguridad.<br>*Full-stack portfolio with dynamic content from PostgreSQL, documented API and security hardening.* | Next.js 15 · React 19 · TypeScript · NestJS · TypeORM · PostgreSQL · Tailwind · shadcn/ui · Docker |
| **[ConnectToPlay](https://github.com/Xibancry/ju4-project)** | App social para crear lobbies y organizar partidas y quedadas deportivas. Proyecto en equipo.<br>*Social app to create lobbies for gaming sessions and sports meet-ups. Team project.* | Next.js · TypeScript · Node.js · PostgreSQL 15 · JWT · Docker |
| **[NotasMugiwara](https://github.com/DevAlvaroHA/NotasMugiwara)** | Gestor de notas interactivo con temas de color y diseño responsive.<br>*Interactive note manager with colour themes and responsive design.* | React · Vite · JavaScript · Tailwind · Docker |

---

## Stack tecnológico

**Sistemas, redes & seguridad**

![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Ubuntu Server](https://img.shields.io/badge/Ubuntu%20Server-E95420?style=flat-square&logo=ubuntu&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows%20Server-0078D6?style=flat-square&logo=windows&logoColor=white)
![Redes](https://img.shields.io/badge/Redes%20%26%20Firewalls-2E8B57?style=flat-square&logo=cisco&logoColor=white)
![WireGuard](https://img.shields.io/badge/WireGuard-88171A?style=flat-square&logo=wireguard&logoColor=white)
![SSH](https://img.shields.io/badge/SSH%20Hardening-4D4D4D?style=flat-square&logo=openssh&logoColor=white)
![Ethical Hacking](https://img.shields.io/badge/Ethical%20Hacking-000000?style=flat-square&logo=kalilinux&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP-000000?style=flat-square&logo=owasp&logoColor=white)
![Análisis Forense](https://img.shields.io/badge/An%C3%A1lisis%20Forense-800000?style=flat-square&logo=wireshark&logoColor=white)
![gitleaks](https://img.shields.io/badge/gitleaks-1E1E1E?style=flat-square&logo=git&logoColor=white)

**DevOps & cloud**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![VirtualBox](https://img.shields.io/badge/VirtualBox-183A61?style=flat-square&logo=virtualbox&logoColor=white)
![VMware](https://img.shields.io/badge/Virtualizaci%C3%B3n-607078?style=flat-square&logo=vmware&logoColor=white)
![Netdata](https://img.shields.io/badge/Netdata-00AB44?style=flat-square&logo=netdata&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

**IA & automatización**

![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![LLMs locales](https://img.shields.io/badge/LLMs%20locales-4B32C3?style=flat-square)
![Tool calling](https://img.shields.io/badge/Agentes%20%26%20Tool%20calling-6E44FF?style=flat-square)
![Automatización](https://img.shields.io/badge/Automatizaci%C3%B3n-3776AB?style=flat-square&logo=python&logoColor=white)

**Lenguajes & scripting**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)

**Bases de datos**

![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=flat-square&logo=mariadb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![TypeORM](https://img.shields.io/badge/TypeORM-FE0803?style=flat-square)
![Entity Framework](https://img.shields.io/badge/Entity%20Framework-512BD4?style=flat-square&logo=dotnet&logoColor=white)

**Backend**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET%20Core-5C2D91?style=flat-square&logo=dotnet&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=flat-square&logo=spring&logoColor=white)
![REST API](https://img.shields.io/badge/REST%20API-005571?style=flat-square&logo=swagger&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Redux](https://img.shields.io/badge/Redux-764ABC?style=flat-square&logo=redux&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=flat-square&logo=bootstrap&logoColor=white)
![Material UI](https://img.shields.io/badge/Material%20UI-0081CB?style=flat-square&logo=mui&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)

**Herramientas & metodologías**

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![GitLab](https://img.shields.io/badge/GitLab-FC6D26?style=flat-square&logo=gitlab&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)
![Scrum](https://img.shields.io/badge/Scrum-009FDA?style=flat-square&logo=jira&logoColor=white)

---

## Contacto · Contact

Abierto a oportunidades en **administración de sistemas, DevOps, ciberseguridad y desarrollo full-stack**.
*Open to opportunities in systems administration, DevOps, cybersecurity and full-stack development.*

- 🌐 **Portfolio** — [aha-portfolio.vercel.app](https://aha-portfolio.vercel.app/)
- 💼 **LinkedIn** — [Álvaro Hermosilla Alameda](https://es.linkedin.com/in/%C3%A1lvaro-hermosilla-alameda-587526339)
- 📫 **Email** — [alvaro.hermosilla.alameda@gmail.com](mailto:alvaro.hermosilla.alameda@gmail.com)
- 🐙 **GitHub** — [@DevAlvaroHA](https://github.com/DevAlvaroHA)
