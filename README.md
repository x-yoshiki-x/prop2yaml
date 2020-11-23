### How to Use

- right click to "Convert properties to yaml"

### example

```properties
spring.datasource.driver-class-name=com.mysql.jdbc.Driver
spring.datasource.url=jdbc:mysql://cent7.a5.jp:3306/stemmdoc?useSSL=false&zeroDateTimeBehavior=convertToNull
spring.datasource.username=root
spring.datasource.password=1

hoge.fuga[0].aga.aaa[0] = 000
hoge.fuga[0].aga.aaa[1] = 001
hoge.fuga[0].iga = 002
hoge.fuga[1].aga.aaa[0] = 100
hoge.fuga[1].aga.aaa[1] = 101
hoge.fuga[1].iga = 102
hoge.fuga[1].mega.uga = 102
hoge.fuga[1].giga.uga.ega = 102
hoge.list[0].aga = 301
hoge.list[0].iga = 302
hoge.list[1].aga = 401
hoge.list[1].iga = 402
hoge.num[0] = 201
hoge.num[1] = 202
age.num[0].itu[0] = 201
age.num[0].itu[1] = 202
age.kum[0].itu = 201
age.kum[1].itu = 202
```

```YAML
spring:
  datasource:
    driver-class-name: com.mysql.jdbc.Driver
    url: jdbc:mysql://cent7.a5.jp:3306/stemmdoc?useSSL=false&zeroDateTimeBehavior=convertToNull
    username: root
    password: 1
hoge:
  fuga:
    - aga:
        aaa:
          - 000
          - 001
      iga: 002
    - aga:
        aaa:
          - 100
          - 101
      iga: 102
      mega:
        uga: 102
      giga:
        uga:
          ega: 102
  list:
    - aga: 301
      iga: 302
    - aga: 401
      iga: 402
  num:
    - 201
    - 202
age:
  num:
    - itu:
      - 201
      - 202
  kum:
    - itu: 201
    - itu: 202
```
