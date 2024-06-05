# 의류재고 떨이 & 리폼 플랫폼

## 프로젝트 소개

### 문제 정의
- 현대 사회에서는 패션 트렌드의 빠른 변화와 소비자들의 다양한 요구로 인해 의류 산업이 크게 성장하고 있다. 하지만 이러한 성장은 그림자를 동반하고 있다. 의류 폐기물이 급증함에 따라 점주들은 많은 손해를 입고 있으며, 환경 오염 문제도 심각해지고 있다.
- 의류 제작 및 폐기가 환경 오염에 끼치는 영향에 대해서 의류/섬유 산업의 순환 경제로의 전환을 위한 연구를 진행한 논문을 인용하면 의류의 환경 영향은 폐기 단계뿐만 아니라 생산 과정에서 도 온실가스 배출, 수질 오염 등을 비롯한 높은 환경 오염을 보이며, 티셔츠 한 벌 생산에 필요 한 물의 양은 2,700L, 청바지는 7,000L이다. 의류 산업에서 배출하는 탄소 배출량은 전체의 10% 에 해당하며, 염료와 표백제 사용으로 산업 수질 오염 비중은 20%, 1차 미세 플라스틱 오염 비 중은 35%인 것으로 조사되었다
- 특히 악성 재고나 시즌 오프 의류들이 적절히 처리되지 못하는 것이 주요 문제 중 하나이며, 이러한 문제는 단순히 판매자와 소비자 간의 경제적인 문제를 넘어서 환경적인 차원에서 우리 사회에 심각한 부담을 가하고 있다.
- 이러한 문제를 해결하기 위해 새로운 처리 방식과 기술이 절실하게 필요하다.
<div align="center">
   <img alt="img_2.png" height="300" src="https://github.com/GachonMoWA/.github/blob/main/profile/img_2.png" width="300"/>
   <img alt="img_3.png" height="300" src="https://github.com/GachonMoWA/.github/blob/main/profile/img_3.png" width="400"/>
</div>

### 프로젝트 목표
- 의류 폐기물로 인한 환경 오염을 줄이는 것과 점주들에게 경제적인 부담을 완화 하는 것이다. 의류 떨이 서비스를 통해 악성 재고를 처리하고, 상품을 재활용 및 개조하여 지속 가능한 소비와 생산을 촉진하며, 판매자, 디자이너, 구매자에게 상호 간의 혜택을 제공한다.
- 판매자는 재고 관리 및 악성 재고 처리에 용이해지고 플랫폼을 통한 디자이너와의 연결이 수월해진다.
- 구매자는 악성 재고를 저렴하게 구매할 수 있고, 플랫폼을 통해 구매와 리폼을 동시에 진행할 수 있다.
- 디자이너는 리폼 시장 활성화로 인한 수익 창출 기회가 확대되고 경험을 쌓을 수 있는 현장을 제공받는다.

## 주요 기능

### 구매자 - 디자이너 리폼 과정

1. 판매자가 상품을 등록한다.

![상품등록](https://github.com/jjsOrganization/server/assets/76249685/973129f8-fbb2-4416-9c98-5947452b8d60)

2. 판매자가 게시한 상품들 중 구매자가 리폼을 원하는 상품이 있다면 해당 상품 페이지에서 리폼 요청 및 디자이너 선택을 한다.

![리폼요청](https://github.com/jjsOrganization/server/assets/76249685/e8351509-10d4-496c-bc4a-430fe7a3727c)

3. 디자이너가 구매자에게 받은 요청서를 확인하고 리폼 진행 승인 여부를 결정한다.

![num3](https://github.com/jjsOrganization/server/assets/76249685/166f973e-ab5d-4993-95c7-796a8a37198a)

4. 디자이너가 구매자와 채팅으로 견적 상담을 진행하고, 견적 작성 후 견적서 제출을 한다. 

![견적서 등록](https://github.com/jjsOrganization/server/assets/76249685/534321bb-e1d0-498d-b00f-068162d2a3df)

5. 구매자가 디자이너가 작성한 견적서를 확인하고, 최종 승인 여부 결정 및  리폼 완료 시 진행되는 배송지 입력 등을 한다. 배송지 입력 완료 시, 디자이너는 리폼을 시작한다.

![num4](https://github.com/jjsOrganization/server/assets/76249685/9fa9d631-d559-4ecf-ab7d-bc9477981c1e)

6. 디자이너는 리폼을 진행하며 형상관리(진행 현황) 이미지를 등록 한다.
7. 구매자는 형상관리 이미지를 확인할 수 있으며, 형상관리 마지막 이미지 등록 확인 시 리폼 완료를 알 수 있다.

### 공통 기능

- 로그인 및 회원가입
  - 회원은 구매자, 판매자, 디자이너로 구분된다. 회원가입 시 각 회원 별 양식이 다르며, 회원 이메일은 중복을 허용하지 않는다.
  - 회원들은 모두 하나의 로그인 화면에서 로그인을 진행한다.
- 판매자
  - 판매자의 상품 등록, 수정, 삭제, 판매 내역 조회
- 구매자
  - 구매자는 장바구니 이용 가능(회원가입 시 하나의 장바구니 자동 생성)
  - 상품 좋아요 가능 (상품 인기순 조회에 반영)
  - 리폼 의뢰 가능(리폼 과정은 [구매자-디자이너 리폼 과정](#구매자---디자이너-리폼-과정) 참고)
  - 상품 구매 가능
- 디자이너
  - 포트폴리오 등록, 수정, 조회
  - 구매자의 리폼 의뢰에 대한 리폼 진행 (리폼 과정은 [구매자-디자이너 리폼 과정](#구매자---디자이너-리폼-과정) 참고)
  - 리폼 완료된 항목에 대한 작업물 등록. 자신의 포트폴리오로 사용하기 위함
- 모든 회원
  - 상품 전체 조회 및 상세 조회
  - 포트폴리오 전체 조회 및 상세 조회
  - 디자이너 작업물 전체 조회 및 상세 조회
  - 물 사용량 조회
  

## 기술 스택

OS | ![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white) ![macOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=macos&logoColor=F0F0F0)
--- | --- |
Frontend | ![HTML5](https://user-images.githubusercontent.com/97425158/161745161-566f015b-0ec2-4bba-82aa-f3bb7498bdd7.svg) ![CSS3](https://user-images.githubusercontent.com/97425158/161745198-92ff3896-7ce0-4946-a8b4-e6d23223eb3b.svg) ![Javascript](https://user-images.githubusercontent.com/97425158/161745127-a3fa5ed0-ceb6-427a-94d1-834d762fd3b4.svg) ![React](https://user-images.githubusercontent.com/97425158/161745107-cc062718-9c52-4446-8f14-9faba0b9dea7.svg) ![Axios](https://user-images.githubusercontent.com/97425158/161745239-453b4075-7bd0-4c63-9c5a-5c1d76021b8d.svg)
Backend | ![Java](https://img.shields.io/badge/JAVA-007396?style=for-the-badge&logo=java&logoColor=white) ![Gradle](https://img.shields.io/badge/gradle-02303A?style=for-the-badge&logo=gradle&logoColor=white) ![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=Hibernate&logoColor=white) ![Spring](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=Spring&logoColor=white) ![Springboot](https://img.shields.io/badge/Springboot-6DB33F?style=for-the-badge&logo=Springboot&logoColor=white) ![Sprint Security](https://img.shields.io/badge/springsecurity-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white) ![Spring Data JPA]()
Database | ![Mysql](https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white) ![Redis](https://img.shields.io/badge/redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
Server | ![AWS](https://img.shields.io/badge/aws-232F3E?style=for-the-badge&logo=AmazonAWS&logoColor=white) ![S3](https://img.shields.io/badge/AmazonS3-569A31?style=for-the-badge&logo=AmazonS3&logoColor=white) ![Ec2](https://img.shields.io/badge/Amazon%20EC2-FF9900?style=for-the-badge&logo=Amazon%20EC2&logoColor=white) ![Kafka](https://img.shields.io/badge/ApacheKafka-%3333333.svg?style=for-the-badge&logo=ApacheKafka&logoColor=white) ![Amazon RDS](https://img.shields.io/badge/Amazon_RDS-232F3E?style=for-the-badge&logo=amazon-rds&logoColor=white)
CI/CD | ![Github Action](https://img.shields.io/badge/GitHubActions-2088FF?style=for-the-badge&logo=GitHubActions&logoColor=white) ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white) ![Nginx](https://img.shields.io/badge/NGINX-009639?style=for-the-badge&logo=NGINX&logoColor=white)
Development Tools | ![VSCode](https://img.shields.io/badge/visualstudiocode-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white) ![IntelliJ IDEA](https://img.shields.io/badge/IntelliJIDEA-000000.svg?style=for-the-badge&logo=intellij-idea&logoColor=white)
Version Control | ![Git](https://img.shields.io/badge/git-F05032?style=for-the-badge&logo=git&logoColor=white) ![Github](https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white)
Communication |  ![Notion](https://img.shields.io/badge/Notion-%23000000.svg?style=for-the-badge&logo=notion&logoColor=white) ![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white) ![Figma](https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white) ![Swagger](https://img.shields.io/badge/-Swagger-%23Clojure?style=for-the-badge&logo=swagger&logoColor=white)


## 시스템 아키텍쳐
<p align="center"><img src="https://github.com/jjsOrganization/.github/blob/main/profile/resources/sw_architecture.jpg" width="90%"/></p>

## ERD 설계
<p align="center"><img src="https://github.com/jjsOrganization/.github/blob/main/profile/resources/jjsDb.png" width="90%"/></p>

## 기획 및 설계

[API 명세서](https://magenta-camp-6cd.notion.site/API-7e5c9ecd12004583a2ba8c368f4a177a?pvs=4)<br>
[전공종합설계(2) 최종 발표 자료](https://github.com/jjsOrganization/.github/blob/main/%EC%A0%84%EA%B3%B5%EC%A2%85%ED%95%A9%EC%84%A4%EA%B3%84(2)%20%EC%A0%9C%EC%B6%9C%EB%AC%BC/%E1%84%8C%E1%85%A5%E1%86%AB%E1%84%8C%E1%85%A9%E1%86%BC%E1%84%89%E1%85%A5%E1%86%AF-%E1%84%8E%E1%85%AC%E1%84%8C%E1%85%A9%E1%86%BC%E1%84%87%E1%85%A1%E1%86%AF%E1%84%91%E1%85%AD%E1%84%8C%E1%85%A1%E1%84%85%E1%85%AD.pdf)

## 팀 소개

|<img src="https://avatars.githubusercontent.com/u/156943610?v=4" width="150" height="150"/>|<img src="https://avatars.githubusercontent.com/u/133757454?v=4" width="150" height="150"/>|<img src="https://avatars.githubusercontent.com/u/122250088?v=4" width="150" height="150"/>|<img src="https://avatars.githubusercontent.com/u/76249685?v=4" width="150" height="150"/>|<img src="https://avatars.githubusercontent.com/u/87377014?v=4" width="150" height="150"/>|
|:-:|:-:|:-:|:-:|:-:|
|Frontend<br/>[이정필](https://github.com/jungpill)|Frontend<br/>[양준규](https://github.com/YJKBigBo)|Frontend<br/>[고한동](https://github.com/Undercrosshd)|Backend<br/>[김경호](https://github.com/sgn07124)|Backend<br/>[손혁](https://github.com/SonHyeok)|
