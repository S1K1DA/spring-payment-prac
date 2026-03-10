### 과제 1: "1000원 해커를 막아라!" (상품 가격 위변조 방어)

- **[과제 목표]**
    1. `Product` 엔티티와 `ProductRepository`를 간단하게 만드세요. (DB에 '스프링 부트 강의', 가격 '10,000원' 데이터가 있다고 가정)
    2. `PaymentFacade`의 `preparePayment` 메서드를 수정하여, 하드코딩된 100원이 아니라 **실제 DB에 있는 상품 가격을 조회해서 총 결제 금액(`calculatedAmount`)을 산출**하도록 변경하세요.
    3. 프론트엔드(`index.html`)에서 임의로 결제 요청 금액을 1000원으로 조작해서 결제를 시도해 보고, 백엔드의 **교차 검증 로직(`verifyAndApprove`)에서 에러가 터지며 결제가 방어되는 것**을 캡처해서 제출하세요.

 <img width="1717" height="1478" alt="image" src="https://github.com/user-attachments/assets/a4c51a1a-1dc6-47bd-8b46-ee1aa0aaab47" />
2천원 짜리 물품을 1천원으로 프론트에서 수정 후 결제

<img width="2557" height="1424" alt="image" src="https://github.com/user-attachments/assets/383cb744-204c-48ff-8adb-c2e255cda5ad" />
