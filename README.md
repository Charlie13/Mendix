# Mendix
Mendix Intro Session

일정: 2019.11.27~28 10:00 ~ 17:00
장소: Siemens Office 12F

Agenda

1. Mendix 소개

2. Mendix Account @ mendix.com
   - Mendix Pro Install
   - Mendix Pro 소개

3. Sample Package
   - https://www.dropbox.com/s/w2ohqiisuebr0yg/MxManual_20191127.mpk?dl=0

4. Register Link
   - https://mxmanual20190913-sandbox.mxapps.io/index.html?profile=Responsive

#####
##

https://github.com/Charlie13/Mendix

https://gettingstarted.mendixcloud.com/link/path

Academy 
  -> Learning Path 
    -> Become a Rapid Developer (Developer)

#####
##
mendix.com 계정 생성
Mendix Pro 설치
eclipse 설치
Mendix App Mobile

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
## iFrame

 Add Modulde 
  iframe
  domain model
  MF Create iframehelper 
  Page create
  
 Navigation
  Page 등록

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
## QA

  Project Template
  > 공유

  HTML 5 기반

#####
## Fce Recogninition with API Service
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
