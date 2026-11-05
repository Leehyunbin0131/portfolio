# LEE HYUN BIN

[GitHub](https://github.com/Leehyunbin0131) ·
[Email](mailto:leehyunbin0131@gmail.com)

## About Me

<img src="assets/about-me-header.svg" alt="From code to motion. — 코드에서 로봇의 움직임으로" width="100%">

<table>
  <tr>
    <td align="center" valign="top">
      <picture>
        <source media="(max-width: 600px)" srcset="assets/profile.jpg" width="110">
        <img src="assets/profile.jpg" alt="LEE HYUN BIN 프로필 사진" width="220">
      </picture>
    </td>
    <td valign="top">
      <p><strong>자율주행 · SLAM · 서비스 로봇</strong></p>
      <p>
        <img src="assets/badge-c.svg" alt="C" height="24">
        <img src="assets/badge-python.svg" alt="Python" height="24">
        <img src="assets/badge-ros2.svg" alt="ROS 2" height="24">
      </p>
      <p><strong>학력</strong><br>대구대학교 컴퓨터소프트웨어전공 재학</p>
      <p><strong>활동</strong><br>42경산 4기<br>전자전기공학부 AIS 동아리 회장</p>
    </td>
  </tr>
</table>

### 수상 이력

<table>
  <thead>
    <tr><th scope="col">연도</th><th scope="col">수상</th><th scope="col">대회 · 분야</th></tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>2021</strong></td><td nowrap>🥉 동메달</td>
      <td><strong>전국기능경기대회</strong> · 모바일로보틱스</td>
    </tr>
    <tr>
      <td><strong>2021</strong></td><td nowrap>🥇 금메달</td>
      <td><strong>대구기능경기대회</strong> · 모바일로보틱스</td>
    </tr>
    <tr>
      <td><strong>2020</strong></td><td nowrap>🥈 은메달</td>
      <td><strong>대구기능경기대회</strong> · 모바일로보틱스</td>
    </tr>
    <tr>
      <td><strong>2019</strong></td><td nowrap>🥉 동상</td>
      <td><strong>IRC 국제로봇콘테스트</strong> · 자율형보행</td>
    </tr>
  </tbody>
</table>

---

## Projects

### Oh-My-MobileRobot

<img src="assets/oh-my-mobilerobot.png" alt="Oh-My-MobileRobot 기본 베이스와 적재함·로봇암·디스플레이 확장형 CAD 렌더링" width="640">

<p>
  <img src="assets/badge-solidcraft.svg" alt="SolidCraft" height="24">
  <img src="assets/badge-python.svg" alt="Python" height="24">
  <img src="assets/badge-urdf-xacro.svg" alt="URDF/Xacro" height="24">
  <img src="assets/badge-ros.svg" alt="ROS" height="24">
  <img src="assets/badge-ros2.svg" alt="ROS 2" height="24">
  <img src="assets/badge-rviz.svg" alt="RViz" height="24">
</p>

- **기간:** 2026.10 ~ 2026.11
- **개발:** 개인 프로젝트
- **현재 상태:** 기본 베이스·확장형 CAD 설계, 부품별 출력 파일 및 ROS 모델 공개
- **코드·설계:** [GitHub](https://github.com/Leehyunbin0131/Oh-My-MobileRobot)

<details>
<summary>프로젝트 자세히 보기</summary>

#### 설계 목표

하나의 모바일 로봇 베이스를 바탕으로 부품 배치와 상부 모듈을 용도에 맞게 바꿀 수 있도록 설계했습니다.
기구 설계 파일과 출력용 부품, ROS 모델을 함께 정리해 하드웨어 구성과 소프트웨어 좌표계를 연결하고자 했습니다.

#### 기구 설계

2020 알루미늄 프로파일을 사용해 외곽 440 × 400 × 140 mm의 프레임을 구성했습니다.
구동 바퀴 2개와 후방 캐스터 2개를 배치하고, 4분할 상판·측면 커버·센서 고정부·2층 전장판을 설계했습니다.
부품별 CAD 원본, 출력용 STL과 도면을 제공하며, 기본 베이스 위에 적재함·로봇암·안내 디스플레이를 올린 확장 개념 모델도 구성했습니다.

#### ROS 모델 연계

기본 베이스와 확장형 3종이 공통 Xacro와 메시를 공유하도록 구성했습니다.
구동 바퀴와 캐스터의 회전 관절, 라이다·카메라 좌표계를 정의하고 ROS 1·ROS 2용 RViz 실행 설정을 제공했습니다.
Python으로 CAD에서 시각화 메시와 URDF를 생성하는 변환 도구를 만들고,
원본 파일 일치 여부·메시 무결성·관절 구조·센서 축을 확인하는 검사 코드도 함께 작성했습니다.

#### 결과

기구 설계부터 출력 파일, ROS 모델과 사용 문서까지 하나의 저장소로 정리했습니다.
확장형은 개념 모델이며, ROS 패키지는 형상·관절·좌표계를 확인하는 용도로 구성했습니다.
실제 주행을 위한 제어·센서 연동과 동역학 시뮬레이션 설정은 사용하는 하드웨어에 맞춰 추가하는 구조입니다.

</details>

---

### claude-ros2-skills

<img src="assets/claude-ros2-skills.png" alt="claude-ros2-skills 프로젝트 배너" width="640">

<p>
  <img src="assets/badge-python.svg" alt="Python" height="24">
  <img src="assets/badge-ros2-jazzy.svg" alt="ROS 2 Jazzy" height="24">
  <img src="assets/badge-claude-code.svg" alt="Claude Code" height="24">
  <img src="assets/badge-codex.svg" alt="Codex" height="24">
</p>

- **기간:** 2026.07 ~ 진행 중
- **개발:** 개인 프로젝트
- **현재 상태:** 스킬과 진단 도구 구현, 실제 로봇 적용 예정
- **코드:** [GitHub](https://github.com/Leehyunbin0131/claude-ros2-skills)

<details>
<summary>프로젝트 자세히 보기</summary>

#### 시작 계기

AI를 활용해 ROS 2 코드를 작성하면서, 코드가 오류 없이 실행되어도 로봇이 예상과 다르게
동작하는 경우를 여러 번 겪었습니다. 그때마다 실행 결과를 설명하고 수정을 요청해야 했습니다.
이런 시행착오를 줄이고, 실제 개발에 도움이 되는 스킬을 `SKILL.md` 형식으로 직접 만들어 보고자 프로젝트를 시작했습니다.

#### 문제와 목표

개발 요청만으로는 실제 하드웨어 구성이나 센서 장착 방향을 AI가 알기 어려웠습니다.
개발 전에 로봇의 구성과 설정을 확인하고,
구현 후에는 실제 로봇이 의도대로 동작하는지 점검하도록 돕는 것이 목표입니다.

#### 진행 방식

필요한 점검 항목을 스킬 문서로 정리하고, Python으로 진단 도구를 구현했습니다.
문서와 코드 작성에는 AI 코딩 도구를 사용했으며, 각 도구의 동작을 확인하기 위한 테스트도 작성했습니다.

#### 핵심 구현

테스트가 실제로 실행되었는지 확인하는 도구와 좌표계(TF), 통신 설정(QoS),
센서 데이터를 점검하는 도구를 구현했습니다.
데이터가 부족한 경우에는 ‘판정 불가’로 표시합니다.
검증 기록을 저장하고 파일 변경 여부를 확인하는 기능도 추가했습니다.

#### 결과

현재는 스킬과 진단 도구를 구현한 상태이며, 실제 로봇 개발에는 아직 적용하지 않았습니다.
다음 로봇 프로젝트에 직접 적용해 개발에 도움이 되는지 확인하고,
필요한 부분을 개선할 예정입니다.

</details>

<!-- 새로운 프로젝트는 위와 같은 형식으로 아래에 추가합니다. -->
