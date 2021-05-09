

# 알쓸코잡

  

Manifest 란 무엇일까?

## 목차

* [사전적 의미](#사전적-의미)

* [프론트에서 의미](#프론트에서-의미)

* [어떤것이 가능한가](#어떤것이-가능한가)

* [어디서 사용하는가](#어디서-사용하는가)

* [Manifest Version 2 VS Version 3](#manifest-version-2-vs-version-3)

  

## 사전적 의미
> [목차](#목차)
  
  React 와 같은 프론트 라이브러리나 Vue와 같은 프레임워크를 사용해본적이 있다면 한번쯤 manifest 파일을 본적이 있을것이라 생각합니다.

사실상 웹페이지 개발하는데 수정이 불필요한 피일이기 때문에 관심을 가지지 않는 사람들이 많을것이라고 생각해요.

과연 이 파일이 무엇이며, 어떤 역할을 하는 것일까요?

일단 Manifest 단어 자체의 사전적 의미부터 알아볼까요?
> **매니페스트 파일**(manifest file)은  [컴퓨팅](https://ko.wikipedia.org/wiki/%EC%BB%B4%ED%93%A8%ED%8C%85 "컴퓨팅")에서 집합의 일부 또는 논리정연한 단위인 파일들의 그룹을 위한  [메타데이터](https://ko.wikipedia.org/wiki/%EB%A9%94%ED%83%80%EB%8D%B0%EC%9D%B4%ED%84%B0 "메타데이터")를 포함하는 파일이다. 예를 들어, 컴퓨터 프로그램의 파일들은 이름, 버전 번호, 라이선스, 프로그램의 구성 파일들을 가질 수 있다.
>
> 이 용어는  [화물 목록](https://ko.wikipedia.org/w/index.php?title=%ED%99%94%EB%AC%BC_%EB%AA%A9%EB%A1%9D&action=edit&redlink=1 "화물 목록 (없는 문서)")(ship manifest)이 선원 및 화물을 나열하는 화물 수송 절차로부터 가져온 것이다.
< **[위키백과 참고](https://ko.wikipedia.org/wiki/%EB%A7%A4%EB%8B%88%ED%8E%98%EC%8A%A4%ED%8A%B8_%ED%8C%8C%EC%9D%BC)** >

위 내용에서 알 수 있듯이 Manifest 파일은 컴퓨팅에서 파일들의 그룹을 위한 메타데이터를 포함하는 파일을 의미합니다.

## 프론트에서 의미
> [목차](#목차)

그러면 위 내용대로라면, 프론트에서 Manifest파일은 프론트개발에 사용되어지는 파일들의 그룹을 위한 메타데이터를 포함하는 파일이 되겠죠?

이렇게 설명해서는 이해가 안될것 같아서 기본적인 Mainifest 파일의 내용물을 가져와 봤습니다.

```json
{  
	"short_name": "React App",  
	"name": "Create React App Sample",  
	"icons": [    
		{      
			"src": "favicon.ico",      
			"sizes": "64x64 32x32 24x24 16x16",      
			"type": "image/x-icon"    
		},    
		{   
			"src": "logo192.png",      
			"type": "image/png",      
			"sizes": "192x192"    
		},    
		{      
			"src": "logo512.png",      
			"type": "image/png",     
			"sizes": "512x512"    
		}  
	],  
	"start_url": ".",  
	"display": "standalone",  
	"theme_color": "#000000",  
	"background_color": "#ffffff"
}
```
파일속 내용을 살펴보면, 해당 manifest 파일이 관리하는 서비스의 풀네임과 간략형 이름부터 각 상황에 필요한 다양한 사이즈의 아이콘 정보까지 담겨져 있는것을 볼 수 있습니다. 

이렇듯 우리가 만드는 서비스에서 사용되는 기타 정보들에 대한 내용들이 담겨져 있습니다.

## 어떤것이 가능한가
> [목차](#목차)
  
해당 매니페스트 및 관련된 기술을 잘 활용한다면 기존의 웹사이트가 하지 못했던 영역가지 다양한 일을 하는 웹서비스를 만들 수 있습니다.

우리가 살펴보고 있는 매니페스트는 **"웹앱 매니페스트"** 라고 불립니다.  앱스토어를 거치지 않고 장치의 홈 화면에 설치할 수 있는 웹사이트를 구성이 가능하며 이는 단순한 홈 화면 링크/북마크를 통한 일반적인 웹 앱과 달른 방식으로 동작합니다. 이러한 역할수행을 돕는 매니페스트

## 어디서 사용하는가
> [목차](#목차)
  

## Manifest Version 2 VS Version 3
> [목차](#목차)
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTYwNjE3NTcxOSw3MDk4NjE1NjksNTU2MT
Y2NjI3LC0xNjczOTA4NDkyXX0=
-->