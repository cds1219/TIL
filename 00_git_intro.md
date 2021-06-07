# Git 초기 설정

커밋 작성자(author) 설정

``` bash
$ git config --global user.email "메일주소"
$ git config --global user.name "유저이름"
```

- 커밋을 작성하는 사람이 누구인지 알아야하기 때문

---

지정된 설정 확인

```bash
$ git config --global -l
# $ git config --global -list
```

---

**커밋 편집기 변경**

```bash
$ git config --global core.editor "code --wait"
```

- 해당 명령어는 반드시 vscode가 설치되어 있어야 함

> 기본 텍스트 편집기 `vim`을 `vscode`로 대체하는 것

---

## Git Basic

### 로컬 저장소 설정

```bash
$ git init
```

- 폴더에 git 저장소를 초기화하면,
  `.git` 숨김 폴더가 생기고 bash에는 (master)라고 표기 된다.

> 주의사항
>
> ​	git 저장소 내에 다른 git 저장소를 만들면 안됨!
>
> ​	git init 명령어를 입력할 때, (master)가 있으면 절대 입력하지 말 것

---

### add

> staging area / INDEX

```bash
$ git add 파일명
$ git add . #현재 디렉토리 (하위 디렉토리)
$ git add a.txt # 특정 파일
$ git add my_folder/ # 특정 폴더
```

- working directory 상태의 파일을 standig area 상태로 변경
- 커밋을 위한 파일 및 폴더들을 추가하는 명령어



