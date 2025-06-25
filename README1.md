### 1️⃣ Install Java

```bash
sudo apt update -y
sudo apt install openjdk-21-jdk -y

# Verify
java -version
javac -version
```

### 2️⃣ Install Maven

```bash
sudo apt update -y
sudo apt install maven -y

# Verify
mvn -version
```

### 3️⃣ Install Docker

```bash
# Run official Docker install script
curl -fsSL https://get.docker.com | bash

# Set permissions
sudo chmod 777 /var/run/docker.sock

# Verify
docker --version
```

### 4️⃣ Set Java and Maven Environment Paths

```bash
nano ~/.bashrc
```

Add the following lines at the end of the file:

```bash
# Java
export JAVA_HOME=/usr/lib/jvm/java-21-openjdk-amd64
export PATH=$JAVA_HOME/bin:$PATH

# Maven
export MAVEN_HOME=/usr/share/maven
export PATH=$MAVEN_HOME/bin:$PATH
```

Apply changes:

```bash
source ~/.bashrc

# Verify
echo $JAVA_HOME
echo $MAVEN_HOME
```
