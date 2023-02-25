# GUG
가이드 유니폼 기반 게임 메이커

## 쉽게 만드는 텍스트 게임
JSON 파일을 수정하여 게임을 만들 수 있습니다.


### 커맨드들
커맨드는 기본 범위에 맞게 작성하도록 되어있습니다.
say 명령어를 예시로 보자면,
```
say normal Kim '그 일을 빨리 끝내세요!'
> Kim : 그 일을 빨리 끝내세요!
```
와 같이 사용합니다.
()안의 내용은 일반적으로 str형식의 데이터를 받습니다. ''으로 묶어서 띄어쓰기를 방지할 수 있습니다.
[]안의 내용은 일반적으로 list형식의 데이터를 받습니다.
##### say
```
say normal (talker) (content)
> talker : content
화자가 해당 내용을 말하게 합니다.
```

```
say raw (content)
> content
아무런 화자 없이 내용만을 출력합니다.
```
##### wait
```
wait (second])
▶ second만큼 기다립니다.
```

##### delete
```
delete (int)
▶ int개 만큼 텍스트를 삭제합니다.
```

##### get
```
> get [sequances] [sequances_text]

```
