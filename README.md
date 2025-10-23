# **코리아 IT 아카데미 국비과정** 
## AWS-Spring 😺
<a name="readme-top"></a> 


#### 설치 과정
  > sudo passwd
> 
  > 1234
> 
  > sudo apt update && sudo apt upgrade -y
> 
  > sudo apt install -y tzdata
> 
  > sudo dpkg-reconfigure tzdata
> 
  > sudo date
> 
  > export TZ=Asia/Seoul
> 
  > sudo apt-get install openjdk-17-jdk (창 나오면 엔터 혹은 →, 엔터)
> 
  > vim ~/.bashrc
> 

  최하단에 추가

  export JAVA_HOME=$(dirname $(dirname $(readlink -f $(which java))))
  
  export PATH=$PATH:$JAVA_HOME/bin

  > source ~/.bashrc
> 
  > echo $JAVA_HOME
> 

  > sudo fallocate -l 2G /swapfile
> 
  sudo chmod 600 /swapfile
  
  > sudo mkswap /swapfile
> 
  > sudo swapon /swapfile
> 
  > echo '/swapfile none swap sw 0 0' | sudo tee -a /etc/fstab
> 
  > free -h
> 

  > git clone
> 
  > chmod +x ./gradlew
> 
  > ./gradlew build
> 
  > java -jar build/libs/app.jar
> 

  > sudo apt install iptables-persistent
> 
  > sudo iptables -t nat -A PREROUTING -p tcp --dport 80 -j REDIRECT --to-ports 10000
> 
  > sudo chmod 777 /etc/iptables/rules.v4
> 
  > sudo iptables-save > /etc/iptables/rules.v4
> 
  > cat /etc/iptables/rules.v4
> 
