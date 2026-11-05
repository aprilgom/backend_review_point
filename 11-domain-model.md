# 도메인 모델·값 표현

[전체 목차](README.md) · [FC 번호별 목차](FC_INDEX.md) · [← 이전: 문서·개발·학습 과정](10-workflow.md) · [다음: 도메인 검증 →](12-validation.md)

**관련 분야:** [엔티티 동등성·식별](06-identity.md) · [도메인 검증](12-validation.md) · [책임·계층 경계](19-responsibility.md)

## 이 분야의 FC

- [FC0203 · ID만 받고 나머지 필드를 null로 두는 `Member` 생성자가 왜 필요한지 질문하며 어색하다는 의견을 제시했다.](fc/FC0203.md)

- [FC0205 · 복잡한 비즈니스 로직에서 객체 상태 변화로 코드가 복잡해지는 점을 고려하여 도메인 객체를 가능한 한 불변 객체로 만들어 보자는 제안이다.](fc/FC0205.md)

- [FC0206 · 도메인과 엔티티를 어떻게 정의하며, Cart에 별도 조건이나 로직이 없다는 이유로 도메인 모델을 두지 않는 판단이 적절한지 논의했다.](fc/FC0206.md)

- [FC0207 · 문자열로 지정하는 ContentType을 HttpStatusCode처럼 enum으로 관리하자고 제안했다.](fc/FC0207.md)

- [FC0204 · 주문 테이블에 updated_at이 필요한지 확인하고, 수정 가능한 데이터와 수정하지 않는 이력 데이터를 구분해 판단하도록 논의했다.](fc/FC0204.md)

- [FC0209 · 날짜 정보를 문자열로 취급하는 대신 LocalDate로 표현하는 방식을 제안했다.](fc/FC0209.md)

- [FC0208 · 상품 가격을 int로 표현하는 대신 BigDecimal 사용을 고려하자고 제안했다.](fc/FC0208.md)

- [FC0211 · Reservation과 ReservationWaiting이 거의 동일한 도메인인 현재 구조에서, 대기를 예약의 상태로 표현하지 않은 이유를 물었다.](fc/FC0211.md)

- [FC0212 · Reservation이 status로 예약과 예약 대기를 표현하는 것을 어색하게 느낀 이유를 묻고, 취소 예약까지 고려해 모델 분리 기준을 검토하도록 제안한다.](fc/FC0212.md)

- [FC0210 · Line의 이름과 색상을 변경하는 setter 사용을 지양하는 것이 어떨지 제안했다.](fc/FC0210.md)

- [FC0213 · HTTP의 method, uri, version은 헤더가 아닌 Request Line에 속하므로 HttpRequestHeader와 다른 객체에서 표현하는 방안을 제안했다.](fc/FC0213.md)

- [FC0214 · 타입에 따라 사용하지 않는 값이 생기는 쿠폰 테이블에서, 기본값과 NOT NULL 제약이 값의 부재 가능성을 가려 혼선을 줄 수 있다는 우려다.](fc/FC0214.md)


---

[전체 목차](README.md) · [FC 번호별 목차](FC_INDEX.md) · [← 이전: 문서·개발·학습 과정](10-workflow.md) · [다음: 도메인 검증 →](12-validation.md)
