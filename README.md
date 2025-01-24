# 💳 Woori Card Data Analyzing
| **Install ELK in ubuntu and practice ELK using Woori card data**
<br></br>

## ⚙️ How to install ELK in ubuntu
<p></p>
<p></p>

### 1. Install ELK ⬇️
```bash
-- Elastic Search Install
wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -

echo "deb https://artifacts.elastic.co/packages/7.x/apt stable main" | sudo tee -a /etc/apt/sources.list.d/elastic-7.x.list

sudo apt update
sudo apt install elasticsearch=7.17.10

sudo systemctl enable elasticsearch
sudo systemctl start elasticsearch


-- Logstash Install
wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -
sudo sh -c 'echo "deb https://artifacts.elastic.co/packages/7.x/apt stable main" > /etc/apt/sources.list.d/elastic-7.x.list'
sudo apt update

sudo apt install -y logstash
logstash --version

sudo systemctl start logstash
sudo systemctl enable logstash


-- Kibana Install
echo "deb https://artifacts.elastic.co/packages/7.x/apt stable main" | sudo tee /etc/apt/sources.list.d/elastic-7.x.list
sudo apt update
sudo apt install kibana=7.17.10 -y
```
<p></p>
<br></br>

### 2. Elasticsearch, Kibana yml 설정 ⚙️

- elasticsearch.yml 수정
```yml
# ---------------------------------- Network -----------------------------------
#
# By default Elasticsearch is only accessible on localhost. Set a different
# address here to expose this node on the network:
#
network.host: 0.0.0.0
#
# By default Elasticsearch listens for HTTP traffic on the first free port it
# finds starting at 9200. Set a specific HTTP port here:
#
http.port: 9200
```

- kibana.yml 수정
```yml
# Specifies the address to which the Kibana server will bind. IP addresses and host names are both valid values.
# The default is 'localhost', which usually means remote machines will not be able to connect.
# To allow connections from remote users, set this parameter to a non-loopback address.
server.host: 0.0.0.0


# The URLs of the Elasticsearch instances to use for all your queries.
elasticsearch.hosts: ["http://localhost:9200"]
```
<p></p>
<br></br>

### 3. 포트 포워딩 🔌


- ubuntu에서 해당 포트에 대해 모두 포워딩 설정
<img src="./img/port.png" alt="Port Image" width="500"/>
<br>
<br>
<p></p>

### 4. 정상 실행 확인 🚀
<br>
<br>

- elastic search 확인
<img src="./img/es.png" alt="es Image" width="500"/>
<br>
<br>

- Kibana 확인
<br>
<img src="./img/kibana.png" alt="Kibana Image" width="500"/>
<br>
<br>

-> EK, Kibama 모두 정상적으로 실행되는 것 확인 완료
<br>
<br>

### 5. Trouble Shooting 💥
<br>
<br>
<details>
  <summary><span style="font-size: 18px;">문제 1: IP 와 port도 모두 열어줬지만 ES가 실행이 되지 않음을 확인</span></summary>
  해결 방법: 시스템 로그 확인 후, Logstash 설정 파일 오류 수정
</details>

<details>
  <summary><span style="font-size: 18px;">문제 2: Elasticsearch 연결 오류</span></summary>
  해결 방법: Elasticsearch와 Logstash의 네트워크 설정 확인
</details>

<details>
  <summary><span style="font-size: 18px;">문제 3: Logstash 필터 오류</span></summary>
  해결 방법: 필터 구문 오류를 수정하고, 로그를 다시 확인
</details>



<br></br>
# 👀 Hands On
