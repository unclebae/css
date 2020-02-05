# css wildcard 이용하기. 

css 를 이용하여 html 에 스타일을 먹일때 동일한 문자열로 시작하는 모든 엘리먼트에 대해서 스타일을 먹이고 싶을 때가 있습니다. 

일일이 css selector 을 나열하기에는 너무 공수가 많이 드는것이 사실입니다. 

이럴때 도움이 되는 셀렉터가 있어 공유하고자 합니다. 

## 기본 HTML 확인하기. 

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Wildcard</title>
</head>
<body>
    <h1> Css Selector </h1>

    <div class="myName">My Name is T-HUB</div>
    <div class="myAge">I'm 3 years old.</div>
    <div class="myHome">I leave in Seoul</div>
    <div class="yourName">Your name is T-HUB</div>
    <div class="yourBrother">Your brother is ... </div>
    <div class="hisBro">His brother is HaHaHa </div>
</body>
</html>
```