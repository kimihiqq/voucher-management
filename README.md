**바우처 관리 애플리케이션**

- [x]  프로그램이 시작하면 다음과 같이 지원가능한 명령어를 알려줍니다.

<img width="1000" alt="image" src="https://github.com/kimihiqq/voucher-management/assets/134909318/86cee335-8493-4064-890f-ca6248029760">
<img width="1000" alt="image2" src="https://github.com/kimihiqq/voucher-management/assets/134909318/ce78c791-510d-4f5b-b8e7-b65c287c3944">

- [x]  create / list 커맨드를 지원합니다.
    - create 커맨드를 통해 바우처를 생성할수 있습니다다. (FixedAmountVoucher, PercentDiscountVoucher)
    - list 커맨드를 통해 만들어진 바우처를 조회할 수 있습니다.
- [x]  적절한 로그를 기록하고 `logback` 설정을해서 에러는 파일로 기록됩니다.
- [x]  Hamcrest 의 메쳐들 바탕으로 단위테스트를 작성했습니다.
- [x]  바우처 정보를 DB로 관리로 관리합니다.
    - 바우처 레포지토리는 JdbcTemplate을 사용해서 구현하였습니다.
- [x]  **바우처 지갑을 추가하였습니다.**
    - 특정 고객에게 바우처를 할당할 수 있습니다.
    - 고객이 어떤 바우처를 보유하고 있는지 조회할 수 있습니다.
    - 고객이 보유한 바우처를 제거할 수 있습니다.
    - 특정 바우처를 보유한 고객을 조회할 수 있습니다.
- [x]  커맨드로 지원했던 기능을 thymeleaf를 이용해 관리페이지를 만들고 다음 기능들을 지원하고 있습니다.
    - 조회페이지
    - 상세페이지
    - 입력페이지
    - 삭제기능

<img width="1000" alt="image3" src="https://github.com/kimihiqq/voucher-management/assets/134909318/444dc83e-b3c4-471e-9917-0e9c563bbbae">
<img width="1000" alt="image4" src="https://github.com/kimihiqq/voucher-management/assets/134909318/c92a609a-ea50-428e-b0cd-519146f320c5">
<img width="1000" alt="image5" src="https://github.com/kimihiqq/voucher-management/assets/134909318/076939ea-039f-41cd-aaae-d7c9364f1307">
<img width="1000" alt="image6" src="https://github.com/kimihiqq/voucher-management/assets/134909318/fa5a9dcc-6540-4d3a-811c-1c9827fa9251">

- [x]  Spring MVC를 적용해서 다음 기능을 제공하는 REST API를 추가하였습니다.
    - 조건별 조회기능 (바우처 생성기간 및 특정 할인타입별)
    - 바우처 추가기능
    - 바우처 삭제기능
    - 바우처 아이디로 조회 기능
