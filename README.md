# 🧪 Home Lab Observability Stack

A complete, self-contained **monitoring and logging system** built for home lab or local DevOps practice. This stack includes **Prometheus**, **Grafana**, **Loki**, and **Promtail**, running entirely on your local machine using **Docker Compose**. It provides real-time system metrics, log collection, and interactive dashboards—just like you'd see in a professional production environment.

---

## 🚀 Features

- 📈 **Prometheus** – Collects and stores system metrics (CPU, memory, etc.)
- 📊 **Grafana** – Visualizes metrics and logs in beautiful dashboards
- 📜 **Loki** – Lightweight log aggregation system
- 🔍 **Promtail** – Log collector for Loki, tailing your system/app logs
- 🐳 **Docker Compose** – Runs the entire stack locally with one command
- ⚙️ **Node Exporter** – Monitors system hardware and OS metrics

---

## 📂 Project Structure



home-lab-observability/
│
├── docker-compose.yml        # Spins up all containers
├── prometheus/
│   └── prometheus.yml        # Scrape config for Prometheus
├── grafana/
│   └── provisioning/
│       └── dashboards/       # Optional prebuilt dashboards
├── loki/
│   └── config.yaml           # Loki config
├── promtail/
│   └── config.yml            # Promtail config
└── README.md                 # You're reading it :)


---

## 🛠️ Prerequisites

- Docker
- Docker Compose
- Linux-based system (for full metrics/log collection)
- Terminal access

---

## ⚙️ Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/home-lab-observability.git
   cd home-lab-observability


2. **Start the stack**

   ```bash
   docker-compose up -d
   ```

3. **Access your dashboards**

   * Grafana: [http://localhost:3000](http://localhost:3000)

     * Default login: `admin` / `admin`
   * Prometheus: [http://localhost:9090](http://localhost:9090)
   * Loki: [http://localhost:3100](http://localhost:3100)

4. **Import dashboards in Grafana**

   * Navigate to Dashboards → Import
   * Use dashboard ID: `1860` for Node Exporter Full
   * Select Prometheus as data source

---

 🔐 Security Note

This is a **local development/homelab project**. Do **not expose** this stack to the internet without securing it with TLS, user authentication, and firewalls.

---

## 📦 Technologies Used

* [Prometheus](https://prometheus.io/)
* [Grafana](https://grafana.com/)
* [Loki](https://grafana.com/oss/loki/)
* [Promtail](https://grafana.com/docs/loki/latest/clients/promtail/)
* [Node Exporter](https://github.com/prometheus/node_exporter)
* [Docker](https://www.docker.com/)
* [Docker Compose](https://docs.docker.com/compose/)

---


## 🤝 Contributing

Contributions welcome! Feel free to open issues or submit PRs if you enhance functionality, fix bugs, or improve documentation.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 💡 Inspiration

Built to simulate a production-grade observability setup on a single machine. Great for DevOps students, homelab enthusiasts, or anyone preparing for SRE/DevOps roles.

---

## ✨ Author

**\[Your Name]**
🔗 [LinkedIn](https://www.linkedin.com/in/rovindu404/) |

---

```
