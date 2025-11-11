
📂 Project Structure

ansible_wordpress
├── ansible.cfg
├── group_vars
│   └── web.yml
├── inventory
│   └── hosts
├── roles
│   ├── nginx
│   │   ├── tasks
│   │   │   ├── main.yml
│   │   │   └── ssl.yml
│   │   └── templates
│   │       ├── phpmyadmin.conf.j2
│   │       └── wordpress.conf.j2
│   ├── php
│   │   └── tasks
│   │       └── main.yml
│   ├── phpmyadmin
│   │   └── tasks
│   │       └── main.yml
│   ├── sftp_user
│   │   └── tasks
│   │       └── main.yml
│   └── wordpress
│       ├── tasks
│       │   └── main.yml
│       └── templates
│           └── wp-config.php.j2
└── site.yml

🚀 Deployment Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/muhammedfasilp07/ansible_wordpress.git
   cd ansible_wordpress

2. **Update your variables**
   * `inventory/hosts` → add your server IP
   * `group_vars/web.yml` → edit domain, database, and credentials

3. **Run the playbook**
   ```bash
   ansible-playbook site.yml
   
4. **Access your sites**
   * 🌐 WordPress → [https://muhammedfasilp07.info](https://muhammedfasilp07.info)
   * 🧰 phpMyAdmin → [https://muhammedfasilp07.info/phpMyAdmin](https://muhammedfasilp07.info/phpMyAdmin)

📄 Documentation

You can download the full **Deployment Guide PDF** below 👇  
👉 [**Download Ansible WordPress Deployment Guide (PDF)**](./Ansible_WordPress_Deployment_Guide.pdf)

or click the badge below:
[![View PDF](https://img.shields.io/badge/📄%20View%20Deployment%20Guide-PDF-blue)](./Ansible_WordPress_Deployment_Guide.pdf)


🧰 Stack Components

| Component      | Description                    |
| -------------- | ------------------------------ |
| **Ansible**    | Automation tool used for setup |
| **Nginx**      | Web server                     |
| **PHP-FPM**    | PHP FastCGI Process Manager    |
| **MariaDB**    | Database server                |
| **WordPress**  | CMS for your website           |
| **phpMyAdmin** | Database management GUI        |
| **Certbot**    | Free SSL via Let’s Encrypt     |
| **SFTP User**  | Secure file access for uploads |

🔒 Security Features

* HTTPS with **Let’s Encrypt SSL**
* Nginx security headers
* Limited SFTP access
* SELinux configuration for Nginx access

👤 Author

**Muhammed Fasil P**
💼 [LinkedIn](https://linkedin.com/in/muhammedfasilp07)
🌐 [Website](https://muhammedfasilp07.info)

 🏁 License
 
This project is open-source and available under the **MIT License**.
