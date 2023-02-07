## Blockchain-based coupon system

>블록체인을 기반으로 하여 쿠폰 발급과 관리를 할 수 있는 시스템이다. 
해당 시스템을 사용하는 카페는 개별적으로 발급하여 사용하는 기존의 쿠폰 시스템에서 벗어나 통합적으로 쿠폰을 발급하여 사용할 수 있다. 
또한 해당 시스템을 이용하는 고객은 하나의 애플리케이션으로 다양한 카페에서 쿠폰 이용을 할 수 있다.

* 개발 배경   
    >기존의 개인 카페 각각에서 쿠폰을 발급하고 관리하는 것에 대한 어려움을 겪었다. 
따라서 쿠폰 발급과 사용 과정을 투명하게 공개 및 공유할 수 있는 시스템의 필요성을 느껴 블록체인을 활용한 통합 쿠폰 시스템을 개발하였다.

* 전체 구성   
    >해당 시스템 네트워크에 참여하는 주체는 Market(코인 발급소), CEO(카페 사장), Customer(고객)이다. 
모든 CEO와 Customer는 각각 코인 지갑을 보유하고 있다. 
코인 1개는 쿠폰 1장과 같으며 CEO가 Customer에게 쿠폰 1장을 지급할 때, CEO는 1코인이 차감되며, Customer는 1코인이 추가되면서 쿠폰 1장이 적립된다. 
해당 시스템이 가진 기능은 ‘CEO 코인 충전, Customer 쿠폰 적립, Customer 쿠폰 사용, Customer 카페리스트 확인’이다.
  * CEO 코인 충전: CEO가 Customer에게 쿠폰을 적립하기 위해 Market으로부터 코인을 충전한다.   
  * Customer 쿠폰 적립: Customer가 음료 한 잔을 구매 시 CEO로부터 쿠폰 1개를 발급받는다.
  * Customer 쿠폰 사용: Customer의 쿠폰이 10개가 되면 자동으로 쿠폰이 사용된다.
  * Customer 카페리스트 확인: Customer가 쿠폰 사용이 가능한 카페 리스트를 확인 가능하다.

* 구현 환경   
    >개발환경(IDE)는 Visual Studio Code, Ganache, Truffle 이다. 
개발 도구는 React, Bootstrap, Web3.js, MySQL, Metamask이며 개발 언어는 JS, Solidity 이다. 
블록체인 네트워크는 Ethereum이며 배포는 Git을 사용했다.

* 구현 결과   
    >Market과 CEO와 Customer의 거래 내역이 모두 퍼블릭 블록체인 네트워크 시스템에 기록이 된다. 
이러한 기록을 통해 CEO는 가장 많이 구매하는 음료 목록 등을 보고, 카페의 운영에 도움을 줄 수 있다. 
또한 해당 쿠폰 시스템을 통해 CEO는 개인 카페에서도 쿠폰 시스템을 적용해 매출 증가 가능성을 높일 수 있고, Customer는 개인 카페에서도 쿠폰 적립이 가능해진다.
