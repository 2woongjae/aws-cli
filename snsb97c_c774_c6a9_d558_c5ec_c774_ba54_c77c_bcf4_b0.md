# SNS를 이용하여 이메일 보내기

전체적인 명령어의 전개는 다음과 같다.

* **Topic** 을 만들고,
* 그 안에 이메일을 발송하는 **Subscription** 을 만든다.
* **Publish** to topic으로 제목과 내용을 입력하여 발송한다.

바로 시작해보자!

SNS는 리전 단위의 서비스이다. 자신의 리전이 어디인지 생각해보고 진행하도록~!



---
```
aws> sns list-topics
{
    "Topics": []
}
```
> 현재 리전의 전체 토픽의 리스트를 리턴하는 명령이다. 당연히 그전에 아무것도 안해봤으면 저렇게 나온다.

---
```
aws> sns create-topic --name TestTopic
{
    "TopicArn": "arn:aws:sns:ap-northeast-2:961228086927:TestTopic"
}
```
> 토픽의 이름을 지정하여 새 토픽을 만드는 명령이다. 성공적으로 만들어지면, arn 을 리턴해준다.

---
```
aws> sns list-topics
{
    "Topics": [
        {
            "TopicArn": "arn:aws:sns:ap-northeast-2:961228086927:TestTopic"
        }
    ]
}
```

> 다시 한번 토픽의 리스트를 확인해보자. 처음과 다르게 만든 토픽을 볼 수 있다.

---



