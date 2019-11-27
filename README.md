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

4. Java Action Set
   - https://docs.mendix.com/howto/logic-business-rules/extending-your-application-with-custom-java

#####
##

https://github.com/Charlie13/Mendix

https://gettingstarted.mendixcloud.com/link/path
Academy 
  -> Learning Path 
    -> Become a Rapid Developer (Developer)
 
#####
##
https://mxmanual20190913-sandbox.mxapps.io/index.html?profile=Responsive

#####
##
mendix.com 계정 생성

#####
##
Mendix Pro 설치

#####
##
eclipse 설치

#####
##

#####
##
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

    > C:\Users\vdmb5t\Documents\Mendix\MxManual_20191127-main\javasource\javaactionset\actions
      ReverseAssetName.java

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

