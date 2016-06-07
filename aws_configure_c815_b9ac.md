# aws configure 정리

```
LeeWoongjaeui-MacBook-Air:~ leewoongjae$ aws configure
AWS Access Key ID [****************CHPA]: 
AWS Secret Access Key [****************DJMj]: 
Default region name [ap-northeast-1]: 
Default output format [None]: 
```

> 옵션없이 사용하면, default 프로파일의 값들을 설정한다.

```
LeeWoongjaeui-MacBook-Air:~ leewoongjae$ aws configure --profile vtouch-logs
AWS Access Key ID [****************MLBA]: 
AWS Secret Access Key [****************8QG4]: 
Default region name [ap-northeast-2]: 
Default output format [None]: 
```

  > --profile 옵션을 사용하면, 해당 프로파일의 값들을 설정한다. (기존에 프로파일이 없는 경우는 설정 값을 지정하면서 프로파일을 새로 만든다.)

```
LeeWoongjaeui-MacBook-Air:~ leewoongjae$ aws configure list
      Name                    Value             Type    Location
      ----                    -----             ----    --------
   profile                <not set>             None    None
access_key     ****************CHPA shared-credentials-file    
secret_key     ****************DJMj shared-credentials-file    
    region           ap-northeast-1      config-file    ~/.aws/config
```

> 옵션없이 사용하면, default 프로파일의 설정 값을 보여준다.

```
LeeWoongjaeui-MacBook-Air:~ leewoongjae$ aws configure list --profile vtouch-logs
      Name                    Value             Type    Location
      ----                    -----             ----    --------
   profile              vtouch-logs           manual    --profile
access_key     ****************MLBA shared-credentials-file    
secret_key     ****************8QG4 shared-credentials-file    
    region           ap-northeast-2      config-file    ~/.aws/config
```

> --profile 옵션을 사용하면, 해당 프로파일의 설정 값을 보여준다.



