
### 1. Go 개발환경 설정

`brew install go` 명령어로 설치하자
Goland를 사용할 것이다.

GOPATH는 아래처럼 설정해두었다.
```shell
> export GOPATH=$HOME
> export PATH=$PATH:$GOPATH/bin

> go env
...
GOPATH="/Users/{USER}/go"
...
```
Goland로 프로젝트를 생성하니 `GOMOD` 값만 변한 것으로 보인다.
```env
GOMOD="/Users/{USER}/GolandProjects/Go/go.mod"
```

### 2. go run

**go run** 명령어는 **go build** 명령어와 똑같이 바이너리를 생성하지만
임시 디렉터리에 만들어진다. 그리고 실행한다. 종료되면 삭제한다.

계속해서 수정하고 실행할땐 go run 명령어로도 충분하다.
실행가능한 바이너리 파일이 필요할 땐 go build가 필요하다.

### 3. go install
