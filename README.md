# Speech Recognition Challenge 2026

학생은 `submission/` 폴더의 **본인 팀 HTML 파일 1개**와, 필요한 영상·음성·이미지를 **배정된 `resource/Team_XX/` 폴더**에 추가한 뒤 Pull Request(PR)로 제출합니다.

팀 번호별 폴더와 자료 업로드 방법은 [팀별 자료 업로드 안내](resource/README.md)를 확인하세요. `XX`는 시트의 Team Name 번호를 두 자리로 쓴 값입니다.

**샘플 페이지의 양식과 내용은 참고만 하세요. 그대로 따라 작성하거나 복사하지 말고, 팀별 프로젝트에 맞게 직접 작성하세요.**

## 제출 파일

파일명은 아래 형식을 사용합니다.

```text
submission/Team_<팀대표이름>_<학번>.html
```

자료 파일은 본인 팀에 배정된 폴더 안에 넣습니다.

```text
resource/Team_XX/
```

### 2. 과제 제출 내용

#### 과제는 HTML 페이지 형태로 구성하며, 아래 항목은 반드시 포함해야 합니다.

<ol>
  <li><strong>메인화면</strong>: <code>index.html</code></li>
  <li><strong>Challenge 설명</strong>: Challenge 개요 및 프로젝트 내용</li>
  <li><strong>Leaderboard</strong>: 벤치마크 결과 및 성능 비교</li>
  <li>개인 GitHub 링크: 아래 항목을 포함한 Repository
    <ol type="a" style="list-style-type: lower-alpha;">
      <li>Baseline 코드</li>
      <li>Dataset(Evaluation용 데이터셋 필수 포함)</li>
      <li>Evaluation: 모델 평가 방법 및 관련 코드</li>
    </ol>
  </li>
</ol>

## 제출 방법

### 1. Fork 및 Clone

GitHub에서 이 저장소를 자신의 계정으로 Fork한 뒤 Clone합니다.

```bash
git clone https://github.com/GITHUB_ID/Speech-Recognition-Challenge-2026.git
cd Speech-Recognition-Challenge-2026
git remote add upstream https://github.com/LSH-Ajou/Speech-Recognition-Challenge-2026.git
```

이미 Fork한 저장소가 있다면 GitHub의 **Sync fork**로 수업 저장소의 최신 변경사항을 반영한 후 작업합니다. 본인 팀 자료 폴더가 보이는지 확인하세요.

### 2. Branch 및 제출 파일 준비

팀 대표 이름과 학번을 사용해 Branch와 제출 파일을 만듭니다.

```bash
git switch -c submission/team-name-studentid
```

`submission/Team_NAME_STUDENTID.html` 파일을 만들거나 기존 제출 HTML을 수정합니다. 필요한 영상·음성·이미지는 배정된 `resource/Team_XX/`에 넣습니다.

### 3. Commit 및 Push

```bash
git add submission/Team_NAME_STUDENTID.html
git add resource/Team_XX/
git commit -m "submission: add Team_NAME_STUDENTID"
git push -u origin submission/team-name-studentid
```

`NAME`과 `STUDENTID`는 팀 대표의 실제 정보로, `XX`는 배정된 두 자리 팀 번호로 바꿉니다. 자료 파일이 없으면 두 번째 `git add` 명령은 생략합니다.

수정이 허용되는 범위는 **본인 팀의 제출 HTML 파일 1개와 배정된 `resource/Team_XX/` 내부**입니다. 다른 팀의 HTML·자료, 공용 `index.html`, 공용 안내문은 수정하지 않습니다.

### 4. Pull Request 제출

GitHub에서 **Compare & pull request**를 선택하고 아래 대상으로 PR을 만듭니다.

```text
base repository: LSH-Ajou/Speech-Recognition-Challenge-2026
base branch: main
head repository: GITHUB_ID/Speech-Recognition-Challenge-2026
compare branch: submission/team-name-studentid
```

PR 제목:

```text
[Submission] Team_NAME_STUDENTID
```

수정 요청을 받으면 같은 Branch에서 수정한 뒤 다시 Commit하고 Push합니다. 기존 PR에 자동으로 반영됩니다.
