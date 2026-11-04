# 팀별 자료 업로드 안내

프로젝트 HTML에서 사용할 영상·음성·이미지는 **본인 팀에 배정된 `resource/Team_XX/` 안에** 넣습니다. `XX`는 시트의 **Team Name** 번호를 두 자리로 쓴 값입니다. 제출 여부와 관계없이 1~18팀 폴더를 준비했습니다.

## 팀별 폴더

| 팀 번호 | 팀원 | 업로드 폴더 |
| --- | --- | --- |
| 1 | 박성재 | [resource/Team_01/](Team_01/) |
| 2 | Kyi Sin Tun, Aye Chan Phyo | [resource/Team_02/](Team_02/) |
| 3 | 이재왕, 박재현 | [resource/Team_03/](Team_03/) |
| 4 | 김현민, 김민균, 송민혁 | [resource/Team_04/](Team_04/) |
| 5 | SHIRUIQING | [resource/Team_05/](Team_05/) |
| 6 | 조용준 | [resource/Team_06/](Team_06/) |
| 7 | 최평화, 임종혁 | [resource/Team_07/](Team_07/) |
| 8 | 이다혜 | [resource/Team_08/](Team_08/) |
| 9 | 장봉현 | [resource/Team_09/](Team_09/) |
| 10 | 황준서 | [resource/Team_10/](Team_10/) |
| 11 | 김지훈 | [resource/Team_11/](Team_11/) |
| 12 | 정현민 | [resource/Team_12/](Team_12/) |
| 13 | 강연우 | [resource/Team_13/](Team_13/) |
| 14 | 김민승 | [resource/Team_14/](Team_14/) |
| 15 | 황재현 | [resource/Team_15/](Team_15/) |
| 16 | 김진수 | [resource/Team_16/](Team_16/) |
| 17 | 허준영 | [resource/Team_17/](Team_17/) |
| 18 | 박준형 | [resource/Team_18/](Team_18/) |

팀 번호가 배정되지 않은 제출자는 임의로 새 팀 번호를 만들지 말고 담당자에게 업로드 폴더를 확인하세요.

## 디렉토리와 파일명

아래는 [Sample HTML](../submission/Team_sample_202624123.html)을 기준으로 한 디렉토리 예시입니다. 예시의 `Team_sample/` 대신 실제 팀은 위 표에 배정된 `Team_01/`~`Team_18/` 폴더를 사용합니다.

```text
Speech-Recognition-Challenge-2026/
├── index.html
├── submission/
│   └── Team_sample_202624123.html
└── resource/
    ├── README.md
    ├── Team_sample/         # Sample HTML의 자료 폴더 예시
    │   ├── sample.wav
    │   ├── demo.mp4
    │   └── pipeline.png
    ├── Team_01/
    ├── ...
    └── Team_18/
```

## 자료 경로와 공개 주소

`audio/` 같은 하위 폴더를 만들었다면 `../resource/Team_06/audio/sample.wav`처럼 실제 위치를 반영합니다. `/resource/...`처럼 슬래시로 시작하거나 `C:\...` 같은 내 컴퓨터 경로를 넣으면 수업 GitHub Pages에서 연결되지 않습니다.

자료를 수업 저장소에 머지하고 Pages 배포가 완료되면 다음 주소에서도 접근할 수 있습니다. 아래 파일명은 예시이며 실제 파일을 올려야 열립니다.

```text
https://lsh-ajou.github.io/Speech-Recognition-Challenge-2026/resource/Team_06/sample.wav
https://lsh-ajou.github.io/Speech-Recognition-Challenge-2026/resource/Team_06/demo.mp4
```

## 업로드 및 PR 제출 순서

1. 본인 Fork에서 **Sync fork**를 눌러 수업 저장소의 최신 변경사항을 반영합니다.
2. 본인 Fork의 작업 브랜치에서 배정된 `resource/Team_XX/` 폴더를 엽니다.
3. GitHub 웹의 **Add file → Upload files**로 자료를 올리거나, 로컬에서 파일을 복사한 후 commit·push합니다.
4. **받는 저장소가 `LSH-Ajou/Speech-Recognition-Challenge-2026`, base 브랜치가 `main`**인 PR을 만듭니다. head는 본인 Fork의 작업 브랜치로 선택합니다.
5. 변경 파일 목록에 본인 팀 HTML(최대 1개)과 본인 팀 자료 폴더의 파일만 포함됐는지 확인합니다. 자료만 갱신하는 PR도 같은 범위를 지킵니다.

본인 Fork 내부에서만 PR을 생성·머지하면 수업 저장소에는 반영되지 않습니다. 상세한 Git 명령은 [기본 제출 안내](../README.md)를 참고하세요.

