# Animal League - 교수님이 던지는 학점 피하기

교수님이 던지는 학점을 피하며 최대한 오래 살아남는 웹 미니게임입니다.
학교를 선택하고 플레이하면 점수가 저장되어 학교별 랭킹을 확인할 수 있습니다.

▶ 플레이: https://k1mg0eun.github.io/Animal_League/

## 게임 방법

- 웹: 방향키 또는 WASD로 이동
- 모바일: 터치로 이동
- A / B 학점 → HP 회복
- C / D 학점 → HP 감소
- F 학점 → 즉사
- 시험기간에는 세이프존에서 F를 피하세요

## 파일 구성

| 파일 | 설명 |
|------|------|
| `index.html` | 게임 본체 (HTML / CSS / JS 단일 파일) |
| `5.0.html` | 이전 버전 |
| `firebase-config.js` | Firebase 설정 (git에 올라가지 않음) |
| `firebase-config.example.js` | Firebase 설정 템플릿 |
| `*.png`, `bgm.mp3`, `neodgm.woff*` | 이미지, 배경음악, 폰트 리소스 |

## 로컬 실행

1. `firebase-config.example.js`를 `firebase-config.js`로 복사하고 Firebase 콘솔의 값을 채웁니다.
2. ES 모듈을 사용하므로 파일을 직접 열지 말고 로컬 서버로 실행합니다.

```bash
python3 -m http.server 8000
```

3. 브라우저에서 `http://localhost:8000` 을 엽니다.

## 기술 스택

- Vanilla HTML / CSS / JavaScript (Canvas)
- Firebase Firestore (점수 저장 및 학교별 랭킹)
- Neo둥근모 폰트
