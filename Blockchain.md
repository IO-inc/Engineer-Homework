
# 블록체인(Blockchain) 분석

- 비트코인(Bitcoin)이라는 가상화폐는 거래 내역을 블록체인이라는 형태로 저장합니다. 블록체인에서 각 블록의 데이터를 확인하기 위한 기능이 필요합니다. 
>+ [비트코인 wikipedia](https://ko.wikipedia.org/wiki/%EB%B9%84%ED%8A%B8%EC%BD%94%EC%9D%B8#.EB.B8.94.EB.A1.9D.EC.B2.B4.EC.9D.B8)
>+ [블록체인 wikipedia](https://ko.wikipedia.org/wiki/%EB%B8%94%EB%A1%9D%EC%B2%B4%EC%9D%B8)
  
## 블록에 포함된 내용

- 해당 블록의 해쉬 값
- 이전 블록의 해쉬 값
- 트랜잭션(Transaction) 리스트
>+ 비트코인 거래내역 리스트
>+ inputs(해당 블록에 포함된 비트코인이 어디에서 왔는지)
>+ out(해당 블록에 포함된 비트코인이 어디로 전달되었는지)
  
## 요구사항

1. "블록 해쉬 값"을 Argument로 전달 받아서 아래의 정보를 출력
>+ 트랜잭션(tx) 수
>+ 평균 트랜잭션의 값(value)
>+ 평균 트랜잭션의 수수료(fee)
>+ 평균 트랜잭션의 크기(size)
  
2. "블록 해쉬 값과 input or output"을 Argument로 받아서, input 혹은 output의 정보만 출력
>+ 즉, **[블록 해쉬 값] input** 형태로 Argument를 전달하게 되면 트랜잭션 내용 중 inputs에 관한 내용만 출력

## 참고

1. 블록 확인 API (해당 API를 활용해서 개발해주세요)
>+ https://blockchain.info/block-index/{blockhash}?format=json
2. 블록 구조 확인
>+ https://blockchain.info

## 주의

- 모든 결과는 GitHub에서 확인합니다.
>+ 메일로 회신해 주신 GitHub 계정에, "IO-Homework"라는 Repository를 생성해서 작업해주세요.
>+ 로컬에서 작업을 완료하신 후 한 번에 commit하지 마시고, 단위 작업별로 commit을 수행해서 과정을 확인할 수 있도록 해주세요.
>+ 5/21(일) PM 10:30 까지 남겨진 commit 로그에 대해서만 리뷰를 진행하겠습니다.
>+ 코드에 대한 접근 방법, 설계 등을 README.md 파일에 정리해 주세요.
- 언어에 대한 제한은 없습니다. 익숙하신 언어로 개발해주세요.
- 불확실한 요구사항이 있다면 개인적으로 가정을 하셔도 좋습니다. 단, 가정에 대한 이유는 README.md 파일에 분명히 밝혀주세요.

## 평가기준

- 기능의 정확도
- TDD
- 테스트 코드
- 모듈화
- 가독성
- 문제 접근방식
- 정보 전달능력




