# Mendix Mendix Intro Session

일정: 20200603 09:30 ~ 17:00
장소: Siemens 12층 2번 교육장

# Agenda

# 0. 인증시험
6월30일 까지 한시적으로 "Rapid Certification exam 400$"을 무상으로 제공합니다.

## Mendix 회원 가입 및 Studio Pro Download(8.10.1 최신 버전. 2020.06.01 현재)
		회원가입 : https://signup.mendix.com/link/signup/?ref=143166
		Studio download : https://appstore.home.mendix.com/link/modelers/

## Learning Path 수강 (12시간 또는 24시간 강의 선택)
		https://gettingstarted.mendixcloud.com/link/path
		“Crash Course” 12 hours online course available here
		또는 “Become a Rapid Developer (Developer)” 24 hours online course available for free here

인증시험 신청 (다음의 코들 사용)
URL: https://gettingstarted.mendixcloud.com/link/module/97/lecture/818/11.1-The-Rapid-Developer-Certification-Exam
		Rapid Developer certificate here (50문항)
		use the voucher code "LEVELUP2020"


# Mendix 교육 Agenda

## 9:30 ~ 10:00	Opening & Mendix 소개
- Mendix Portal 가입 및 설치
- 아키텍처
- 기능 및 사례

## 10:00 ~ 10:30	SDS 솔루션 소개 및 협의
- Brity Works 등

## 10:40 ~ 12:00	Mendix 기본 기능 교육
- Sample App 개발 실습
- 솔루션 기능 소개 및 실습 (REST API I/F 등)

## 12:00 ~ 13:00	중식

## 13:00 ~ 16:40	Mendix 활용 App 개발 워크샵
- 생산라인 제품 불량 집계 App 개발
- DB, UI, 로직 구현 등
- 대시보드 개발
		
## 16:40 ~ 17:00	Wrap up
- 솔루션 구현 및 협업 Open discussion

# 1. Mendix 소개

# 2. 참조 Link:
    a. Mendix Studio Free Link
      i. 회원가입 : https://signup.mendix.com/link/signup/?ref=143166
      ii. Studio download : https://appstore.home.mendix.com/link/modelers/
    b. https://gettingstarted.mendixcloud.com/link/path

# 3. Contents
    a. Mendix Intro
    b. Mendix Sample Application Development
    c. Mobile Application Deployment
    d. Data Model & Application
      i. Micro Flow
      ii. Rest API
    e. Integration Demo
      i. Team Center
      ii. MindSphere
      iii. RAPIDAUTHOR
   
# 4. Domain Model & Microflow
    a. https://docs.mendix.com/howto/data-models/denormalize-data-to-improve-performance

# 5. 공장라인 제품 불량관리

# 6. Database Connector - DB 연계 Test
    a. 이 기종 DBMS 통합

# 7. Demo
    a. IoT Demo
    b. 전자 카탈로그 Demo

# 참조:

https://github.com/Charlie13/Mendix
https://gettingstarted.mendixcloud.com/link/path

Academy 
  -> Learning Path 
    -> Become a Rapid Developer (Developer)

#####
## Java Action Set

https://docs.mendix.com/howto/logic-business-rules/extending-your-application-with-custom-java

Project
 -> Add Module
   -> add 
      Java Action set

 -> Domain Model
      Assets
       AssetName
       AssetId
       AssetLocation

 -> Overview Page
    -> Object Page
       -> MF Call
          -> Java Action Call
	  
 -> Java Edit
    F6 / Deploy for eclipse

    Edit in eclipse or editor
    C:\Users\xxxxxx\Documents\Mendix\MxManual_20191127-main\javasource\javaactionset\actions\ReverseAssetName.java

    	@java.lang.Override
	public java.lang.String executeAction() throws Exception
	{
		this.inputAssets = __inputAssets == null ? null : javaactionset.proxies.Assets.initialize(getContext(), __inputAssets);

		// BEGIN USER CODE
		// throw new com.mendix.systemwideinterfaces.MendixRuntimeException("Java action was not implemented");
		String assetsAssetName = this.inputAssets.getAssetName(this.getContext());
		return new StringBuilder(assetsAssetName).reverse().toString();
		// END USER CODE
	}

#####
## Image Edit

#####
## Customer Order with Database interoperation Microflow

Project
 -> Add Module
   -> MyFirstModule
   Domain Model
     Entity Add
       Customer
         
       Order

     Generate Overview Pages

    Project
     -> Navigation
        Menu edit
        Customer
          customer
          order

     Console
       -> Advanced
          -> start build-in database browser

       SELECT a.* , b.*
         FROM "PUBLIC"."myfirstmodule$customer" a
           ,  "PUBLIC"."myfirstmodule$order" b

#####
## iFrame

 Add Modulde 
  iframe
  domain model
  MF Create iframehelper 
  Page create
  
 Navigation
  Page 등록

#####
## Rest API

  https://docs.mendix.com/howto/integration/consume-a-rest-service
  https://en.wikipedia.org/api/rest_v1/page/summary/{1}

#####
## Excel Importer

  https://docs.mendix.com/howto/integration/using-the-excel-exporter

#####
## Model Share

  https://modelshare.mendix.com/models/514edca3-4cb4-491c-ae49-653dc3453a28/test-execute-statement-postgre-sql

#####
## Face Recogninition with API Service
  https://facequote.zurich.co.uk/#/Upload_selfie

#####
## Data with List to widget
참조: Tree View Module

#####
## Debug
https://docs.mendix.com/howto/logic-business-rules/create-your-first-microflow-hello-world#1-introduction

- MicroFlow 정의
- Add Breakpoint
- 실행 후, 
- Run -> Debug -> Connect Debuger

- Console 영역의 Debug Window 참조

#####
## Barcode Scan & Google vision
참조 Link
https://www.dropbox.com/sh/s588rnbvwyx32p9/AABFj6I8gQfLIlPgL4rHKspia?dl=0

#####
## Siemens Plant Simulation Sample

https://www.dropbox.com/s/l92vfp8tzhh69jb/Siemens_Plant_Maintenance_Inspections_KC.mpk?dl=0

#####
## Microflow and menu

https://docs.mendix.com/howto/logic-business-rules/create-your-first-microflow-hello-world#1-introduction

- MicroFlow 정의
- Add Breakpoint
- 실행 후, 
- Run -> Debug -> Connect Debuger

- Console 영역의 Debug Window 참조

#####
## Tab Widget

STS Demo 
XPATH Expression


#####
## Rapid Advaanced Developer

email - REG Expression
After Commit - Microflow

#####
## items
