# 책임·계층 경계

[전체 목차](README.md) · [FC 번호별 목차](FC_INDEX.md) · [← 이전: 렌더링·데이터 로딩](18-rendering.md) · [다음: 인증·보안·비밀값 →](20-security.md)

**관련 분야:** [추상화·중복](01-abstraction.md) · [의존성·교체 가능성](09-dependency.md) · [도메인 모델·값 표현](11-domain-model.md)

## 이 분야의 FC

- [FC0360 · 컨트롤러를 한 번 생성해 재사용하려는 목적이라면 LoginController 자체를 싱글톤으로 구현하는 방안을 논의했다.](fc/FC0360.md)

- [FC0363 · 컨트롤러에서 도메인과 DTO를 변환하는 대신 서비스가 요청 DTO를 받고 응답 DTO를 반환하는 구조를 검토한다.](fc/FC0363.md)

- [FC0356 · 컨트롤러 메서드를 가져오는 단계에서 RequestMapping 어노테이션으로 필터링하지 않고 모든 메서드를 가져온 이유를 질문했다.](fc/FC0356.md)

- [FC0359 · HttpResponse가 응답 값을 표현하는 것 외에 요청에 맞는 Controller를 찾고 실행하는 책임까지 가져야 하는지 검토한다.](fc/FC0359.md)

- [FC0364 · 요청 메서드 값을 외부에서 직접 비교하기보다 RequestMethod 객체에 isGet() 메시지를 보내 판단하도록 제안했다.](fc/FC0364.md)

- [FC0367 · HttpRequest가 요청 파싱, 로직 처리, 응답 생성까지 담당하므로 책임을 분리하는 것이 좋겠다는 의견을 제시한다.](fc/FC0367.md)

- [FC0362 · 도메인 객체가 응답 역할까지 과도하게 담당하는지 검토하고 응답 객체 분리를 고려하자.](fc/FC0362.md)

- [FC0369 · 서비스가 예약의 날짜와 시간을 꺼내 과거 예약인지 계산하기보다 Reservation 객체에 판단을 요청하자는 제안이다.](fc/FC0369.md)

- [FC0365 · 도메인 패키지에 여러 개념이 섞이지 않도록 필요해지면 domain.line 같은 개념별 하위 패키지로 분리하자고 제안했다.](fc/FC0365.md)

- [FC0374 · Request DTO를 Controller 패키지가 아니라 Service 패키지에 둔 이유와 계층별 DTO 분리 방식을 논의했다.](fc/FC0374.md)

- [FC0361 · LineStationController가 너무 많은 로직을 책임지고 있으므로 비즈니스 로직을 서비스에서 처리하도록 제안했다.](fc/FC0361.md)

- [FC0375 · 도메인 객체가 DAO에 직접 접근해야 하는 이유를 검토하고, 도메인은 판단 결과를 반환하며 서비스가 DAO를 통해 저장하는 역할 분담을 고려하자.](fc/FC0375.md)

- [FC0378 · PathService에서 역을 조회할 때 LineService를 경유하기보다 해당 역할을 맡은 StationService를 활용하자는 제안이다.](fc/FC0378.md)

- [FC0370 · Service 계층의 역할을 정리하고, 현재 구현에서 계층 분리가 필요한지와 미리 분리하는 방식의 장단점을 검토하도록 요청했다.](fc/FC0370.md)

- [FC0366 · RequestMapping 클래스를 controller 패키지에 배치한 특별한 이유가 있는지 질문했다.](fc/FC0366.md)

- [FC0357 · 요청에서 User를 추출하는 행위와 User를 저장하는 행위를 분리하자고 제안했다.](fc/FC0357.md)

- [FC0382 · 컨트롤러가 단일 책임을 지키도록 예외 처리를 분리하고 ControllerAdvice 계열의 활용을 검토하도록 제안한다.](fc/FC0382.md)

- [FC0377 · HandlerMapping과 HandlerAdapter 각각의 역할과, 두 역할을 하나로 합치지 않고 분리한 이유를 설명해 달라고 요청했다.](fc/FC0377.md)

- [FC0380 · 서비스 등에 남아 있는 로직을 도메인 객체에 더 위임할 수 있는지 검토하자는 제안이다.](fc/FC0380.md)

- [FC0358 · cart 문자열만 조회하는 대신 Member를 조회해 MemberEntity로 변환하고, 관련 변환 로직을 MemberEntity에 둘 수도 있다고 제안했다.](fc/FC0358.md)

- [FC0373 · 복잡한 조회 로직 때문에 fakeRepository 구현이 어렵다면 Repository의 책임이 많은지 살펴보고 관련 로직을 Service로 옮기는 방안을 제안했다.](fc/FC0373.md)

- [FC0383 · DispatcherServlet과 DispatcherServletInitializer를 app 패키지에 둔 이유를 묻고 mvc 패키지로의 이동을 검토하자고 제안했다.](fc/FC0383.md)

- [FC0379 · 서비스가 컨트롤러와 소통할 때 도메인 객체를 그대로 노출하면 어떤 문제가 생길 수 있는지 질문했다.](fc/FC0379.md)

- [FC0384 · DAO에 @Repository를 사용한 이유를 묻고 DAO와 Repository의 역할 차이를 논의했다.](fc/FC0384.md)

- [FC0385 · 트랜잭션 사용 여부에 따른 커넥션 상태 확인과 처리를 JdbcTemplate이 아닌 DataSourceUtils에 둔 이유를 묻는다.](fc/FC0385.md)

- [FC0386 · OrderService의 사용 중이지 않은 테이블에 대한 주문 검증을 Order 생성 시 도메인에서 수행하도록 옮길 것을 제안했다.](fc/FC0386.md)

- [FC0372 · Adapter에서 ModelAndView를 얻은 뒤 렌더링은 별도로 수행하는 구조를 확인했다.](fc/FC0372.md)

- [FC0368 · 발급을 돕는 CouponIssuer가 쿠폰 한 건에 종속되는 현재 구조 대신, 미리 생성한 발급기를 활용할 수 있는 협력 관계를 고민하도록 제안했다.](fc/FC0368.md)

- [FC0376 · 화면 안내 문구를 action으로 내려주면 UI 문구 변경 때 백엔드와 API 계약도 함께 변경해야 하는 결합이 생길 수 있다.](fc/FC0376.md)

- [FC0381 · 조회 결과를 리스트로 반환하는 로직과 executeUpdate 실행 로직이 한 메서드에 있으므로 두 역할을 분리하는 방안을 제안했다.](fc/FC0381.md)

- [FC0371 · 서비스 코드에 데이터 액세스 관련 코드가 남아 있으므로 컴포넌트의 위치와 책임을 고려해 분리하도록 제안했다.](fc/FC0371.md)


---

[전체 목차](README.md) · [FC 번호별 목차](FC_INDEX.md) · [← 이전: 렌더링·데이터 로딩](18-rendering.md) · [다음: 인증·보안·비밀값 →](20-security.md)
