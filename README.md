# Schapi-Go

Schapi Go는 Schapi의 Go언어 버전으로  
Go언어 기반의 급식, 학사일정 파싱 라이브러리입니다.  

## 1. 설치  

schapi-go 는 GOPATH의 프로젝트에 다음과 같이 설치할 수 있습니다.  

```
go get github.com/DSM-SchoolAPI/schapi-go
```

## 2. 예제

다음은 대덕소프트웨어마이스터고등학교 (G100000170) 의 5월 23일자 점심  
식단표를 불러와 출력하는 예제입니다.

```
api := schapi.NewSchoolAPI(schapi.HighSchool, schapi.Daejeon, "G100000170")
fmt.Println(api.GetMonthlyMeals(2018, 5)[23].Lunch)
```

## 3. 음;

현재 작성된 Schapi-Go는 다른 언어의 Schapi와 구조도 다르고  
학사일정 파싱을 구현하지 못하는 등 구현에 있어 아쉬운 부분이 많습니다. 


그래서 추후 Schapi의 구조에 맞게 라이브러리 구조를 변경하고 학사일정  
파싱 기능을 추가하는 마이그레이션 작업을 진행하고 있습니다!


현재 API 구조를 기존 Schapi 와 비슷하게 변경하고
학사일정 기능 추가를 고려하고 있습니다 
