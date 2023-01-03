# TIL

### Windows Navigator
- `Windows Navigator`통해 URL 복사 기능을 구현할 수 있다.
    ```js
    function copyUrl(url) {
      navigator.clipboard.writeText(url).then(() => {
        console.log('URL copied to clipboard');
      }, (err) => {
        console.error('Failed to copy URL: ', err);
      });
    }
    ```
  
### NextJS에서 환경변수 사용
- 기본적으로 `env.local`을 통해 로드된 모든 환경 변수는 `Node.js`에서만 사용할 수 있는데,
 브라우저에 변수를 사용하려면 변수 앞에 NEXT_PUBLIC_을 붙여야합니다.
- [참고](https://nextjs.org/docs/basic-features/environment-variables#exposing-environment-variables-to-the-browser)