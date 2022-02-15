# JDK Installation

If you want to get help regarding our products or just want to ask something, join our [discord](https://discord.gg/MUCKhgFUCA).

#### Linux Update
```
sudo apt update && sudo apt upgrade -y
```

#### Add the additionals packets
```
sudo apt-get install software-properties-common
```

#### Java 8
```linux
sudo apt-get install openjdk-8-jdk -y
```

#### Java 11
```linux
sudo apt-get install openjdk-11-jdk -y
```

####  Java 16
```linux
wget -O- https://apt.corretto.aws/corretto.key | sudo apt-key add -
sudo add-apt-repository 'deb https://apt.corretto.aws stable main'
sudo apt-get update
sudo apt-get install -y java-16-amazon-corretto-jdk
```

#### Java 17
```linux
wget -O- https://apt.corretto.aws/corretto.key | sudo apt-key add -
sudo add-apt-repository 'deb https://apt.corretto.aws stable main'
sudo apt-get update
sudo apt-get install -y java-17-amazon-corretto-jdk
```

#### Check the java version 
```linux
java -version
```

#### If the java version is not correct, type and set the specify version
```linux 
sudo update-alternatives --config java
```

# Uninstalling all Java version
```linux
sudo apt purge java-common -y
sudo apt autoremove -y
```

# RPM-Based

#### DFN
```linux
sudo rpm --import https://yum.corretto.aws/corretto.key
sudo curl -Lo /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo
sudo dnf -y install java-17-amazon-corretto-devel
```

#### zypper
```
sudo zypper addrepo https://yum.corretto.aws/corretto.repo
sudo zypper refresh
sudo zypper install java-17-amazon-corretto-devel
```

#### Yum
```
sudo rpm --import https://yum.corretto.aws/corretto.key
sudo curl -Lo /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo
sudo yum -y install java-17-amazon-corretto-devel
```

#### Arch linux
```
sudo pacman -Syu jdk-openjdk
```
