# センサーの計測実験

センサーの計測実験は、Arduinoでおこなう。

## 用意するもの

* Arduino IDE
* 土
* センサー
* FaBo Out/In Shield

## 計測方法

[Arduino IDE](https://www.arduino.cc/en/main/software#)をダウンロードし、インストールする。

## 接続

## ソース

```c
void setup() {
  Serial.begin(9600);
  Serial.println("Init");
}

void loop() {
  int analogValue0 = 0;
  analogValue0 = analogRead(A0);
  Serial.print(analogValue0);
  Serial.println("");
  delay(1000);
}
```

