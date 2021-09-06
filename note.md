# 虛擬機伺服器管理
- 登入ip: _10.11.0.156_
- 帳號/密碼: _ubuntu548/ubuntu548_

## 常用服務
### _influxDB 2.0_
> 用於紀錄資料: VCP-30 PPR電流、ENG-10(化金)析出電流、
> 各設備ADC Sensor(電流、G-sensor、東元G-sensor)

- http://10.11.0.156:8087 管理介面
- 帳號/密碼: _171104/crew1274_
#### _啟動指令_
 ```sh
cd /home/ubuntu548/influxdb2-2.0.3_linux_amd64/
nohup  ./influxd --http-bind-address=:8087 --engine-path=/lvmdata/influxdbv2 > /dev/null &
```
