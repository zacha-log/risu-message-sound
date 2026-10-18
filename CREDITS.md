# 라이선스 및 음원 출처

대상: 메시지 알림음 조절 플러그인 v1.36.0

## 플러그인 코드

플러그인 코드 및 포함된 DSP 스크립트: **GPL-3.0-only**.
라이선스 전문은 함께 배포하는 `LICENSE`를 참고하세요.
음원별 조건은 아래와 같이 별도로 적용됩니다. 플러그인 전체가 CC0인 것은 아닙니다.

## RisuAI 기본 메시지음

- 파일: RisuAI의 `src/etc/send.mp3`
- 출처: https://github.com/kwaroran/Risuai/blob/1db1199eef3575af9b52e8a85e83e3d333488933/src/etc/send.mp3
- 저장소 저작권 표시: Copyright (C) 2024 Kwaroran
- 저장소 라이선스: GPL-3.0
- 음원 자체의 원작자와 별도 이용 조건은 독립적으로 확인되지 않았습니다. 저장소 라이선스만으로 제3자 음원의 권리 관계까지 보장되지는 않습니다. 이 음원을 CC0로 표시하지 않습니다.
- 처리: 원본 인코딩 데이터 유지, 재생 시 끝부분 페이드 적용.

## 외부 녹음 음원 — CC0

다음 외부 음원은 각 출처에서 CC0로 공개된 녹음본을 사용했습니다.
CC0 조건: https://creativecommons.org/publicdomain/zero/1.0/
개별 음원 출처 표기는 CC0의 의무가 아니며, 이 목록은 출처 확인을 위해 제공합니다.

| 사용 항목 | 원본 / 제작자 | 출처 |
| --- | --- | --- |
| 도장 · 짧게 찍기 | es-stamp.wav / eddies2000 | https://freesound.org/people/eddies2000/sounds/448474/ |
| 스위치 · 딸깍 및 ON/OFF 조작음 | light_switch10 / funkysandwich | https://freesound.org/people/funkysandwich/sounds/870289/ |
| 타자 · 세 번 / 두 번 | Keyboard Soundpack #1 [Typing and Single Keystrokes] / unicaegames | https://opengameart.org/content/keyboard-soundpack-1-typing-and-single-keystrokes |
| 종이 · 앞으로 넘기기 | Flipping Page Forward / Ym_The_Cosmic | https://freesound.org/people/Ym_The_Cosmic/sounds/858468/ |
| 필기 · 펜 | Writing on paper / AkiYaSuShi | https://freesound.org/people/AkiYaSuShi/sounds/830323/ |

### 편집 내용

- 도장: 짧은 구간 추출, 레벨 조정, 끝부분 페이드.
- 스위치: 레벨 조정 및 기존 끝부분 페이드 유지. 꺼짐음은 두 반음 낮게 재생. 알림음은 꺼짐음과 켜짐음을 100ms 간격으로 연결. ON/OFF 조작음과 알림음의 음량은 별도 설정.
- 타자: `keypress-001.wav`, `keypress-007.wav`, `keypress-014.wav`를 사용해 두 번/세 번 입력 배열 구성, 레벨 및 끝부분 처리.
- 종이: 고음 완화, 약한 구간의 배경 잡음 감소, 레벨 조정 및 끝부분 페이드. 원본 길이와 피치 유지.
- 필기: 원본 앞 1.6초 사용, 배경 잡음 감소, 고음 완화, 레벨 조정 및 끝 0.8초 페이드.

Freesound 음원은 공개 HQ MP3 미리듣기 파일을 가공했습니다. 로그인이 필요한 원본 다운로드 파일을 사용했다는 의미는 아닙니다.
외부 녹음본은 플러그인 안에 포함되며, 재생 시 외부 서버에서 음원을 내려받지 않습니다.

## 아이콘 및 사용자 음원

- UI 아이콘은 플러그인 코드에 직접 작성한 인라인 SVG이며, 코드와 같은 GPL-3.0-only로 제공합니다.
- 사용자가 직접 불러오는 음원은 이 출처 목록에 포함되지 않습니다. 해당 음원의 이용 조건은 사용자가 확인해야 합니다.

## Update distribution

Version 1.36.0 adds the update URL https://raw.githubusercontent.com/zacha-log/risu-message-sound/main/risu-message-sound.js. All audio and playback behavior unchanged.
