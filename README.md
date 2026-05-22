# Web Deploy

## 업로드 대상

```text
web/index.html -> /www/app/index.html
web/app.js     -> /www/app/app.js
web/.htaccess  -> /www/app/.htaccess
```

## 확인 URL

```text
./app/?v=4.1.8
```

## 체크리스트

- `index.html`이 중간에서 잘리지 않았는지 확인합니다.
- `app.js` 크기가 너무 작지 않은지 확인합니다.
- `.htaccess`가 숨김 파일이라 누락되지 않았는지 확인합니다.
- 브라우저 개발자도구 콘솔에서 `Unexpected end of input`이 없어야 합니다.
- CSP 오류가 나면 `/www/app/.htaccess` 업로드 여부를 먼저 확인합니다.
