# 추상화·중복

[전체 목차](README.md) · [FC 번호별 목차](FC_INDEX.md) · [다음: 접근성·의미론 →](02-accessibility.md)

**관련 분야:** [의존성·교체 가능성](09-dependency.md) · [책임·계층 경계](19-responsibility.md)

## 이 분야의 FC

- [FC0003 · 모든 테스트 메서드에 반복되는 API 요청 로직을 별도 메서드로 추출하고, 중복 제거의 장점을 검토해 보자는 제안이다.](fc/FC0003.md)

- [FC0002 · 모든 테스트에서 반복되는 요청 실행 코드를 메서드로 분리해 중복을 제거하는 방안을 제안했다.](fc/FC0002.md)

- [FC0001 · 요구사항을 절차적으로 나열한 듯한 구현으로 요구사항의 복잡함이 코드에 그대로 드러나는 구조를 개선할 수 있을지 검토하자.](fc/FC0001.md)

- [FC0008 · ResponseEntity에서 HttpResponse를 만드는 빌더 코드를 정적 팩토리 메서드 HttpResponse.from(responseEntity)로 표현하는 대안을 제안했다.](fc/FC0008.md)

- [FC0012 · 생성자와 차이가 드러나지 않는 of 정적 팩토리 메서드를 별도로 사용하는 이유가 있는지 물었다.](fc/FC0012.md)

- [FC0005 · 이미 인터페이스인 JpaMemberRepository를 다시 추상화하여 얻는 이점이 무엇인지 질문했다.](fc/FC0005.md)

- [FC0013 · 기본 생성자에서 다른 생성자를 호출해 변수 초기화를 한 생성자로 모으고 그 장점을 생각해 보자고 제안했다.](fc/FC0013.md)

- [FC0007 · 테스트 준비 코드를 Fixture로 감싸는 것이 추가 탐색 깊이에 비해 실제로 가독성과 단순성을 높이는지, 현재 필요한 추상화인지 재검토하자는 의견이다.](fc/FC0007.md)

- [FC0009 · 여러 테스트에서 반복되는 코드를 메서드로 분리해 이후 테스트 추가에도 재사용할 수 있도록 제안했다.](fc/FC0009.md)

- [FC0004 · 관리자와 일반 사용자의 예약 생성 로직이 동일하므로 서비스 메서드를 중복으로 두기보다 로직에 차이가 생길 때 분리하는 방안을 제안했다.](fc/FC0004.md)

- [FC0017 · Controller를 직접 구현한 이유를 묻고, AbstractController에서 HTTP 메서드별 처리를 분기하는 구조를 검토하자고 제안했다.](fc/FC0017.md)

- [FC0020 · ManualHandlerMapping을 수정하지 않는 방향이라면 HandlerAdapter 도입을 고려해 보라고 제안했다.](fc/FC0020.md)

- [FC0025 · 생성 요청과 수정 요청에 실제 차이가 없다면 미래 확장만을 예상해 DTO를 미리 분리하지 않고 하나로 유지하는 방안을 제안한다.](fc/FC0025.md)

- [FC0027 · 여러 조회 메서드에 중복된 User 매핑 코드를 RowMapper 구현 클래스로 분리하도록 제안했다.](fc/FC0027.md)

- [FC0011 · TEMPLATES_PATH 정의가 RequestDispatcher에도 중복되어 있다.](fc/FC0011.md)

- [FC0030 · UserHistoryDao에도 작성한 JdbcTemplate을 적용해 보자고 제안했다.](fc/FC0030.md)

- [FC0029 · Reservation의 부생성자에서 필드 초기화를 반복하기보다 다른 생성자에 위임해 객체를 생성하자는 제안이다.](fc/FC0029.md)

- [FC0031 · 문자열을 RequestMethod로 변환하는 별도 구현 대신 enum의 valueOf 메서드를 활용할 수 있는지 제안했다.](fc/FC0031.md)

- [FC0032 · queryForObject와 query의 공통 구현을 추출하고, 반복되는 try-with-resources 구문까지 메서드로 묶어 중복을 줄이자고 제안했다.](fc/FC0032.md)

- [FC0033 · PreparedStatementSetter를 함수형 인터페이스로 정의했지만 그 특성을 활용하지 않는 것으로 보이는데, 그렇게 정의한 이유가 무엇인지 질문했다.](fc/FC0033.md)

- [FC0034 · 필요하다면 컬렉션을 일급 컬렉션으로 추상화하여 여러 검증 로직을 처리하도록 제안했다.](fc/FC0034.md)

- [FC0016 · ControllerAdvice의 상태 코드별 응답 구성에서 반복되는 규칙을 활용해 코드를 줄여 볼 것을 제안했다.](fc/FC0016.md)

- [FC0010 · 엔티티 영속 시각을 공통 구조로 래핑하면 개별 엔티티에 @EntityListeners를 선언하지 않아도 되겠다고 관찰했다.](fc/FC0010.md)

- [FC0019 · LocalTime도 LocalDate처럼 공통 포맷 처리를 적용하여 필드의 @JsonFormat을 제거할 수 있지 않은지 제안했다.](fc/FC0019.md)

- [FC0015 · 세션 처리 보완으로 addCookie()가 커질 수 있으므로 함수를 분리하는 방안을 제안했다.](fc/FC0015.md)

- [FC0018 · Content-Type:과 charset=utf-8 문자열 리터럴이 반복되는 부분을 재사용할 방법이 있는지 묻는다.](fc/FC0018.md)

- [FC0021 · 거리 구간에 따른 요금 계산을 전략 패턴으로 수행해 보는 방안을 제안한다.](fc/FC0021.md)

- [FC0023 · Predicate를 키로 둔 Map이 Map의 탐색 특성을 활용하는지 의문을 제기하고, 조건 판정과 View 생성을 함께 담은 클래스의 리스트를 대안으로 제안했다.](fc/FC0023.md)

- [FC0006 · 메모리와 데이터베이스처럼 서로 다른 저장 방식을 추상화하고 어떤 코드를 왜 재사용할지 고민하는 것을 학습 목표로 제시한다.](fc/FC0006.md)

- [FC0028 · CartItem의 필드를 각각 꺼내 응답 DTO를 만들기보다 CartItem 자체를 받는 생성 메서드를 추가하자는 제안이다.](fc/FC0028.md)

- [FC0024 · ContentType과 ContentTypeValue를 하나로 병합하는 방안을 제안했다.](fc/FC0024.md)

- [FC0022 · setAutoCommit, commit, rollback을 ConnectionContext로 한 번 더 감싸기보다 Connection에서 직접 호출해도 되지 않는지 논의했다.](fc/FC0022.md)


---

[전체 목차](README.md) · [FC 번호별 목차](FC_INDEX.md) · [다음: 접근성·의미론 →](02-accessibility.md)
