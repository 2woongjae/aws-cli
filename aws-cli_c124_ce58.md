# aws-cli 설치


> 본 교재는 OS X El Capitan 10.11.5 에서 진행되었음.


Mac(또는 Linux)에서 AWS 명령줄 인터페이스(CLI) 를 설치하려면, **Python 2.6.5 이상**이 필요하다. **pip**를 사용하여 설치한다.

```
pip install awscli
```

* 요즘 맥에는 대부분 python 2.7 이상이 기본으로 설치되어 있기 때문에 그냥 바로 진행해도 된다. 하지만 필자는 파이썬 버전 관리를 위해 [pyenv](https://github.com/yyuu/pyenv) 를 이용한다.
* AWS CLI는 Amazon Linux AMI에 미리 설치되어 제공된다.

