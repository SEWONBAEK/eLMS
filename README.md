<div align="center">
  <img src="./images/eLMS_Thumbnail.png" width="80%">
  <h3비대면 과제관리 시스템</h3>
</div>

## ⌨️ 기간

- **2026.01.19 ~ 2026.02.27(5주)**

<a name="tableContents"></a>

<br/>

## 🔎 목차

1. <a href="#subject">🎯 주제</a>
1. <a href="#mainContents">⭐️ 주요 기능</a>
1. <a href="#systemArchitecture">⚙ 시스템 아키텍쳐</a>
1. <a href="#skills">🛠️ 기술 스택</a>
1. <a href="#erd">💾 ERD</a>
1. <a href="#contents">🖥️ 화면 소개</a>
1. <a href="#developers">👥 팀원 소개</a>

<br/>

<!------- 주제 시작 -------->

## 🎯 주제

<a name="subject"></a>

**Ajax** 기반의 실시간 상호작용을 지원하는 비대면 과제 관리 플랫폼<br />
<br />
Ajax를 활용하여 화면 전환(Reload) 없이 과제 등록, 제출, 채점 프로세스를 구현함으로써<br />
웹 성능을 최적화하고 사용자 편의성을 극대화한 프로젝트입니다.

<br />
**주요 기능**


- 과목 등록, 과제 등록 등 모달창을 이용한 Ajax 통신을 이용하여 실시간 데이터 최신화
- 입력 데이터 유효성 검증, 비정상적인 접근 및 파라미터 변조 방지, 서버 측 예외 처리 등
  
<div align="right"><a href="#tableContents">목차로 이동</a></div>

<br/>

<!------- 주요 기능 시작 -------->

## ⭐️ 주요 기능

<a name="mainContents"></a>

### 공통

- 인터셉터를 통해 해당 페이지의 기능을 회원 등급에 맞게 제한합니다.    

---

### 관리자

- 공지사항 작성 및 관리합니다.
- 회원 관리(재학, 휴학, 퇴학, 퇴직 등)를 진행합니다.

---

### 교수

- 해당 교수가 수업할 과목을 등록, 수정, 삭제합니다.
  - 수강 신청한 학생이 있다면 과목 삭제를 제한합니다.
- 수업하는 과목의 과제를 등록, 수정, 삭제합니다.
  - 과제는 백분율 방식과 PASS or FALSE 방식에 맞게 등록할 수 있습니다.
  - 과제를 제출한 학생이 있다면 과제 삭제를 제한합니다.
- 학생이 제출한 과제를 채점 방식에 맞게 채점합니다.

---

### 학생

- 교수가 등록한 과목이 수강 신청 기간안에 포함되어 있다면 수강 신청 가능합니다.
- 수강 신청한 과목이 수강 신청 기간안에 있다면 수강 취소할 수 있습니다.
- 


---


### 구매내역

#### 현재 사용자가 지금까지 구매한 내용을 바탕으로 상품을 추천할 수 있도록 분석합니다.

- 현재 사용자가 구매한 상품의 구매빈도와 구매수량에 대한 가중치를 계산하여 최애 상품을 분석합니다.
- 가중치 점수: (빈도 * 0.7) + (수량 * 0.3)


---


<div align="right"><a href="#tableContents">목차로 이동</a></div>

<br/>


<!------- 시스템 아키텍쳐 시작 -------->

## ⚙ 시스템 아키텍쳐

<a name="systemArchitecture"></a>

<img src="./images/unicook_System Architecture.png">

- Frontend: HTML5, CSS3, JavaScript를 활용하여 깔끔하고 가독성 좋은 UI와 Ajax를 이용한 비동기 통신 환경을 구축 
- Backend & DB: Flask 프레임워크를 사용하여 서버를 구현하였으며, MySQL을 통해 사용자 정보 및 구매 이력 데이터를 관리
- AI Engine: Pandas와 NumPy로 전처리된 데이터를 바탕으로, Scikit-learn의 SVD(특이값 분해) 및 코사인 유사도 알고리즘을 활용해 고도화된 개인화 추천 로직을 수행

본 프로젝트는 Flask 기반의 웹 서버와 Scikit-learn 기반의 AI 추천 엔진을 결합한 지능형 커머스 플랫폼입니다. 사용자 구매 데이터를 분석하여 개인 맞춤형 상품을 추천하는 시스템 아키텍처를 구축하였습니다.

<div align="right"><a href="#tableContents">목차로 이동</a></div>

<br/>

<!------- 기술 스택 시작 -------->

## 🛠️ 기술 스택

<a name="skills"></a>

### 💻 FrontEnd

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![Ajax](https://img.shields.io/badge/Ajax-%23ffffff.svg?style=for-the-badge&logo=jquery&logoColor=black)
![Figma](https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white)
---

### ⚙️ BackEnd

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![Mysql](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mariadb&logoColor=white)
---

### 🤝 Collaboration

![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
---

<div align="right"><a href="#tableContents">목차로 이동</a></div>

<br/>

<!------- ERD 시작 -------->

## 💾 ERD
<a name="erd"></a>
<img src="./images/unicook_ERD.png">

<div align="right"><a href="#tableContents">목차로 이동</a></div>

<br/>

<!------- 화면 소개 시작 -------->

<a name="contents"></a>

<br/>

## 🖥️ 화면 소개

### 1. 메인 페이지

<table>
    <tr>
        <td align="center" width="200">
            <h5>메인 페이지</h5>
            <img src="./images/main_1.png" alt="main_1" width="100%" />  
        </td>
        <td align="center" width="200">
            <h5>시간대별 분석</h5>
            <img src="./images/main_1_recommend.png" alt="시간대별 분석" width="100%" />  
        </td> 
        <td align="center" width="200">
            <h5>메인 페이지 하단</h5>
            <img src="./images/main_2.png" alt="메인하단" width="100%" />
        </td>
        <td align="center" width="200">
            <h5>하단 비회원 분석</h5>
            <img src="./images/main_2_recommend1.png" alt="비회원 분석" width="100%" />
        </td>
        <td align="center" width="200">
            <h5>하단 회원 분석</h5>
            <img src="./images/main_2_recommend2.png" alt="회원 분석" width="100%" />
        </td>
    </tr>
    <tr>
      <td align="center">
        <div>✔ 시간대별 추천 상품 화면에 표시</div>
      </td>
      <td align="center">
        <div>✔ 비회원은 시간대별 분석</div>
        <div>✔ 회원은 시간대별 + 사용자 구매이력(SVD) + 아이템 카테고리 결합 분석</div>
      </td>
      <td align="center">
        <div>✔ 구매 빈도와 수량으로 가중치를 계산하여 화면에 표시</div>
      </td>
      <td align="center">
        <div>✔ 전체회원을 대상으로 가중치 점수가 높은 상품 분석</div>
      </td>
      <td align="center">
        <div>✔ 로그인한 회원 대상으로 비슷한 성별, 나이대 회원의 유사도 분석</div>
      </td>
    </tr>
</table>

### 2. 상세 페이지

<table>
    <tr>
        <td align="center" width="200">
            <h5>상세 페이지 화면</h5>
            <img src="./images/view.png" alt="상세 페이지" width="200" />  
        </td>
        <td align="center" width="200">
            <h5>상세 페이지 분석 및 시각화</h5>
            <img src="./images/view_recommend.png" alt="상세 페이지 분석" width="200" />  
        </td>
    </tr>
    <tr>
      <td align="center">
        <div>✔ 현재 페이지의 제품과 유사한 상품 화면에 표시</div>
      </td>
      <td align="center">
        <div>✔ 현재 페이지 상품과 유사한 제품을 분석 및 Heatmap으로 시각화</div>
      </td>
    </tr>
</table>

### 3. 장바구니

<table>
    <tr>
        <td align="center" width="200">
            <h5>장바구니 화면</h5>
            <img src="./images/cart.png" alt="" width="200" />  
        </td>
        <td align="center" width="200">
            <h5>장바구니 분석</h5>
            <img src="./images/cart_recommend.png" alt="" width="200" />  
        </td>
    </tr>
    <tr>
      <td align="center">
        <div>✔ 장바구니 담은 상품 비동기 통신(AJAX)을 통한수량 및 가격 변경</div>
      </td>
      <td align="center">
        <div>✔ 장바구니에 담은 상품과 유사한 상품을 분석 및 시각화</div>
      </td>
    </tr>
</table>

### 4. 구매내역

<table>
    <tr>
        <td align="center" width="200">
            <h5>구매내역 화면</h5>
            <img src="./images/purchase.png" alt="" width="200" />  
        </td>
        <td align="center" width="200">
            <h5>구매내역 분석</h5>
            <img src="./images/purchase_recommend.png" alt="" width="200" />  
        </td>
    </tr>
    <tr>
      <td align="center">
        <div>✔ 구매내역을 전체, 1개월, 3개월 필터화</div>
      </td>
      <td align="center">
        <div>✔ 구매한 상품과 유사한 상품을 분석 및 시각화</div>
      </td>
    </tr>
</table>

<div align="right"><a href="#tableContents">목차로 이동</a></div>

<br/>

### ✔ 프로젝트 결과물

---

<!-- - [포팅메뉴얼] -->
<!-- - [발표자료] -->
- [중간발표자료](./ppt/중간발표_eLMS.pdf)
- [최종발표자료](./ppt/최종발표_eLMS.pdf)


<!------- 팀원 소개 시작 -------->

## 👥 팀원 소개

<a name="developers"></a>
<table>
    <tr>
        <td align="center" width="200">
            <h5>Name</h5>
        </td>
        <td align="center" width="200">
            <h5>박윤희</h5>
        </td>
        <td align="center" width="200">
            <h5>박세연</h5>
        </td>
        <td align="center" width="200">
            <h5>박정희</h5>
        </td>
        <td align="center" width="200">
            <h5>백세원</h5>
        </td>
        <td align="center" width="200">
            <h5>진선용</h5>
        </td>
        <td align="center" width="200">
            <h5>정정원</h5>
        </td>
    </tr>
    <tr>
        <td align="center" width="200">
            <h5>역할</h5>
        </td>
        <td align="center" width="200">
            <h5>풀스택</h5>
        </td>
        <td align="center" width="200">
            <h5>프론트엔드</h5>
        </td>
        <td align="center" width="200">
            <h5>프론트엔드</h5>
        </td>
        <td align="center" width="200">
            <h5>풀스택</h5>
        </td>
        <td align="center" width="200">
            <h5>풀스택</h5>
        </td>
        <td align="center" width="200">
            <h5>프론트엔드</h5>
        </td>
    </tr>
</table>

<div align="right"><a href="#tableContents">목차로 이동</a></div>
