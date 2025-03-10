---
layout: docwithnav-edge
assignees:
title: Upgrade instructions
description: ThingsBoard Edge upgrade instructions

---

<ul id="markdown-toc">
    <li>
        <a href="#prepare-for-upgrading" id="markdown-toc-prepare-for-upgrading">Prepare for upgrading ThingsBoard Edge</a>
        <ul>
            <li>
                <a href="#prepare-ubuntucentos" id="markdown-toc-prepare-ubuntucentos">Ubuntu/CentOS</a>
            </li>
            <li>
                <a href="#prepare-docker-linux-mac" id="markdown-toc-prepare-docker-linux-mac">Docker (Linux or Mac OS)</a>
            </li>
            <li>
                <a href="#prepare-windows" id="markdown-toc-prepare-windows">Windows</a>
            </li>                        
        </ul>
    </li>
    <li>
        <a href="#upgrading-to-361" id="markdown-toc-upgrading-to-361">Upgrading to 3.6.1EDGE</a>
        <ul>
            <li>
                <a href="#ubuntucentos-361" id="markdown-toc-ubuntucentos-361">Ubuntu/CentOS</a>
            </li>
            <li>
                <a href="#docker-linux-mac-361" id="markdown-toc-docker-linux-mac-361">Docker (Linux or Mac OS)</a>
            </li>            
            <li>
                <a href="#windows-361" id="markdown-toc-windows-361">Windows</a>
            </li> 
        </ul>
    </li>
    <li>
        <a href="#upgrading-to-36" id="markdown-toc-upgrading-to-36">Upgrading to 3.6.0EDGE</a>
        <ul>
            <li>
                <a href="#ubuntucentos-36" id="markdown-toc-ubuntucentos-36">Ubuntu/CentOS</a>
            </li>
            <li>
                <a href="#docker-linux-mac-36" id="markdown-toc-docker-linux-mac-36">Docker (Linux or Mac OS)</a>
            </li>            
            <li>
                <a href="#windows-36" id="markdown-toc-windows-36">Windows</a>
            </li> 
        </ul>
    </li>
    <li>
        <a href="#upgrading-to-3511" id="markdown-toc-upgrading-to-3511">Upgrading to 3.5.1.1EDGE</a>
        <ul>
            <li>
                <a href="#ubuntucentos-3511" id="markdown-toc-ubuntucentos-3511">Ubuntu/CentOS</a>
            </li>
            <li>
                <a href="#docker-linux-mac-3511" id="markdown-toc-docker-linux-mac-3511">Docker (Linux or Mac OS)</a>
            </li>            
            <li>
                <a href="#windows-3511" id="markdown-toc-windows-3511">Windows</a>
            </li> 
        </ul>
    </li>
    <li>
        <a href="#upgrading-to-351" id="markdown-toc-upgrading-to-351">Upgrading to 3.5.1EDGE</a>
        <ul>
            <li>
                <a href="#ubuntucentos-351" id="markdown-toc-ubuntucentos-351">Ubuntu/CentOS</a>
            </li>
            <li>
                <a href="#docker-linux-mac-351" id="markdown-toc-docker-linux-mac-351">Docker (Linux or Mac OS)</a>
            </li>            
            <li>
                <a href="#windows-351" id="markdown-toc-windows-351">Windows</a>
            </li> 
        </ul>
    </li>
    <li>
        <a href="#upgrading-to-35" id="markdown-toc-upgrading-to-35">Upgrading to 3.5.0EDGE</a>
        <ul>
            <li>
                <a href="#ubuntucentos-35" id="markdown-toc-ubuntucentos-35">Ubuntu/CentOS</a>
            </li>
            <li>
                <a href="#docker-linux-mac-35" id="markdown-toc-docker-linux-mac-35">Docker (Linux or Mac OS)</a>
            </li>            
            <li>
                <a href="#windows-35" id="markdown-toc-windows-35">Windows</a>
            </li> 
        </ul>
    </li>
    <li>
        <a href="#upgrading-to-343" id="markdown-toc-upgrading-to-343">Upgrading to 3.4.3EDGE</a>
        <ul>
            <li>
                <a href="#ubuntucentos-343" id="markdown-toc-ubuntucentos-343">Ubuntu/CentOS</a>
            </li>
            <li>
                <a href="#docker-linux-mac-343" id="markdown-toc-docker-linux-mac-343">Docker (Linux or Mac OS)</a>
            </li>            
            <li>
                <a href="#windows-343" id="markdown-toc-windows-343">Windows</a>
            </li> 
        </ul>
    </li>
    <li>
        <a href="#upgrading-to-341" id="markdown-toc-upgrading-to-341">Upgrading to 3.4.1EDGE</a>
        <ul>
            <li>
                <a href="#ubuntucentos-341" id="markdown-toc-ubuntucentos-341">Ubuntu/CentOS</a>
            </li>
            <li>
                <a href="#docker-linux-mac-341" id="markdown-toc-docker-linux-mac-341">Docker (Linux or Mac OS)</a>
            </li>            
            <li>
                <a href="#windows-341" id="markdown-toc-windows-341">Windows</a>
            </li> 
        </ul>
    </li>
    <li>
        <a href="#upgrading-to-34" id="markdown-toc-upgrading-to-34">Upgrading to 3.4EDGE</a>
        <ul>
            <li>
                <a href="#ubuntucentos-34" id="markdown-toc-ubuntucentos-34">Ubuntu/CentOS</a>
            </li>
            <li>
                <a href="#docker-linux-mac-34" id="markdown-toc-docker-linux-mac-34">Docker (Linux or Mac OS)</a>
            </li>            
            <li>
                <a href="#windows-34" id="markdown-toc-windows-34">Windows</a>
            </li> 
        </ul>
    </li>
    <li>
        <a href="#upgrading-to-334" id="markdown-toc-upgrading-to-3341">Upgrading to 3.3.4.1EDGE</a>
        <ul>
            <li>
                <a href="#ubuntucentos-334" id="markdown-toc-ubuntucentos-3341">Ubuntu/CentOS</a>
            </li>
            <li>
                <a href="#docker-linux-mac-334" id="markdown-toc-docker-linux-mac-3341">Docker (Linux or Mac OS)</a>
            </li>            
            <li>
                <a href="#windows-334" id="markdown-toc-windows-3341">Windows</a>
            </li> 
        </ul>
    </li>
</ul>

{% include templates/edge/install/compatibility-warning-general.md %}

## Prepare for upgrading ThingsBoard Edge {#prepare-for-upgrading}

### Ubuntu/CentOS {#prepare-ubuntucentos}

Stop ThingsBoard Edge service:

```bash
sudo systemctl stop tb-edge
```
{: .copy-code}

#### Backup Database

Make a backup of the database before upgrading.  

***Make sure you have enough space to place a backup of the database***  

Check database size

```bash
sudo -u postgres psql -c "SELECT pg_size_pretty( pg_database_size('tb_edge') );"
```
{: .copy-code}

Check free space

```bash
df -h /
```
{: .copy-code}

If there is enough free space - make a backup.

```bash
sudo -Hiu postgres pg_dump tb_edge > tb_edge.sql.bak
```
{: .copy-code}

Check backup file created successfully.

### Docker (Linux or Mac OS) {#prepare-docker-linux-mac}

Set the terminal in the directory which contains the `docker-compose.yml` file and execute the following command to stop and remove currently running TB Edge container:
```
docker compose stop
docker compose rm mytbedge
```
{: .copy-code}

{% capture dockerComposeStandalone %}
If you still rely on Docker Compose as docker-compose (with a hyphen) here is the list of the above commands:
<br>**docker-compose stop**
<br>**docker-compose rm mytbedge**
{% endcapture %}
{% include templates/info-banner.md content=dockerComposeStandalone %}

#### Backup Database

Make a copy of the database folder before upgrading:
```
sudo cp -r ~/.mytb-edge-data/db ~/.mytb-edge-db-BACKUP
```
{: .copy-code}

### Windows {#prepare-windows}

Stop ThingsBoard Edge service:

```text
net stop tb-edge
```
{: .copy-code}

#### Backup Database

Launch the "pgAdmin" software and login as superuser (postgres). 
Open your server and create backup of database **tb_edge** using 'Backup Dialog' functionality of "pgAdmin".

## Upgrading to 3.6.1EDGE {#upgrading-to-361}

{% assign serverVersion = "3.6.1" %}
{% assign updateServerLink = "#upgrading-to-361" %}
{% include templates/edge/install/compatibility-warning-version.md %}

### Ubuntu/CentOS {#ubuntucentos-361}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.6.0EDGE version.

#### ThingsBoard Edge package download

{% capture tabspec %}tb-edge-download-3-6-1
tb-edge-download-3-6-1-ubuntu,Ubuntu,shell,resources/3.6.1/tb-edge-ubuntu-download.sh,/docs/user-guide/install/edge/resources/3.6.1/tb-edge-ubuntu-download.sh
tb-edge-download-3-6-1-centos,CentOS,shell,resources/3.6.1/tb-edge-centos-download.sh,/docs/user-guide/install/edge/resources/3.6.1/tb-edge-centos-download.sh{% endcapture %}
{% include tabs.html %}

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running.

```bash
sudo service tb-edge stop
```
{: .copy-code}

{% capture tabspec %}tb-edge-installation-3-6-1
tb-edge-installation-3-6-1-ubuntu,Ubuntu,shell,resources/3.6.1/tb-edge-ubuntu-installation.sh,/docs/user-guide/install/edge/resources/3.6.1/tb-edge-ubuntu-installation.sh
tb-edge-installation-3-6-1-centos,CentOS,shell,resources/3.6.1/tb-edge-centos-installation.sh,/docs/user-guide/install/edge/resources/3.6.1/tb-edge-centos-installation.sh{% endcapture %}
{% include tabs.html %}

**NOTE:** Package installer may ask you to merge your tb-edge configuration. It is preferred to use **merge option** to make sure that all your previous parameters will not be overwritten.

Execute regular upgrade script:

```bash
sudo /usr/share/tb-edge/bin/install/upgrade.sh --fromVersion=3.6.0
```
{: .copy-code}

#### Start the service

```bash
sudo service tb-edge start
```
{: .copy-code}

### Docker (Linux or Mac OS) {#docker-linux-mac-361}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.6.0EDGE version.

Execute the following command to pull **3.6.1EDGE** image:
```
docker pull thingsboard/tb-edge:3.6.1EDGE
```
{: .copy-code}

Set the terminal in the directory which contains the `docker-compose.yml` file and execute the following command to stop and remove currently running TB Edge container (if it's still running):
```
docker compose stop
docker compose rm mytbedge
```
{: .copy-code}

Create docker compose file for ThingsBoard Edge upgrade process:

```text
nano docker-compose-upgrade.yml
```
{: .copy-code}

Add the following lines to the yml file:

```yml
version: '3.0'
services:
  mytbedge:
    restart: on-failure
    image: "thingsboard/tb-edge:3.6.1EDGE"
    environment:
      SPRING_DATASOURCE_URL: jdbc:postgresql://postgres:5432/tb-edge
    volumes:
      - ~/.mytb-edge-data:/data
      - ~/.mytb-edge-logs:/var/log/tb-edge
    entrypoint: upgrade-tb-edge.sh
  postgres:
    restart: always
    image: "postgres:12"
    ports:
      - "5432"
    environment:
      POSTGRES_DB: tb-edge
      POSTGRES_PASSWORD: postgres
    volumes:
      - ~/.mytb-edge-data/db:/var/lib/postgresql/data
```
{: .copy-code}

Execute the following command to start upgrade process:
```
docker compose -f docker-compose-upgrade.yml up
```
{: .copy-code}

Once upgrade process successfully completed, exit from the docker-compose shell by this combination:
```
Ctrl + C
```

Execute the following command to stop TB Edge upgrade container:
```
docker compose -f docker-compose-upgrade.yml stop
```
{: .copy-code}

Modify 'main' docker compose (`docker-compose.yml`) file for ThingsBoard Edge and update version of the image:

```text
nano docker-compose.yml
```
{: .copy-code}

```yml
version: '3.0'
services:
  mytbedge:
    restart: always
    image: "thingsboard/tb-edge:3.6.1EDGE"
...
```

Make sure your image is the set to tb-edge-**3.6.1EDGE**.

Execute the following commands to up this docker compose directly:
```
docker compose up -d
docker compose logs -f mytbedge
```
{: .copy-code}


### Windows {#windows-361}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.6.0EDGE version.

#### ThingsBoard Edge package download

Download ThingsBoard Edge package for Windows: [tb-edge-windows-3.6.1.zip](https://github.com/thingsboard/thingsboard-edge/releases/download/v3.6.1/tb-edge-windows-3.6.1.zip).

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running:

```text
net stop tb-edge
```
{: .copy-code}

* Make a backup of previous ThingsBoard Edge configuration located in *\<ThingsBoard Edge install dir\>\conf* (for example: *C:\tb-edge\conf*).

* Extract ThingsBoard Edge package.

* Compare and merge your old ThingsBoard Edge configuration files (from the backup you made in the previous step) with new ones.

* Finally, run **upgrade.bat** script to upgrade ThingsBoard Edge to the new version.

**NOTE** Scripts listed below should be executed using Administrator Role.

Execute regular upgrade script:

```text
C:\tb-edge>upgrade.bat --fromVersion=3.6.0
```

#### Start the service

```text
net start tb-edge
```
{: .copy-code}


## Upgrading to 3.6.0EDGE {#upgrading-to-36}

{% assign serverVersion = "3.6.0" %}
{% assign updateServerLink = "#upgrading-to-36" %}
{% include templates/edge/install/compatibility-warning-version.md %}

### Ubuntu/CentOS {#ubuntucentos-36}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.5.1.1EDGE version.

#### ThingsBoard Edge package download

{% capture tabspec %}tb-edge-download-3-6-0
tb-edge-download-3-6-0-ubuntu,Ubuntu,shell,resources/3.6/tb-edge-ubuntu-download.sh,/docs/user-guide/install/edge/resources/3.6/tb-edge-ubuntu-download.sh
tb-edge-download-3-6-0-centos,CentOS,shell,resources/3.6/tb-edge-centos-download.sh,/docs/user-guide/install/edge/resources/3.6/tb-edge-centos-download.sh{% endcapture %}
{% include tabs.html %}

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running.

```bash
sudo service tb-edge stop
```
{: .copy-code}

{% capture tabspec %}tb-edge-installation-3-6-0
tb-edge-installation-3-6-0-ubuntu,Ubuntu,shell,resources/3.6/tb-edge-ubuntu-installation.sh,/docs/user-guide/install/edge/resources/3.6/tb-edge-ubuntu-installation.sh
tb-edge-installation-3-6-0-centos,CentOS,shell,resources/3.6/tb-edge-centos-installation.sh,/docs/user-guide/install/edge/resources/3.6/tb-edge-centos-installation.sh{% endcapture %}
{% include tabs.html %}

**NOTE:** Package installer may ask you to merge your tb-edge configuration. It is preferred to use **merge option** to make sure that all your previous parameters will not be overwritten.

Execute regular upgrade script:

```bash
sudo /usr/share/tb-edge/bin/install/upgrade.sh --fromVersion=3.5.1
```
{: .copy-code}

#### Start the service

```bash
sudo service tb-edge start
```
{: .copy-code}

### Docker (Linux or Mac OS) {#docker-linux-mac-36}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.5.1.1EDGE version.

Execute the following command to pull **3.6.0EDGE** image:
```
docker pull thingsboard/tb-edge:3.6.0EDGE
```
{: .copy-code}

Set the terminal in the directory which contains the `docker-compose.yml` file and execute the following command to stop and remove currently running TB Edge container (if it's still running):
```
docker compose stop
docker compose rm mytbedge
```
{: .copy-code}

Create docker compose file for ThingsBoard Edge upgrade process:

```text
nano docker-compose-upgrade.yml
```
{: .copy-code}

Add the following lines to the yml file:

```yml
version: '3.0'
services:
  mytbedge:
    restart: on-failure
    image: "thingsboard/tb-edge:3.6.0EDGE"
    environment:
      SPRING_DATASOURCE_URL: jdbc:postgresql://postgres:5432/tb-edge
    volumes:
      - ~/.mytb-edge-data:/data
      - ~/.mytb-edge-logs:/var/log/tb-edge
    entrypoint: upgrade-tb-edge.sh
  postgres:
    restart: always
    image: "postgres:12"
    ports:
      - "5432"
    environment:
      POSTGRES_DB: tb-edge
      POSTGRES_PASSWORD: postgres
    volumes:
      - ~/.mytb-edge-data/db:/var/lib/postgresql/data
```
{: .copy-code}

Execute the following command to start upgrade process:
```
docker compose -f docker-compose-upgrade.yml up
```
{: .copy-code}

Once upgrade process successfully completed, exit from the docker-compose shell by this combination:
```
Ctrl + C
```

Execute the following command to stop TB Edge upgrade container:
```
docker compose -f docker-compose-upgrade.yml stop
```
{: .copy-code}

Modify 'main' docker compose (`docker-compose.yml`) file for ThingsBoard Edge and update version of the image:

```text
nano docker-compose.yml
```
{: .copy-code}

```yml
version: '3.0'
services:
  mytbedge:
    restart: always
    image: "thingsboard/tb-edge:3.6.0EDGE"
...
```

Make sure your image is the set to tb-edge-**3.6.0EDGE**.

Execute the following commands to up this docker compose directly:
```
docker compose up -d
docker compose logs -f mytbedge
```
{: .copy-code}


### Windows {#windows-36}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.5.1.1EDGE version.

#### ThingsBoard Edge package download

Download ThingsBoard Edge package for Windows: [tb-edge-windows-3.6.zip](https://github.com/thingsboard/thingsboard-edge/releases/download/v3.6/tb-edge-windows-3.6.zip).

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running:

```text
net stop tb-edge
```
{: .copy-code}

* Make a backup of previous ThingsBoard Edge configuration located in *\<ThingsBoard Edge install dir\>\conf* (for example: *C:\tb-edge\conf*).

* Extract ThingsBoard Edge package.

* Compare and merge your old ThingsBoard Edge configuration files (from the backup you made in the previous step) with new ones.

* Finally, run **upgrade.bat** script to upgrade ThingsBoard Edge to the new version.

**NOTE** Scripts listed below should be executed using Administrator Role.

Execute regular upgrade script:

```text
C:\tb-edge>upgrade.bat --fromVersion=3.5.1
```

#### Start the service

```text
net start tb-edge
```
{: .copy-code}

## Upgrading to 3.5.1.1EDGE {#upgrading-to-3511}

{% assign serverVersion = "3.5.1" %}
{% assign updateServerLink = "#upgrading-to-351" %}
{% include templates/edge/install/compatibility-warning-version.md %}

### Ubuntu/CentOS {#ubuntucentos-3511}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.5.1EDGE version.

#### ThingsBoard Edge package download

{% capture tabspec %}tb-edge-download-3-5-1-1
tb-edge-download-3-5-1-1-ubuntu,Ubuntu,shell,resources/3.5.1.1/tb-edge-ubuntu-download.sh,/docs/user-guide/install/edge/resources/3.5.1.1/tb-edge-ubuntu-download.sh
tb-edge-download-3-5-1-1-centos,CentOS,shell,resources/3.5.1.1/tb-edge-centos-download.sh,/docs/user-guide/install/edge/resources/3.5.1.1/tb-edge-centos-download.sh{% endcapture %}
{% include tabs.html %}

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running.

```bash
sudo service tb-edge stop
```
{: .copy-code}

{% capture tabspec %}tb-edge-installation-3-5-1-1
tb-edge-installation-3-5-1-1-ubuntu,Ubuntu,shell,resources/3.5.1.1/tb-edge-ubuntu-installation.sh,/docs/user-guide/install/edge/resources/3.5.1.1/tb-edge-ubuntu-installation.sh
tb-edge-installation-3-5-1-1-centos,CentOS,shell,resources/3.5.1.1/tb-edge-centos-installation.sh,/docs/user-guide/install/edge/resources/3.5.1.1/tb-edge-centos-installation.sh{% endcapture %}
{% include tabs.html %}

**NOTE:** Package installer may ask you to merge your tb-edge configuration. It is preferred to use **merge option** to make sure that all your previous parameters will not be overwritten.

#### Start the service

```bash
sudo service tb-edge start
```
{: .copy-code}

### Docker (Linux or Mac OS) {#docker-linux-mac-3511}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.5.1EDGE version.

Execute the following command to pull **3.5.1.1EDGE** image:
```
docker pull thingsboard/tb-edge:3.5.1.1EDGE
```
{: .copy-code}

Set the terminal in the directory which contains the `docker-compose.yml` file and execute the following command to stop and remove currently running TB Edge container (if it's still running):
```
docker compose stop
docker compose rm mytbedge
```
{: .copy-code}

Modify docker compose (`docker-compose.yml`) file for ThingsBoard Edge and update version of the image:

```text
nano docker-compose.yml
```
{: .copy-code}

```yml
version: '3.0'
services:
  mytbedge:
    restart: always
    image: "thingsboard/tb-edge:3.5.1.1EDGE"
...
```

Make sure your image is the set to tb-edge-**3.5.1.1EDGE**.

Execute the following commands to up this docker compose directly:
```
docker compose up -d
docker compose logs -f mytbedge
```
{: .copy-code}


### Windows {#windows-3511}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.5.1EDGE version.

#### ThingsBoard Edge package download

Download ThingsBoard Edge package for Windows: [tb-edge-windows-3.5.1.1.zip](https://github.com/thingsboard/thingsboard-edge/releases/download/v3.5.1.1/tb-edge-windows-3.5.1.1.zip).

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running:

```text
net stop tb-edge
```
{: .copy-code}

* Make a backup of previous ThingsBoard Edge configuration located in *\<ThingsBoard Edge install dir\>\conf* (for example: *C:\tb-edge\conf*).

* Extract ThingsBoard Edge package.

* Compare and merge your old ThingsBoard Edge configuration files (from the backup you made in the previous step) with new ones.

#### Start the service

```text
net start tb-edge
```
{: .copy-code}


## Upgrading to 3.5.1EDGE {#upgrading-to-351}

{% assign serverVersion = "3.5.1" %}
{% assign updateServerLink = "#upgrading-to-351" %}
{% include templates/edge/install/compatibility-warning-version.md %}

### Ubuntu/CentOS {#ubuntucentos-351}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.5.0EDGE version.

#### ThingsBoard Edge package download

{% capture tabspec %}tb-edge-download-3-5-1
tb-edge-download-3-5-1-ubuntu,Ubuntu,shell,resources/3.5.1/tb-edge-ubuntu-download.sh,/docs/user-guide/install/edge/resources/3.5.1/tb-edge-ubuntu-download.sh
tb-edge-download-3-5-1-centos,CentOS,shell,resources/3.5.1/tb-edge-centos-download.sh,/docs/user-guide/install/edge/resources/3.5.1/tb-edge-centos-download.sh{% endcapture %}
{% include tabs.html %}

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running.

```bash
sudo service tb-edge stop
```
{: .copy-code}

{% capture tabspec %}tb-edge-installation-3-5-1
tb-edge-installation-3-5-1-ubuntu,Ubuntu,shell,resources/3.5.1/tb-edge-ubuntu-installation.sh,/docs/user-guide/install/edge/resources/3.5.1/tb-edge-ubuntu-installation.sh
tb-edge-installation-3-5-1-centos,CentOS,shell,resources/3.5.1/tb-edge-centos-installation.sh,/docs/user-guide/install/edge/resources/3.5.1/tb-edge-centos-installation.sh{% endcapture %}
{% include tabs.html %}

**NOTE:** Package installer may ask you to merge your tb-edge configuration. It is preferred to use **merge option** to make sure that all your previous parameters will not be overwritten.

Execute regular upgrade script:

```bash
sudo /usr/share/tb-edge/bin/install/upgrade.sh --fromVersion=3.5.0
```
{: .copy-code}

#### Start the service

```bash
sudo service tb-edge start
```
{: .copy-code}

### Docker (Linux or Mac OS) {#docker-linux-mac-351}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.5.0EDGE version.

Execute the following command to pull **3.5.1EDGE** image:
```
docker pull thingsboard/tb-edge:3.5.1EDGE
```
{: .copy-code}

Set the terminal in the directory which contains the `docker-compose.yml` file and execute the following command to stop and remove currently running TB Edge container (if it's still running):
```
docker compose stop
docker compose rm mytbedge
```
{: .copy-code}

Create docker compose file for ThingsBoard Edge upgrade process:

```text
nano docker-compose-upgrade.yml
```
{: .copy-code}

Add the following lines to the yml file:

```yml
version: '3.0'
services:
  mytbedge:
    restart: on-failure
    image: "thingsboard/tb-edge:3.5.1EDGE"
    environment:
      SPRING_DATASOURCE_URL: jdbc:postgresql://postgres:5432/tb-edge
    volumes:
      - ~/.mytb-edge-data:/data
      - ~/.mytb-edge-logs:/var/log/tb-edge
    entrypoint: upgrade-tb-edge.sh
  postgres:
    restart: always
    image: "postgres:12"
    ports:
      - "5432"
    environment:
      POSTGRES_DB: tb-edge
      POSTGRES_PASSWORD: postgres
    volumes:
      - ~/.mytb-edge-data/db:/var/lib/postgresql/data
```
{: .copy-code}

Execute the following command to start upgrade process:
```
docker compose -f docker-compose-upgrade.yml up
```
{: .copy-code}

Once upgrade process successfully completed, exit from the docker-compose shell by this combination:
```
Ctrl + C
```

Execute the following command to stop TB Edge upgrade container:
```
docker compose -f docker-compose-upgrade.yml stop
```
{: .copy-code}

Modify 'main' docker compose (`docker-compose.yml`) file for ThingsBoard Edge and update version of the image:

```text
nano docker-compose.yml
```
{: .copy-code}

```yml
version: '3.0'
services:
  mytbedge:
    restart: always
    image: "thingsboard/tb-edge:3.5.1EDGE"
...
```

Make sure your image is the set to tb-edge-**3.5.1EDGE**.

Execute the following commands to up this docker compose directly:
```
docker compose up -d
docker compose logs -f mytbedge
```
{: .copy-code}


### Windows {#windows-351}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.5.0EDGE version.

#### ThingsBoard Edge package download

Download ThingsBoard Edge package for Windows: [tb-edge-windows-3.5.1.zip](https://github.com/thingsboard/thingsboard-edge/releases/download/v3.5.1/tb-edge-windows-3.5.1.zip).

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running:

```text
net stop tb-edge
```
{: .copy-code}

* Make a backup of previous ThingsBoard Edge configuration located in *\<ThingsBoard Edge install dir\>\conf* (for example: *C:\tb-edge\conf*).

* Extract ThingsBoard Edge package.

* Compare and merge your old ThingsBoard Edge configuration files (from the backup you made in the previous step) with new ones.

* Finally, run **upgrade.bat** script to upgrade ThingsBoard Edge to the new version.

**NOTE** Scripts listed below should be executed using Administrator Role.

Execute regular upgrade script:

```text
C:\tb-edge>upgrade.bat --fromVersion=3.5.0
```

#### Start the service

```text
net start tb-edge
```
{: .copy-code}


## Upgrading to 3.5.0EDGE {#upgrading-to-35}

{% assign serverVersion = "3.5.0" %}
{% assign updateServerLink = "#upgrading-to-35" %}
{% include templates/edge/install/compatibility-warning-version.md %}

### Ubuntu/CentOS {#ubuntucentos-35}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.4.3EDGE version.

#### ThingsBoard Edge package download

{% capture tabspec %}tb-edge-download-3-5-0
tb-edge-download-3-5-0-ubuntu,Ubuntu,shell,resources/3.5/tb-edge-ubuntu-download.sh,/docs/user-guide/install/edge/resources/3.5/tb-edge-ubuntu-download.sh
tb-edge-download-3-5-0-centos,CentOS,shell,resources/3.5/tb-edge-centos-download.sh,/docs/user-guide/install/edge/resources/3.5/tb-edge-centos-download.sh{% endcapture %}
{% include tabs.html %}

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running.

```bash
sudo service tb-edge stop
```
{: .copy-code}

{% capture tabspec %}tb-edge-installation-3-5-0
tb-edge-installation-3-5-0-ubuntu,Ubuntu,shell,resources/3.5/tb-edge-ubuntu-installation.sh,/docs/user-guide/install/edge/resources/3.5/tb-edge-ubuntu-installation.sh
tb-edge-installation-3-5-0-centos,CentOS,shell,resources/3.5/tb-edge-centos-installation.sh,/docs/user-guide/install/edge/resources/3.5/tb-edge-centos-installation.sh{% endcapture %}
{% include tabs.html %}

**NOTE:** Package installer may ask you to merge your tb-edge configuration. It is preferred to use **merge option** to make sure that all your previous parameters will not be overwritten.

Execute regular upgrade script:

```bash
sudo /usr/share/tb-edge/bin/install/upgrade.sh --fromVersion=3.4.3
```
{: .copy-code}

#### Start the service

```bash
sudo service tb-edge start
```
{: .copy-code}

### Docker (Linux or Mac OS) {#docker-linux-mac-35}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.4.3EDGE version.

Execute the following command to pull **3.5.0EDGE** image:
```
docker pull thingsboard/tb-edge:3.5.0EDGE
```
{: .copy-code}

Set the terminal in the directory which contains the `docker-compose.yml` file and execute the following command to stop and remove currently running TB Edge container (if it's still running):
```
docker compose stop
docker compose rm mytbedge
```
{: .copy-code}

Create docker compose file for ThingsBoard Edge upgrade process:

```text
nano docker-compose-upgrade.yml
```
{: .copy-code}

Add the following lines to the yml file:

```yml
version: '3.0'
services:
  mytbedge:
    restart: on-failure
    image: "thingsboard/tb-edge:3.5.0EDGE"
    environment:
      SPRING_DATASOURCE_URL: jdbc:postgresql://postgres:5432/tb-edge
    volumes:
      - ~/.mytb-edge-data:/data
      - ~/.mytb-edge-logs:/var/log/tb-edge
    entrypoint: upgrade-tb-edge.sh
  postgres:
    restart: always
    image: "postgres:12"
    ports:
      - "5432"
    environment:
      POSTGRES_DB: tb-edge
      POSTGRES_PASSWORD: postgres
    volumes:
      - ~/.mytb-edge-data/db:/var/lib/postgresql/data
```
{: .copy-code}

Execute the following command to start upgrade process:
```
docker compose -f docker-compose-upgrade.yml up
```
{: .copy-code}

Once upgrade process successfully completed, exit from the docker-compose shell by this combination:
```
Ctrl + C
```

Execute the following command to stop TB Edge upgrade container:
```
docker compose -f docker-compose-upgrade.yml stop
```
{: .copy-code}

Modify 'main' docker compose (`docker-compose.yml`) file for ThingsBoard Edge and update version of the image:

```text
nano docker-compose.yml
```
{: .copy-code}

```yml
version: '3.0'
services:
  mytbedge:
    restart: always
    image: "thingsboard/tb-edge:3.5.0EDGE"
...
```

Make sure your image is the set to tb-edge-**3.5.0EDGE**.

Execute the following commands to up this docker compose directly:
```
docker compose up -d
docker compose logs -f mytbedge
```
{: .copy-code}


### Windows {#windows-35}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.4.3EDGE version.

#### ThingsBoard Edge package download

Download ThingsBoard Edge package for Windows: [tb-edge-windows-3.5.zip](https://github.com/thingsboard/thingsboard-edge/releases/download/v3.5/tb-edge-windows-3.5.zip).

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running:

```text
net stop tb-edge
```
{: .copy-code}

* Make a backup of previous ThingsBoard Edge configuration located in *\<ThingsBoard Edge install dir\>\conf* (for example: *C:\tb-edge\conf*).

* Extract ThingsBoard Edge package.

* Compare and merge your old ThingsBoard Edge configuration files (from the backup you made in the previous step) with new ones.

* Finally, run **upgrade.bat** script to upgrade ThingsBoard Edge to the new version.

**NOTE** Scripts listed below should be executed using Administrator Role.

Execute regular upgrade script:

```text
C:\tb-edge>upgrade.bat --fromVersion=3.4.3
```

#### Start the service

```text
net start tb-edge
```
{: .copy-code}


## Upgrading to 3.4.3EDGE {#upgrading-to-343}

{% assign serverVersion = "3.4.3" %}
{% assign updateServerLink = "#upgrading-to-343" %}
{% include templates/edge/install/compatibility-warning-version.md %}

### Ubuntu/CentOS {#ubuntucentos-343}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.4.1EDGE version.

#### ThingsBoard Edge package download

{% capture tabspec %}tb-edge-download-3-4-3
tb-edge-download-3-4-3-ubuntu,Ubuntu,shell,resources/3.4.3/tb-edge-ubuntu-download.sh,/docs/user-guide/install/edge/resources/3.4.3/tb-edge-ubuntu-download.sh
tb-edge-download-3-4-3-centos,CentOS,shell,resources/3.4.3/tb-edge-centos-download.sh,/docs/user-guide/install/edge/resources/3.4.3/tb-edge-centos-download.sh{% endcapture %}
{% include tabs.html %}

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running.

```bash
sudo service tb-edge stop
```
{: .copy-code}

{% capture tabspec %}tb-edge-installation-3-4-3
tb-edge-installation-3-4-3-ubuntu,Ubuntu,shell,resources/3.4.3/tb-edge-ubuntu-installation.sh,/docs/user-guide/install/edge/resources/3.4.3/tb-edge-ubuntu-installation.sh
tb-edge-installation-3-4-3-centos,CentOS,shell,resources/3.4.3/tb-edge-centos-installation.sh,/docs/user-guide/install/edge/resources/3.4.3/tb-edge-centos-installation.sh{% endcapture %}
{% include tabs.html %}

**NOTE:** Package installer may ask you to merge your tb-edge configuration. It is preferred to use **merge option** to make sure that all your previous parameters will not be overwritten.

Execute regular upgrade script:

```bash
sudo /usr/share/tb-edge/bin/install/upgrade.sh --fromVersion=3.4.1
```
{: .copy-code}

#### Start the service

```bash
sudo service tb-edge start
```
{: .copy-code}

### Docker (Linux or Mac OS) {#docker-linux-mac-343}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.4.1EDGE version.

Execute the following command to pull **3.4.3EDGE** image:
```
docker pull thingsboard/tb-edge:3.4.3EDGE
```
{: .copy-code}

Set the terminal in the directory which contains the `docker-compose.yml` file and execute the following command to stop and remove currently running TB Edge container (if it's still running):
```
docker compose stop
docker compose rm mytbedge
```
{: .copy-code}

Create docker compose file for ThingsBoard Edge upgrade process:

```text
nano docker-compose-upgrade.yml
```
{: .copy-code}

Add the following lines to the yml file:

```yml
version: '3.0'
services:
  mytbedge:
    restart: on-failure
    image: "thingsboard/tb-edge:3.4.3EDGE"
    environment:
      SPRING_DATASOURCE_URL: jdbc:postgresql://postgres:5432/tb-edge
    volumes:
      - ~/.mytb-edge-data:/data
      - ~/.mytb-edge-logs:/var/log/tb-edge
    entrypoint: upgrade-tb-edge.sh
  postgres:
    restart: always
    image: "postgres:12"
    ports:
      - "5432"
    environment:
      POSTGRES_DB: tb-edge
      POSTGRES_PASSWORD: postgres
    volumes:
      - ~/.mytb-edge-data/db:/var/lib/postgresql/data
```
{: .copy-code}

Execute the following command to start upgrade process:
```
docker compose -f docker-compose-upgrade.yml up
```
{: .copy-code}

Once upgrade process successfully completed, exit from the docker-compose shell by this combination:
```
Ctrl + C
```

Execute the following command to stop TB Edge upgrade container:
```
docker compose -f docker-compose-upgrade.yml stop
```
{: .copy-code}

Modify 'main' docker compose (`docker-compose.yml`) file for ThingsBoard Edge and update version of the image:

```text
nano docker-compose.yml
```
{: .copy-code}

```yml
version: '3.0'
services:
  mytbedge:
    restart: always
    image: "thingsboard/tb-edge:3.4.3EDGE"
...
```

Make sure your image is the set to tb-edge-**3.4.3EDGE**.

Execute the following commands to up this docker compose directly:
```
docker compose up -d
docker compose logs -f mytbedge
```
{: .copy-code}


### Windows {#windows-343}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.4.1EDGE version.

#### ThingsBoard Edge package download

Download ThingsBoard Edge package for Windows: [tb-edge-windows-3.4.3.zip](https://github.com/thingsboard/thingsboard-edge/releases/download/v3.4.3/tb-edge-windows-3.4.3.zip).

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running:

```text
net stop tb-edge
```
{: .copy-code}

* Make a backup of previous ThingsBoard Edge configuration located in *\<ThingsBoard Edge install dir\>\conf* (for example: *C:\tb-edge\conf*).

* Extract ThingsBoard Edge package.

* Compare and merge your old ThingsBoard Edge configuration files (from the backup you made in the previous step) with new ones.

* Finally, run **upgrade.bat** script to upgrade ThingsBoard Edge to the new version.

**NOTE** Scripts listed below should be executed using Administrator Role.

Execute regular upgrade script:

```text
C:\tb-edge>upgrade.bat --fromVersion=3.4.1
```

#### Start the service

```text
net start tb-edge
```
{: .copy-code}

## Upgrading to 3.4.1EDGE {#upgrading-to-341}

{% assign serverVersion = "3.4.1" %}
{% assign updateServerLink = "#upgrading-to-341" %}
{% include templates/edge/install/compatibility-warning-version.md %}

### Ubuntu/CentOS {#ubuntucentos-341}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.4.0EDGE version.

#### ThingsBoard Edge package download

{% capture tabspec %}tb-edge-download-3-4-1
tb-edge-download-3-4-1-ubuntu,Ubuntu,shell,resources/3.4.1/tb-edge-ubuntu-download.sh,/docs/user-guide/install/edge/resources/3.4.1/tb-edge-ubuntu-download.sh
tb-edge-download-3-4-1-centos,CentOS,shell,resources/3.4.1/tb-edge-centos-download.sh,/docs/user-guide/install/edge/resources/3.4.1/tb-edge-centos-download.sh{% endcapture %}
{% include tabs.html %}

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running.

```bash
sudo service tb-edge stop
```
{: .copy-code}

{% capture tabspec %}tb-edge-installation-3-4-1
tb-edge-installation-3-4-1-ubuntu,Ubuntu,shell,resources/3.4.1/tb-edge-ubuntu-installation.sh,/docs/user-guide/install/edge/resources/3.4.1/tb-edge-ubuntu-installation.sh
tb-edge-installation-3-4-1-centos,CentOS,shell,resources/3.4.1/tb-edge-centos-installation.sh,/docs/user-guide/install/edge/resources/3.4.1/tb-edge-centos-installation.sh{% endcapture %}
{% include tabs.html %}

**NOTE:** Package installer may ask you to merge your tb-edge configuration. It is preferred to use **merge option** to make sure that all your previous parameters will not be overwritten.

Execute regular upgrade script:

```bash
sudo /usr/share/tb-edge/bin/install/upgrade.sh --fromVersion=3.4.0
```
{: .copy-code}

#### Start the service

```bash
sudo service tb-edge start
```
{: .copy-code}

### Docker (Linux or Mac OS) {#docker-linux-mac-341}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.4.0EDGE version.

Execute the following command to pull **3.4.1EDGE** image:
```
docker pull thingsboard/tb-edge:3.4.1EDGE
```
{: .copy-code}

Set the terminal in the directory which contains the `docker-compose.yml` file and execute the following command to stop and remove currently running TB Edge container (if it's still running):
```
docker-compose stop
docker-compose rm mytbedge
```
{: .copy-code}

Create docker compose file for ThingsBoard Edge upgrade process:

```text
nano docker-compose-upgrade.yml
```
{: .copy-code}

Add the following lines to the yml file:

```yml
version: '3.0'
services:
  mytbedge:
    restart: on-failure
    image: "thingsboard/tb-edge:3.4.1EDGE"
    environment:
      SPRING_DATASOURCE_URL: jdbc:postgresql://postgres:5432/tb-edge
    volumes:
      - ~/.mytb-edge-data:/data
      - ~/.mytb-edge-logs:/var/log/tb-edge
    entrypoint: upgrade-tb-edge.sh
  postgres:
    restart: always
    image: "postgres:12"
    ports:
      - "5432"
    environment:
      POSTGRES_DB: tb-edge
      POSTGRES_PASSWORD: postgres
    volumes:
      - ~/.mytb-edge-data/db:/var/lib/postgresql/data
```
{: .copy-code}

Execute the following command to start upgrade process:
```
docker-compose -f docker-compose-upgrade.yml up
```
{: .copy-code}

Once upgrade process successfully completed, exit from the docker-compose shell by this combination:
```
Ctrl + C
```

Execute the following command to stop TB Edge upgrade container:
```
docker-compose -f docker-compose-upgrade.yml stop
```
{: .copy-code}

Modify 'main' docker compose (`docker-compose.yml`) file for ThingsBoard Edge and update version of the image:

```text
nano docker-compose.yml
```
{: .copy-code}

```yml
version: '3.0'
services:
  mytbedge:
    restart: always
    image: "thingsboard/tb-edge:3.4.1EDGE"
...
```

Make sure your image is the set to tb-edge-**3.4.1EDGE**.

Execute the following command to up this docker compose directly:
```
docker-compose up
```
{: .copy-code}


### Windows {#windows-341}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.4.0EDGE version.

#### ThingsBoard Edge package download

Download ThingsBoard Edge package for Windows: [tb-edge-windows-3.4.1.zip](https://github.com/thingsboard/thingsboard-edge/releases/download/v3.4.1/tb-edge-windows-3.4.1.zip).

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running:

```text
net stop tb-edge
```
{: .copy-code}

* Make a backup of previous ThingsBoard Edge configuration located in *\<ThingsBoard Edge install dir\>\conf* (for example: *C:\tb-edge\conf*).

* Extract ThingsBoard Edge package.

* Compare and merge your old ThingsBoard Edge configuration files (from the backup you made in the previous step) with new ones.

* Finally, run **upgrade.bat** script to upgrade ThingsBoard Edge to the new version.

**NOTE** Scripts listed below should be executed using Administrator Role.

Execute regular upgrade script:

```text
C:\tb-edge>upgrade.bat --fromVersion=3.4.0
```

#### Start the service

```text
net start tb-edge
```
{: .copy-code}

## Upgrading to 3.4EDGE {#upgrading-to-34}

{% assign serverVersion = "3.4" %}
{% assign updateServerLink = "#upgrading-to-34" %}
{% include templates/edge/install/compatibility-warning-version.md %}

### Ubuntu/CentOS {#ubuntucentos-34}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.3.4.1EDGE version.

#### ThingsBoard Edge package download

{% capture tabspec %}tb-edge-download-3-4-0
tb-edge-download-3-4-0-ubuntu,Ubuntu,shell,resources/3.4/tb-edge-ubuntu-download.sh,/docs/user-guide/install/edge/resources/3.4/tb-edge-ubuntu-download.sh
tb-edge-download-3-4-0-centos,CentOS,shell,resources/3.4/tb-edge-centos-download.sh,/docs/user-guide/install/edge/resources/3.4/tb-edge-centos-download.sh{% endcapture %}
{% include tabs.html %}

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running.

```bash
sudo service tb-edge stop
```
{: .copy-code}

{% capture tabspec %}tb-edge-installation-3-4-0
tb-edge-installation-3-4-0-ubuntu,Ubuntu,shell,resources/3.4/tb-edge-ubuntu-installation.sh,/docs/user-guide/install/edge/resources/3.4/tb-edge-ubuntu-installation.sh
tb-edge-installation-3-4-0-centos,CentOS,shell,resources/3.4/tb-edge-centos-installation.sh,/docs/user-guide/install/edge/resources/3.4/tb-edge-centos-installation.sh{% endcapture %}
{% include tabs.html %}

**NOTE:** Package installer may ask you to merge your tb-edge configuration. It is preferred to use **merge option** to make sure that all your previous parameters will not be overwritten.

Execute regular upgrade script:

```bash
sudo /usr/share/tb-edge/bin/install/upgrade.sh --fromVersion=3.3.4.1
```
{: .copy-code}

#### Start the service

```bash
sudo service tb-edge start
```
{: .copy-code}

### Docker (Linux or Mac OS) {#docker-linux-mac-34}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.3.4.1EDGE version.

Execute the following command to pull **3.4.0EDGE** image:
```
docker pull thingsboard/tb-edge:3.4.0EDGE
```
{: .copy-code}

Set the terminal in the directory which contains the `docker-compose.yml` file and execute the following command to stop and remove currently running TB Edge container (if it's still running):
```
docker-compose stop
docker-compose rm mytbedge
```
{: .copy-code}

Create docker compose file for ThingsBoard Edge upgrade process:

```text
nano docker-compose-upgrade.yml
```
{: .copy-code}

Add the following lines to the yml file:

```yml
version: '3.0'
services:
  mytbedge:
    restart: on-failure
    image: "thingsboard/tb-edge:3.4.0EDGE"
    environment:
      SPRING_DATASOURCE_URL: jdbc:postgresql://postgres:5432/tb-edge
    volumes:
      - ~/.mytb-edge-data:/data
      - ~/.mytb-edge-logs:/var/log/tb-edge
    entrypoint: upgrade-tb-edge.sh
  postgres:
    restart: always
    image: "postgres:12"
    ports:
      - "5432"
    environment:
      POSTGRES_DB: tb-edge
      POSTGRES_PASSWORD: postgres
    volumes:
      - ~/.mytb-edge-data/db:/var/lib/postgresql/data
```
{: .copy-code}

Execute the following command to start upgrade process:
```
docker-compose -f docker-compose-upgrade.yml up
```
{: .copy-code}

Once upgrade process successfully completed, exit from the docker-compose shell by this combination:
```
Ctrl + C
```

Execute the following command to stop TB Edge upgrade container:
```
docker-compose -f docker-compose-upgrade.yml stop
```
{: .copy-code}

Modify 'main' docker compose (`docker-compose.yml`) file for ThingsBoard Edge and update version of the image:

```text
nano docker-compose.yml
```
{: .copy-code}

```yml
version: '3.0'
services:
  mytbedge:
    restart: always
    image: "thingsboard/tb-edge:3.4.0EDGE"
...
```

Make sure your image is the set to tb-edge-**3.4.0EDGE**.

Execute the following command to up this docker compose directly:
```
docker-compose up
```
{: .copy-code}


### Windows {#windows-34}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.3.4.1EDGE version.

#### ThingsBoard Edge package download

Download ThingsBoard Edge package for Windows: [tb-edge-windows-3.4.zip](https://github.com/thingsboard/thingsboard-edge/releases/download/v3.4/tb-edge-windows-3.4.zip).

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running:

```text
net stop tb-edge
```
{: .copy-code}

* Make a backup of previous ThingsBoard Edge configuration located in *\<ThingsBoard Edge install dir\>\conf* (for example: *C:\tb-edge\conf*).

* Extract ThingsBoard Edge package.

* Compare and merge your old ThingsBoard Edge configuration files (from the backup you made in the previous step) with new ones.

* Finally, run **upgrade.bat** script to upgrade ThingsBoard Edge to the new version.

**NOTE** Scripts listed below should be executed using Administrator Role.

Execute regular upgrade script:

```text
C:\tb-edge>upgrade.bat --fromVersion=3.3.4.1
```

#### Start the service

```text
net start tb-edge
```
{: .copy-code}

## Upgrading to 3.3.4.1EDGE {#upgrading-to-3341}

{% assign serverVersion = "3.3.4.1" %}
{% assign updateServerLink = "#upgrading-to-3341" %}
{% include templates/edge/install/compatibility-warning-version.md %}

### Ubuntu/CentOS {#ubuntucentos-3341}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.3.4EDGE version.

#### ThingsBoard Edge package download

{% capture tabspec %}tb-edge-download-3-3-4-1
tb-edge-download-3-3-4-1-ubuntu,Ubuntu,shell,resources/3.3.4.1/tb-edge-ubuntu-download.sh,/docs/user-guide/install/edge/resources/3.3.4.1/tb-edge-ubuntu-download.sh
tb-edge-download-3-3-4-1-centos,CentOS,shell,resources/3.3.4.1/tb-edge-centos-download.sh,/docs/user-guide/install/edge/resources/3.3.4.1/tb-edge-centos-download.sh{% endcapture %}
{% include tabs.html %}

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running.

```bash
sudo service tb-edge stop
```
{: .copy-code}

{% capture tabspec %}tb-edge-installation-3-3-4-1
tb-edge-installation-3-3-4-1-ubuntu,Ubuntu,shell,resources/3.3.4.1/tb-edge-ubuntu-installation.sh,/docs/user-guide/install/edge/resources/3.3.4.1/tb-edge-ubuntu-installation.sh
tb-edge-installation-3-3-4-1-centos,CentOS,shell,resources/3.3.4.1/tb-edge-centos-installation.sh,/docs/user-guide/install/edge/resources/3.3.4.1/tb-edge-centos-installation.sh{% endcapture %}
{% include tabs.html %}

**NOTE:** Package installer may ask you to merge your tb-edge configuration. It is preferred to use **merge option** to make sure that all your previous parameters will not be overwritten.

Execute regular upgrade script:

```bash
sudo /usr/share/tb-edge/bin/install/upgrade.sh --fromVersion=3.3.4
```
{: .copy-code}

#### Start the service

```bash
sudo service tb-edge start
```
{: .copy-code}

### Docker (Linux or Mac OS) {#docker-linux-mac-3341}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.3.4EDGE version.

Execute the following command to pull **3.3.4.1EDGE** image:
```
docker pull thingsboard/tb-edge:3.3.4.1EDGE
```
{: .copy-code}

Set the terminal in the directory which contains the `docker-compose.yml` file and execute the following command to stop and remove currently running TB Edge container (if it's still running):
```
docker-compose stop
docker-compose rm mytbedge
```
{: .copy-code}

Create docker compose file for ThingsBoard Edge upgrade process:

```text
nano docker-compose-upgrade.yml
```
{: .copy-code}

Add the following lines to the yml file:

```yml
version: '3.0'
services:
  mytbedge:
    restart: on-failure
    image: "thingsboard/tb-edge:3.3.4.1EDGE"
    environment:
      SPRING_DATASOURCE_URL: jdbc:postgresql://postgres:5432/tb-edge
    volumes:
      - ~/.mytb-edge-data:/data
      - ~/.mytb-edge-logs:/var/log/tb-edge
    entrypoint: upgrade-tb-edge.sh
  postgres:
    restart: always
    image: "postgres:12"
    ports:
      - "5432"
    environment:
      POSTGRES_DB: tb-edge
      POSTGRES_PASSWORD: postgres
    volumes:
      - ~/.mytb-edge-data/db:/var/lib/postgresql/data
```
{: .copy-code}

Execute the following command to start upgrade process:
```
docker-compose -f docker-compose-upgrade.yml up
```
{: .copy-code}

Once upgrade process successfully completed, exit from the docker-compose shell by this combination:
```
Ctrl + C
```

Execute the following command to stop TB Edge upgrade container:
```
docker-compose -f docker-compose-upgrade.yml stop
```
{: .copy-code}

Modify 'main' docker compose (`docker-compose.yml`) file for ThingsBoard Edge and update version of the image:

```text
nano docker-compose.yml
```
{: .copy-code}

```yml
version: '3.0'
services:
  mytbedge:
    restart: always
    image: "thingsboard/tb-edge:3.3.4.1EDGE"
...
```

Make sure your image is the set to tb-edge-**3.3.4.1EDGE**.

Execute the following command to up this docker compose directly:
```
docker-compose up
```
{: .copy-code}


### Windows {#windows-3341}

**NOTE**: These steps are applicable for ThingsBoard Edge 3.3.4EDGE version.

#### ThingsBoard Edge package download

Download ThingsBoard Edge package for Windows: [tb-edge-windows-3.3.4.1.zip](https://github.com/thingsboard/thingsboard-edge/releases/download/v3.3.4.1/tb-edge-windows-3.3.4.1.zip).

#### ThingsBoard Edge service upgrade

* Stop ThingsBoard Edge service if it is running:

```text
net stop tb-edge
```
{: .copy-code}

* Make a backup of previous ThingsBoard Edge configuration located in *\<ThingsBoard Edge install dir\>\conf* (for example: *C:\tb-edge\conf*).

* Extract ThingsBoard Edge package.

* Compare and merge your old ThingsBoard Edge configuration files (from the backup you made in the previous step) with new ones.

* Finally, run **upgrade.bat** script to upgrade ThingsBoard Edge to the new version.

**NOTE** Scripts listed below should be executed using Administrator Role.

Execute regular upgrade script:

```text
C:\tb-edge>upgrade.bat --fromVersion=3.3.4
```

#### Start the service

```text
net start tb-edge
```
{: .copy-code}
