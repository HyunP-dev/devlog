# VS에서의 libewf 빌드

1. [libyal/libewf](https://github.com/libyal/libewf) 에서 릴리즈를 받아 푼다.
2. 압축을 푼 폴더가 있는 위치에 zlib과 bzip2를 똑같이 받아 푼다. (각각 이름을 zlib, bzip2로 해야 함.)
3. libewf의 msvscpp에서 솔루션을 연다.
4. 솔루션의 bzip2 프로젝트의 속성에서 `링커 > 입력 > 모듈 정의 파일` 을 bzip2 폴더 안에 있던 libbz2.def로 지정한다.
5. 빌드한다.
