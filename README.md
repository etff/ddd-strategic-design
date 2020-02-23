# 키친포스

## 요구 사항

### 상품

* 상품을 등록할 수 있다.
* 상품의 가격이 올바르지 않으면 등록할 수 없다.
    * 상품의 가격은 0 원 이상이어야 한다.
* 상품의 목록을 조회할 수 있다.

### 메뉴 그룹

* 메뉴 그룹을 등록할 수 있다.
* 메뉴 그룹의 목록을 조회할 수 있다.

### 메뉴

* 1 개 이상의 등록된 상품으로 메뉴를 등록할 수 있다.
* 메뉴의 가격이 올바르지 않으면 등록할 수 없다.
    * 메뉴의 가격은 0 원 이상이어야 한다.
    * 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
* 메뉴는 특정 메뉴 그룹에 속해야 한다.
* 메뉴의 목록을 조회할 수 있다.

### 테이블

* 테이블을 등록할 수 있다.
* 테이블의 목록을 조회할 수 있다.
* 빈 테이블 설정 또는 해지할 수 있다.
* 단체 지정된 테이블은 빈 테이블 설정 또는 해지할 수 없다.
* 주문 상태가 조리 또는 식사인 테이블은 빈 테이블 설정 또는 해지할 수 없다.
* 방문한 손님 수를 입력할 수 있다.
* 방문한 손님 수가 올바르지 않으면 입력할 수 없다.
    * 방문한 손님 수는 0 명 이상이어야 한다.
* 빈 테이블은 방문한 손님 수를 입력할 수 없다.

### 단체 지정

* 2 개 이상의 빈 테이블을 단체로 지정할 수 있다.
* 단체 지정은 중복될 수 없다.
* 단체 지정을 해지할 수 있다.
* 단체 지정된 테이블의 주문 상태가 조리 또는 식사인 경우 단체 지정을 해지할 수 없다.

### 주문

* 1 개 이상의 등록된 메뉴로 주문을 등록할 수 있다.
* 빈 테이블에는 주문을 등록할 수 없다.
* 주문의 목록을 조회할 수 있다.
* 주문 상태를 변경할 수 있다.
* 주문 상태가 계산 완료인 경우 변경할 수 없다.

## 용어 사전

| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 포스 | POS | 상품의 판매 관리. 재고, 손님, 판매정보를 관리하여 판매를 돕는 시스템. |
| 상품 | Product | 판매되는 음식을 뜻한다. |
| 메뉴 상품 | Menu Product | 메뉴에 담기는 상품과 갯수를 뜻한다. |
| 메뉴 | Menu | 메뉴이름과 상품의 가격과 수량이 포함되어 주문이 만들어진다. |
| 메뉴 그룹 | Menu Group | 메뉴의 상위 카테고리를 뜻한다. |
| 손님 | Guest | 상품을 주문하고, 식사를 하는 사람 |
| 테이블 | Table | 손님이 주문을 한 뒤, 식사를 하게되는 곳 |
| 빈 테이블 | Empty Table | 손님이 이용중이지 않은 테이블을 뜻한다. |
| 단체석 | Table Group | 2개 이상의 테이블을 묶어서 손님에게 제공한다. |
| 주문 | Order | 손님이 식사를 하기위해 테이블에서 메뉴를 지정하는것을 뜻한다. |
| 주문상태 | Order Status | 주문이 실행되면 실행되는 단계 (조리, 식사중, 완료) |
| 조리 | Cooking | 주문이 접수되어 상품이 만들어지는 단계 |
| 식사중 | Meal | 상품이 테이블의 손님에게 전달된 단계 |
| 완료 | Completion | 손님이 계산을 끝낸 단계 |




## 모델링
