# AWS CLI 버전 업그레이드

설치된 awscli 의 버전은 다음과 같이 확인한다.

```
LeeWoongjaeui-MacBook-Air:~ leewoongjae$ aws --version
aws-cli/1.10.34 Python/2.7.11 Darwin/15.5.0 botocore/1.4.24
```

현재 awscli 의 버전은 1.10.34 이다.
최신 릴리즈된 버전은 [출시정보](https://aws.amazon.com/releasenotes/CLI)에서 확인할 수 있다.

업데이트를 위해서는 다음과 같이 pip upgrade 를 통해서 진행하면 된다.

```
LeeWoongjaeui-MacBook-Air:~ leewoongjae$ pip install --upgrade awscli
```

다시 확인하면 다음과 같이 버전이 업그레이드 된 것을 볼 수 있다.

```
LeeWoongjaeui-MacBook-Air:~ leewoongjae$ aws --version
aws-cli/1.10.35 Python/2.7.11 Darwin/15.5.0 botocore/1.4.25
```