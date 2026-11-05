# 의존성·교체 가능성

[전체 목차](README.md) · [FC 번호별 목차](FC_INDEX.md) · [← 이전: 데이터 관계·영속성](08-persistence.md) · [다음: 문서·개발·학습 과정 →](10-workflow.md)

**관련 분야:** [추상화·중복](01-abstraction.md) · [책임·계층 경계](19-responsibility.md) · [테스트 준비·격리](22-test-isolation.md)

## 이 분야의 FC

- [FC0146 · 인터페이스를 분리한 뒤에도 알고리즘 변경 시 서비스 내부 구현을 수정해야 하는 의존 구조를 검토하고, OCP 관점에서 교체 가능한 구조를 고민하도록 제안한다.](fc/FC0146.md)

- [FC0149 · 컨트롤러 인스턴스를 매번 새로 생성해야 하는지 검토하고, 싱글턴으로 재사용하는 방식을 고려해볼 것을 제안했다.](fc/FC0149.md)

- [FC0155 · DispatcherServlet에서 특정 매핑 구현체를 직접 생성하는 대신 HandlerMapping 구현체를 리플렉션으로 찾는 방식을 고려해 보자는 의견이다.](fc/FC0155.md)

- [FC0151 · JPA 리포지터리를 직접 사용하지 않고 구현체에 주입해서 사용하는 이유를 물었다.](fc/FC0151.md)

- [FC0153 · 외부에서 의존성을 주입받는 구조가 되었으므로 일부 클래스를 제외하면 mvc로 옮겨도 mvc가 app을 의존하지 않을 것으로 보인다고 확인했다.](fc/FC0153.md)

- [FC0150 · 컨트롤러의 실제 인스턴스를 만들지 않고 클래스 타입만 보관하도록 구현한 이유를 질문한다.](fc/FC0150.md)

- [FC0156 · 도메인 Member가 MemberEntity를 받아 변환하면 MemberEntity의 변경이 도메인에 영향을 준다는 의존성 문제를 짚었다.](fc/FC0156.md)

- [FC0152 · 의존 객체를 new로 직접 생성하는 대신 의존성 주입을 사용하는 이유를 설명해 달라고 묻는다.](fc/FC0152.md)

- [FC0154 · 구현체가 하나인 서비스에도 인터페이스를 두는 기준과 인터페이스를 사용하기 적절한 시점을 질문했다.](fc/FC0154.md)

- [FC0164 · 서비스에서 사용하는 DTO를 ui 패키지에 두면 서비스가 컨트롤러 계층에 의존하는 형태가 되는 것 아닌지 구성 이유를 질문한다.](fc/FC0164.md)

- [FC0166 · DataSource를 받아 내부에서 JdbcTemplate을 생성하는 UserDao 생성자를 제거하고 JdbcTemplate을 직접 주입받도록 한 이유를 논의했다.](fc/FC0166.md)

- [FC0162 · Service 간 의존을 허용할 조건과 Service 사이의 계층을 표현하는 방법을 고민해 보도록 제안했다.](fc/FC0162.md)

- [FC0147 · Caffeine을 Redis 및 다른 로컬 캐시 구현체와 비교해 선택 근거와 특징을 설명하도록 요청한다.](fc/FC0147.md)

- [FC0165 · AppUserService가 UserService 대신 Service 인터페이스를 구현한 것이 의도된 선택인지 물었다.](fc/FC0165.md)

- [FC0170 · 도메인 객체가 요청 DTO에 의존하면 DTO 변경이 도메인에도 영향을 줄 가능성이 있는데, 이 의존 관계가 적절한지 질문했다.](fc/FC0170.md)

- [FC0157 · LocalDateTime.now()처럼 제어하기 어려운 요소를 밖으로 분리해 테스트 가능한 영역을 확보하자는 제안이다.](fc/FC0157.md)

- [FC0167 · ReservationRepository가 JpaRepository 대신 Repository 인터페이스를 상속한 이유를 질문했다.](fc/FC0167.md)

- [FC0160 · Repository를 직접 호출하는 대신 도메인별 서비스를 주입해 재사용하고 직접 의존성을 줄이는 방안을 검토하도록 제안했다.](fc/FC0160.md)

- [FC0172 · ReservationDateService가 ReservationRepository에 의존하는 방향이 자연스러운지 물었다.](fc/FC0172.md)

- [FC0177 · 서비스가 DAO를 직접 의존하는 방식과 다른 서비스를 의존하는 방식의 차이를 고민하도록 질문한다.](fc/FC0177.md)

- [FC0178 · 여러 HTTP 클라이언트 중 RestClient를 선택한 이유를 질문했다.](fc/FC0178.md)

- [FC0158 · 구현체가 하나인 Repository에 인터페이스가 필요한지, 분리의 이점을 현재 누리거나 앞으로 누릴 가능성을 납득할 근거가 있는지 검토하도록 했다.](fc/FC0158.md)

- [FC0176 · 애플리케이션에서도 InMemoryUserRepository 대신 DB에 연결된 UserDao를 사용하도록 바꾸는 것을 제안한다.](fc/FC0176.md)

- [FC0171 · 서비스 테스트에서 mocking 라이브러리나 실제 객체 대신 직접 구현한 Fake 객체를 선택한 이유와 유지관리 부담을 논의한다.](fc/FC0171.md)

- [FC0180 · DAO를 인터페이스로 분리해 어떤 이점을 얻었는지 질문했다.](fc/FC0180.md)

- [FC0173 · 필드 주입 대신 생성자 주입을 사용하고 그 이유도 함께 고민하도록 요청한다.](fc/FC0173.md)

- [FC0184 · 추가 결제수단에서 요청 내용이 달라질 경우에도 현재 PaymentClient 인터페이스를 그대로 구현할 수 있는지 물었다.](fc/FC0184.md)

- [FC0181 · 스캔 대상 패키지를 바꿀 때 DispatcherServlet 코드를 수정하지 않도록 상수 대신 애플리케이션 실행 패키지를 기준으로 동적으로 정하는 방안을 제안했다.](fc/FC0181.md)

- [FC0175 · 도메인이 데이터 계층을 모르게 하는 레포지토리 패턴을 적용하려면 도메인 측 인터페이스와 데이터 계층 구현체로 의존 방향을 분리해야 한다고 설명했다.](fc/FC0175.md)

- [FC0174 · 서비스가 다른 서비스를 의존하는 구조는 허용할 수 있지만 순환 참조가 생기지 않도록 관리해야 한다는 의견이다.](fc/FC0174.md)

- [FC0186 · Order에서 OrderTable을 향한 의존성은 인터페이스로 끊고 반대 방향 의존성은 남겨 둔 이유를 묻는다.](fc/FC0186.md)

- [FC0185 · 일부 도메인에는 Repository를 정의하면서 다른 부분에서는 DAO를 직접 사용하는 설계 이유를 설명해 달라고 요청했다.](fc/FC0185.md)

- [FC0190 · 이번 단계부터 Lombok을 도입한 이유를 질문했다.](fc/FC0190.md)

- [FC0187 · RedisSerializer 구현체 중 GenericJackson2JsonRedisSerializer를 선택한 이유를 묻고, JdkSerializationRedisSerializer와의 차이와 절충점을 검토한다.](fc/FC0187.md)

- [FC0168 · CartController에 H2CartDao 구현체가 직접 주입되고 있음을 지적한다.](fc/FC0168.md)

- [FC0159 · SQL에 사용할 값을 PreparedStatementSetter를 통해 전달받는 방식도 구현해 볼 것을 제안한다.](fc/FC0159.md)

- [FC0161 · HandlerAdaptors가 JsonView의 내부 약속인 "model" 키를 알고 값을 넣어야 하는 결합을 우려했다.](fc/FC0161.md)

- [FC0188 · 여러 캐시 구현 중 Caffeine을 선택한 이유를 물었다.](fc/FC0188.md)

- [FC0191 · 사용하지 않는 의존성과 import 정리를 요청했고, 후속 리뷰에서는 HandlerMappers의 java.util.Objects import가 남아 있다고 지적했다.](fc/FC0191.md)

- [FC0182 · ManualHandler가 ModelAndView를 알고 있어도 괜찮은 의존 관계인지 질문했다.](fc/FC0182.md)


---

[전체 목차](README.md) · [FC 번호별 목차](FC_INDEX.md) · [← 이전: 데이터 관계·영속성](08-persistence.md) · [다음: 문서·개발·학습 과정 →](10-workflow.md)
