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

## 특정 문자로 시작하는 엘리먼트 찾기. 

위 내용중에서 'my' 로 시작하는 엘리먼트를 찾아서 색상을 파란색으로 바꾸어 보겠습니다.

형식은 다음과 같습니다. 

```
[attribute^="찾고자하는 문자"]
```

```

<style>
    [class^="my"] {
        color: blue;
    }
</style>
```

이렇게 하면 class 엘리먼트값이 "my" 로 시작하는 모덴 엘리먼트를 파란색으로 바꾸어 줍니다. 

## 측정 문자로 끝나는 엘리먼트 찾기. 

이제는 'Name' 로 끝나는 엘리먼트를 찾아서 폰트 패밀리와 크기를 바꿔 보겠습니다. 

형식은 다음과 같습니다. 

```
[attribute$="찾고자하는 문자"]
```

```
<style>
    [class$="Name"] {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-weight: 800;
    }
</style>
```

이렇게 하면 'Name' 로 끝이나는 엘리먼트의 폰트와 엘리먼트가 변경될 것입니다. 

## 특정 문자가 들어간 모든 엘리먼트 찾기. 

지금까지 시작, 종료 문자열을 찾았습니다. 

이제는 특정 문자가 들어간 모든 엘리먼트를 찾아보겠습니다. 

```
[attribute*="찾고자하는 문자"]
```

```
<style>
    [class*="Bro"] {
        color: red;
        font-style: italic;
    }
</style>
```

이렇게 스타일을 추가하면 'Bro' 라는 단어가 들어간 모든 엘리먼트의 폰트 색상을 붉은색, 이탤릭체로 바꿔줍니다. 

결과를 한번 보겠습니다. 

