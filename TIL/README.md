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