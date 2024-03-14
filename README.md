# Linux WebServer: LAMP Stack

Welcome to my professional portfolio where I showcase my expertise in setting up robust and secure IT infrastructures. Today, I'll walk you through the process of installing and configuring a LAMP (Linux, Apache, MySQL, PHP) stack. This stack is essential for hosting dynamic web applications and websites, providing a solid foundation for your online presence.

![lamp](https://github.com/rasheedjimoh/lamp/assets/157264080/a02c50a3-cf4b-4bf7-8b5c-2094240fb7d1)


LAMP Stack Installation and Configuration:

1. **Assign IP and Install Linux (Ubuntu):**
   - Begin by assigning an IP address to your server and installing Ubuntu Linux.
   ```bash
   # Assign IP
   # Install Ubuntu
   ```

2. **Update System and Install Apache:**
   - Keep your system up-to-date and install the Apache web server.
   ```bash
   sudo apt update
   sudo apt install -y apache2 apache2-utils
   ```

3. **Install MariaDB/MySQL:**
   - Install MariaDB, a popular open-source database management system.
   ```bash
   sudo apt install -y mariadb-server mariadb-client
   ```

4. **Secure MySQL Installation:**
   - Secure your MySQL installation by running the MySQL secure installation script.
   ```bash
   sudo mysql_secure_installation
   ```

5. **Install PHP and PHP-MySQL Extension:**
   - Install PHP and its MySQL extension for server-side scripting.
   ```bash
   sudo apt install -y php php-mysql libapache2-mod-php
   ```

6. **Restart Apache and Verify Installation:**
   - Restart Apache to apply changes and verify the installation.
   ```bash
   sudo systemctl restart apache2
   ```

7. **Verify MariaDB Database and Apache Version:**
   - Confirm that MariaDB is functioning and check the Apache version.
   ```bash
   sudo mysql -u root -p
   sudo apache2 -V
   ```
![lamp-1](https://github.com/rasheedjimoh/lamp/assets/157264080/5e04db52-e621-4875-83c6-a3643907f220)
---
![lamp-2](https://github.com/rasheedjimoh/lamp/assets/157264080/d7303403-fab3-4deb-ae65-979fdeca8853)


8. **Check Apache Status and Test PHP:**
   - Ensure Apache is running and test PHP functionality.
   ```bash
   systemctl status apache2
   echo "<?php phpinfo();?>" | sudo tee /var/www/html/info.php
   ```
![lamp-3](https://github.com/rasheedjimoh/lamp/assets/157264080/8a1aae09-5a38-4bf7-9f13-d2e66d6192b1)

---

![lamp-4](https://github.com/rasheedjimoh/lamp/assets/157264080/7723d022-ca1d-4a60-ba71-ec735062ae66)

By completing these steps, you've established a LAMP stack, providing a powerful platform for hosting web applications and websites.

![lamp-5](https://github.com/rasheedjimoh/lamp/assets/157264080/d2be45d3-755b-4a12-acc8-0647c0d43570)


Benefits and Connection:

The LAMP stack combines four essential technologies: Linux, Apache, MySQL/MariaDB, and PHP, seamlessly integrated to deliver a robust web server environment. Here's how each component contributes:

- **Linux (Ubuntu):** Provides a stable and secure operating system foundation.
- **Apache:** Serves as the web server software, handling HTTP requests and delivering web content.
- **MariaDB/MySQL:** Acts as the database management system, storing and managing website data efficiently.
- **PHP:** Empowers dynamic web development, enabling server-side scripting for interactive web applications.

The interconnectedness of these technologies ensures a cohesive and reliable web hosting environment, supporting various web applications and services.

Conclusion:

By following these instructions, you've successfully set up a LAMP stack, laying the groundwork for hosting dynamic and secure web applications. This robust infrastructure enhances your organization's online presence, facilitating seamless interaction with users and clients.

Keep exploring and innovating in the realm of cybersecurity to ensure the resilience and security of your IT infrastructure.

Stay vigilant and secure!
