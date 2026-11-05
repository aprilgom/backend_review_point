# 백엔드 FC 번호별 목차

[전체 분야 목차](README.md)

FC 번호는 기존 식별자를 유지합니다. 제외된 FC는 이 목차에 포함하지 않습니다.

| FC | 분야 | 백엔드 점검 주제 |
| --- | --- | --- |
| [FC0001](fc/FC0001.md) | [추상화·중복](01-abstraction.md) | 요구사항을 절차적으로 나열한 듯한 구현으로 요구사항의 복잡함이 코드에 그대로 드러나는 구조를 개선할 수 있을지 검토하자. |
| [FC0002](fc/FC0002.md) | [추상화·중복](01-abstraction.md) | 모든 테스트에서 반복되는 요청 실행 코드를 메서드로 분리해 중복을 제거하는 방안을 제안했다. |
| [FC0003](fc/FC0003.md) | [추상화·중복](01-abstraction.md) | 모든 테스트 메서드에 반복되는 API 요청 로직을 별도 메서드로 추출하고, 중복 제거의 장점을 검토해 보자는 제안이다. |
| [FC0004](fc/FC0004.md) | [추상화·중복](01-abstraction.md) | 관리자와 일반 사용자의 예약 생성 로직이 동일하므로 서비스 메서드를 중복으로 두기보다 로직에 차이가 생길 때 분리하는 방안을 제안했다. |
| [FC0005](fc/FC0005.md) | [추상화·중복](01-abstraction.md) | 이미 인터페이스인 JpaMemberRepository를 다시 추상화하여 얻는 이점이 무엇인지 질문했다. |
| [FC0006](fc/FC0006.md) | [추상화·중복](01-abstraction.md) | 메모리와 데이터베이스처럼 서로 다른 저장 방식을 추상화하고 어떤 코드를 왜 재사용할지 고민하는 것을 학습 목표로 제시한다. |
| [FC0007](fc/FC0007.md) | [추상화·중복](01-abstraction.md) | 테스트 준비 코드를 Fixture로 감싸는 것이 추가 탐색 깊이에 비해 실제로 가독성과 단순성을 높이는지, 현재 필요한 추상화인지 재검토하자는 의견이다. |
| [FC0008](fc/FC0008.md) | [추상화·중복](01-abstraction.md) | ResponseEntity에서 HttpResponse를 만드는 빌더 코드를 정적 팩토리 메서드 HttpResponse.from(responseEntity)로 표현하는 대안을 제안했다. |
| [FC0009](fc/FC0009.md) | [추상화·중복](01-abstraction.md) | 여러 테스트에서 반복되는 코드를 메서드로 분리해 이후 테스트 추가에도 재사용할 수 있도록 제안했다. |
| [FC0010](fc/FC0010.md) | [추상화·중복](01-abstraction.md) | 엔티티 영속 시각을 공통 구조로 래핑하면 개별 엔티티에 @EntityListeners를 선언하지 않아도 되겠다고 관찰했다. |
| [FC0011](fc/FC0011.md) | [추상화·중복](01-abstraction.md) | TEMPLATES_PATH 정의가 RequestDispatcher에도 중복되어 있다. |
| [FC0012](fc/FC0012.md) | [추상화·중복](01-abstraction.md) | 생성자와 차이가 드러나지 않는 of 정적 팩토리 메서드를 별도로 사용하는 이유가 있는지 물었다. |
| [FC0013](fc/FC0013.md) | [추상화·중복](01-abstraction.md) | 기본 생성자에서 다른 생성자를 호출해 변수 초기화를 한 생성자로 모으고 그 장점을 생각해 보자고 제안했다. |
| [FC0015](fc/FC0015.md) | [추상화·중복](01-abstraction.md) | 세션 처리 보완으로 addCookie()가 커질 수 있으므로 함수를 분리하는 방안을 제안했다. |
| [FC0016](fc/FC0016.md) | [추상화·중복](01-abstraction.md) | ControllerAdvice의 상태 코드별 응답 구성에서 반복되는 규칙을 활용해 코드를 줄여 볼 것을 제안했다. |
| [FC0017](fc/FC0017.md) | [추상화·중복](01-abstraction.md) | Controller를 직접 구현한 이유를 묻고, AbstractController에서 HTTP 메서드별 처리를 분기하는 구조를 검토하자고 제안했다. |
| [FC0018](fc/FC0018.md) | [추상화·중복](01-abstraction.md) | Content-Type:과 charset=utf-8 문자열 리터럴이 반복되는 부분을 재사용할 방법이 있는지 묻는다. |
| [FC0019](fc/FC0019.md) | [추상화·중복](01-abstraction.md) | LocalTime도 LocalDate처럼 공통 포맷 처리를 적용하여 필드의 @JsonFormat을 제거할 수 있지 않은지 제안했다. |
| [FC0020](fc/FC0020.md) | [추상화·중복](01-abstraction.md) | ManualHandlerMapping을 수정하지 않는 방향이라면 HandlerAdapter 도입을 고려해 보라고 제안했다. |
| [FC0021](fc/FC0021.md) | [추상화·중복](01-abstraction.md) | 거리 구간에 따른 요금 계산을 전략 패턴으로 수행해 보는 방안을 제안한다. |
| [FC0022](fc/FC0022.md) | [추상화·중복](01-abstraction.md) | setAutoCommit, commit, rollback을 ConnectionContext로 한 번 더 감싸기보다 Connection에서 직접 호출해도 되지 않는지 논의했다. |
| [FC0023](fc/FC0023.md) | [추상화·중복](01-abstraction.md) | Predicate를 키로 둔 Map이 Map의 탐색 특성을 활용하는지 의문을 제기하고, 조건 판정과 View 생성을 함께 담은 클래스의 리스트를 대안으로 제안했다. |
| [FC0024](fc/FC0024.md) | [추상화·중복](01-abstraction.md) | ContentType과 ContentTypeValue를 하나로 병합하는 방안을 제안했다. |
| [FC0025](fc/FC0025.md) | [추상화·중복](01-abstraction.md) | 생성 요청과 수정 요청에 실제 차이가 없다면 미래 확장만을 예상해 DTO를 미리 분리하지 않고 하나로 유지하는 방안을 제안한다. |
| [FC0027](fc/FC0027.md) | [추상화·중복](01-abstraction.md) | 여러 조회 메서드에 중복된 User 매핑 코드를 RowMapper 구현 클래스로 분리하도록 제안했다. |
| [FC0028](fc/FC0028.md) | [추상화·중복](01-abstraction.md) | CartItem의 필드를 각각 꺼내 응답 DTO를 만들기보다 CartItem 자체를 받는 생성 메서드를 추가하자는 제안이다. |
| [FC0029](fc/FC0029.md) | [추상화·중복](01-abstraction.md) | Reservation의 부생성자에서 필드 초기화를 반복하기보다 다른 생성자에 위임해 객체를 생성하자는 제안이다. |
| [FC0030](fc/FC0030.md) | [추상화·중복](01-abstraction.md) | UserHistoryDao에도 작성한 JdbcTemplate을 적용해 보자고 제안했다. |
| [FC0031](fc/FC0031.md) | [추상화·중복](01-abstraction.md) | 문자열을 RequestMethod로 변환하는 별도 구현 대신 enum의 valueOf 메서드를 활용할 수 있는지 제안했다. |
| [FC0032](fc/FC0032.md) | [추상화·중복](01-abstraction.md) | queryForObject와 query의 공통 구현을 추출하고, 반복되는 try-with-resources 구문까지 메서드로 묶어 중복을 줄이자고 제안했다. |
| [FC0033](fc/FC0033.md) | [추상화·중복](01-abstraction.md) | PreparedStatementSetter를 함수형 인터페이스로 정의했지만 그 특성을 활용하지 않는 것으로 보이는데, 그렇게 정의한 이유가 무엇인지 질문했다. |
| [FC0034](fc/FC0034.md) | [추상화·중복](01-abstraction.md) | 필요하다면 컬렉션을 일급 컬렉션으로 추상화하여 여러 검증 로직을 처리하도록 제안했다. |
| [FC0036](fc/FC0036.md) | [접근성·의미론](02-accessibility.md) | HTML의 lang 속성에 대해 추가로 학습해 보자는 제안이다. |
| [FC0037](fc/FC0037.md) | [접근성·의미론](02-accessibility.md) | HTML id가 문서 전체에서 고유해야 한다는 기준에 따라 반복되는 방 목록을 포함해 id 사용을 전반적으로 점검하도록 요청했다. |
| [FC0041](fc/FC0041.md) | [접근성·의미론](02-accessibility.md) | 이미지 요소의 alt가 어떤 용도로 사용되는지 물으며 관련 문서 확인을 권했다. |
| [FC0053](fc/FC0053.md) | [API·공개 인터페이스 계약](03-api-contract.md) | 항상 기본값만 사용하는 것으로 보이는 whiteName과 blackName을 요청 파라미터로 받는 이유를 질문했다. |
| [FC0054](fc/FC0054.md) | [API·공개 인터페이스 계약](03-api-contract.md) | JSON 본문을 사용하지 않고 RequestParam으로 입력을 받는다면 application/json 대신 다른 Content-Type을 고려하도록 제안했다. |
| [FC0055](fc/FC0055.md) | [API·공개 인터페이스 계약](03-api-contract.md) | HandlerExecution이 String뿐 아니라 ModelAndView 등 여러 반환 타입을 지원하도록 바꾸자고 제안했다. |
| [FC0057](fc/FC0057.md) | [API·공개 인터페이스 계약](03-api-contract.md) | 로그인 상태에서 GET /login 요청 시 index.html로 리다이렉트하는 요구사항이 동작하지 않는 것으로 보여 확인을 요청했다. |
| [FC0058](fc/FC0058.md) | [API·공개 인터페이스 계약](03-api-contract.md) | RequestUri의 hasRequestParameters 메서드가 테스트에서만 사용되는 메서드임을 지적했다. |
| [FC0059](fc/FC0059.md) | [API·공개 인터페이스 계약](03-api-contract.md) | API와 페이지 URL 경로의 결정 기준을 묻고 RESTful 경로 설계와 자신의 선택 기준을 고민해 볼 것을 제안했다. |
| [FC0060](fc/FC0060.md) | [API·공개 인터페이스 계약](03-api-contract.md) | LoginMember 타입만으로 인자 해석 대상을 정하지 말고, hasParameterAnnotation()을 활용해 특정 조건을 만족하는 파라미터에만 로그인 정보를 제공하도록 제안했다. |
| [FC0061](fc/FC0061.md) | [API·공개 인터페이스 계약](03-api-contract.md) | 본문을 반환하지 않는 성공 응답에 200을 사용한 이유와 이 경우 적절한 응답 상태 코드를 묻는다. |
| [FC0062](fc/FC0062.md) | [API·공개 인터페이스 계약](03-api-contract.md) | 쿠키를 세미콜론과 공백 한 개로 분리하면 공백이 없거나 여러 개인 입력을 제대로 파싱하지 못할 수 있으므로 공백을 정리해 처리하도록 제안한다. |
| [FC0063](fc/FC0063.md) | [API·공개 인터페이스 계약](03-api-contract.md) | RequestMapping의 method가 배열인 만큼 여러 RequestMethod를 입력했을 때의 매핑 동작을 명확히 정해보자고 제안했다. |
| [FC0064](fc/FC0064.md) | [API·공개 인터페이스 계약](03-api-contract.md) | 직접 사용하지 않는 기본 생성자의 접근 제한자를 public에서 protected로 변경할 것을 제안한다. |
| [FC0065](fc/FC0065.md) | [API·공개 인터페이스 계약](03-api-contract.md) | JSON 응답에 Content-Type을 지정했을 때와 지정하지 않았을 때의 차이를 질문했다. |
| [FC0066](fc/FC0066.md) | [API·공개 인터페이스 계약](03-api-contract.md) | 예약 가능 여부를 포함하는 시간 조회 API의 요청과 응답을 현재 형태로 설계한 이유를 질문했다. |
| [FC0067](fc/FC0067.md) | [API·공개 인터페이스 계약](03-api-contract.md) | API 안정성을 DTO 사용 근거로 들면서 요청에만 DTO를 적용한 이유와, 도메인 변경이 응답 형식에도 영향을 줄 가능성을 질문했다. |
| [FC0069](fc/FC0069.md) | [API·공개 인터페이스 계약](03-api-contract.md) | 별도 사용처가 없는 기본 생성자의 접근 범위를 protected에서 public으로 넓힌 이유를 질문했다. |
| [FC0070](fc/FC0070.md) | [API·공개 인터페이스 계약](03-api-contract.md) | Member의 @NoArgsConstructor에 생성자 접근 수준 설정이 빠져 있다고 지적한다. |
| [FC0071](fc/FC0071.md) | [API·공개 인터페이스 계약](03-api-contract.md) | 정적 팩토리 메서드가 있고 생성자를 별도로 사용하지 않는다면 RequestUri 생성자를 private으로 제한하는 방안을 제안했다. |
| [FC0072](fc/FC0072.md) | [API·공개 인터페이스 계약](03-api-contract.md) | 상품 수정 API에서 PUT과 PATCH의 차이를 이해하고 PATCH 사용도 고려했는지 묻는다. |
| [FC0073](fc/FC0073.md) | [빌드·환경·배포](04-build-config.md) | ddl-auto를 update로 설정할 수도 있는데 validate를 선택한 이유가 무엇인지 묻는다. |
| [FC0074](fc/FC0074.md) | [빌드·환경·배포](04-build-config.md) | rest-assured 의존성을 실제로 사용하는지, 해당 모듈이 있는 상태에서 작성자 환경에서도 빌드와 실행이 정상인지 확인하고 싶다. |
| [FC0075](fc/FC0075.md) | [빌드·환경·배포](04-build-config.md) | ddl-auto의 create-drop 동작과 다른 옵션을 정리하고, 운영 환경에 적합한 옵션을 검토해 보라고 제안했다. |
| [FC0076](fc/FC0076.md) | [빌드·환경·배포](04-build-config.md) | 추가한 JPA 설정 옵션 각각이 무엇을 의미하는지 설명을 요청했다. |
| [FC0077](fc/FC0077.md) | [빌드·환경·배포](04-build-config.md) | 애플리케이션이 실행되지 않는다고 보고하고, 테이블 구조 문제인지 확인해 달라고 요청했다. |
| [FC0078](fc/FC0078.md) | [빌드·환경·배포](04-build-config.md) | 모듈별 build.gradle 설정에 불필요한 의존성이 포함되어 있지 않은지 검토하도록 질문한다. |
| [FC0079](fc/FC0079.md) | [빌드·환경·배포](04-build-config.md) | Gradle 빌드 시 CSS를 불러오지 못하는 문제를 보고하고, 정적 리소스를 기본 서블릿에 매핑하는 web.xml 추가를 제안했다. |
| [FC0080](fc/FC0080.md) | [빌드·환경·배포](04-build-config.md) | web과 core의 빌드 설정에 중복 선언된 의존성을 제거해 보자고 제안했다. |
| [FC0081](fc/FC0081.md) | [빌드·환경·배포](04-build-config.md) | 버전을 명시해 추가하는 라이브러리는 해당 버전이 최신인지 확인해 보면 좋겠다고 제안했다. |
| [FC0082](fc/FC0082.md) | [빌드·환경·배포](04-build-config.md) | JUnit 4.13.1 테스트 의존성을 추가한 이유를 묻는다. |
| [FC0083](fc/FC0083.md) | [빌드·환경·배포](04-build-config.md) | 개발용 초기 데이터를 애플리케이션 코드로 관리하는 대신 data.sql로 초기화하자고 제안한다. |
| [FC0084](fc/FC0084.md) | [빌드·환경·배포](04-build-config.md) | 외부 API URL을 코드에 직접 넣지 않고 외부 설정에서 관리하도록 바꾸고 그 장점을 생각해 볼 것을 제안했다. |
| [FC0087](fc/FC0087.md) | [빌드·환경·배포](04-build-config.md) | 공유된 배포 주소에 접근할 수 없다고 보고하며 배포 상태 확인을 요청했다. |
| [FC0088](fc/FC0088.md) | [빌드·환경·배포](04-build-config.md) | 향후 배포를 고려해 CSS 주소를 localhost가 포함된 절대경로 대신 상대경로로 바꾸는 것을 제안한다. |
| [FC0089](fc/FC0089.md) | [빌드·환경·배포](04-build-config.md) | 특정 테스트 클래스에만 있는 프로파일 설정을 application.yml로 옮겨 설정을 명시적으로 관리하도록 제안했다. |
| [FC0090](fc/FC0090.md) | [빌드·환경·배포](04-build-config.md) | Redis 설정에 별도의 프로파일을 지정한 이유를 묻는다. |
| [FC0091](fc/FC0091.md) | [빌드·환경·배포](04-build-config.md) | 각 모듈마다 .gitignore 파일이 생성된 이유를 질문했다. |
| [FC0094](fc/FC0094.md) | [빌드·환경·배포](04-build-config.md) | 내용이 없는 application.properties 파일이 추가되어 있음을 지적했다. |
| [FC0095](fc/FC0095.md) | [빌드·환경·배포](04-build-config.md) | 결제 API 클라이언트의 연결 타임아웃을 5초, 읽기 타임아웃을 30초로 설정한 이유를 질문했다. |
| [FC0096](fc/FC0096.md) | [빌드·환경·배포](04-build-config.md) | 변경된 banner.txt 파일의 용도가 무엇인지 질문한다. |
| [FC0097](fc/FC0097.md) | [비동기·동시성](05-concurrency.md) | 복제 지연 대응으로 reader 조회 결과가 없을 때 writer를 조회하는 방식을 선택한 이유를 묻는다. |
| [FC0098](fc/FC0098.md) | [비동기·동시성](05-concurrency.md) | 요청마다 스레드를 새로 생성하는 방식에서 어떤 문제가 생길 수 있는지 고민해 보도록 권했다. |
| [FC0099](fc/FC0099.md) | [비동기·동시성](05-concurrency.md) | calculate 메서드에 synchronized를 붙이면 테스트가 통과하는 이유를 질문했다. |
| [FC0100](fc/FC0100.md) | [비동기·동시성](05-concurrency.md) | Session 내부 HashMap에도 동시성 고려가 필요한지, 필요하다면 어떤 상황에서 동시 접근이 발생하는지 질문했다. |
| [FC0101](fc/FC0101.md) | [비동기·동시성](05-concurrency.md) | 대기 생성 요청이 거의 동시에 들어오는 상황을 검토하고 트랜잭션 격리 수준을 확인해보자는 제안이다. |
| [FC0102](fc/FC0102.md) | [비동기·동시성](05-concurrency.md) | ArgumentResolver와 Interceptor를 사용할 때 각각 요청이 처리되는 순서를 질문한다. |
| [FC0103](fc/FC0103.md) | [비동기·동시성](05-concurrency.md) | 동시 요청이 애플리케이션의 중복 검사를 함께 통과하면 중복 저장이 가능하므로 데이터베이스에서도 정합성을 보장해야 한다는 우려다. |
| [FC0104](fc/FC0104.md) | [비동기·동시성](05-concurrency.md) | 여러 스레드가 동시에 접근하는 세션 저장소를 ConcurrentHashMap으로 처리해 보자고 제안했다. |
| [FC0105](fc/FC0105.md) | [비동기·동시성](05-concurrency.md) | 학습 차원에서 ThreadLocal이 무엇인지 설명해 달라고 질문했다. |
| [FC0106](fc/FC0106.md) | [비동기·동시성](05-concurrency.md) | 스레드 풀의 최대 스레드 수를 보통 어느 정도로 설정하는지 학습해 보도록 제안했다. |
| [FC0107](fc/FC0107.md) | [비동기·동시성](05-concurrency.md) | RedisTemplate의 내부 호출이 동기인지 비동기인지, 그리고 캐시 TTL 연장 메서드에 비동기를 사용한 이유가 무엇인지 물었다. |
| [FC0108](fc/FC0108.md) | [비동기·동시성](05-concurrency.md) | Executors의 여러 스레드 풀 생성 방식 중 FixedThreadPool을 선택한 이유를 질문했다. |
| [FC0109](fc/FC0109.md) | [비동기·동시성](05-concurrency.md) | 예약과 대기의 API가 분리된 상태에서 예약 취소와 해당 슬롯의 대기 신청이 동시에 발생해도 문제가 없는지 검토하도록 요청했다. |
| [FC0110](fc/FC0110.md) | [비동기·동시성](05-concurrency.md) | 작업 실행에 submit() 대신 execute()를 선택한 이유를 질문했다. |
| [FC0111](fc/FC0111.md) | [비동기·동시성](05-concurrency.md) | Long과 AtomicLong의 차이와 예약 ID 생성에 AtomicLong을 사용하는 이유를 설명하도록 질문했다. |
| [FC0112](fc/FC0112.md) | [엔티티 동등성·식별](06-identity.md) | id를 예약 식별자로 본다면 같은 id의 예약도 추가할 수 있는지 테스트하고, 예약 번호라고 해도 고유해야 하지 않는지 검토하도록 질문했다. |
| [FC0113](fc/FC0113.md) | [엔티티 동등성·식별](06-identity.md) | 필요한 경우 equals와 hashCode를 재정의해 사용할 수 있다는 의견을 제시했다. |
| [FC0114](fc/FC0114.md) | [엔티티 동등성·식별](06-identity.md) | Reservation을 비롯한 엔티티의 동등성을 나머지 속성이 아니라 id만으로 판단하도록 다뤄보자고 제안했다. |
| [FC0115](fc/FC0115.md) | [엔티티 동등성·식별](06-identity.md) | `GenerationType.IDENTITY`의 ID 부여 방식과 다른 기본 키 생성 전략 대신 이를 선택한 이유를 물었다. |
| [FC0116](fc/FC0116.md) | [쿼리·데이터 조작](07-data-query.md) | 조회 쿼리에서 컬럼을 명시하지 않고 SELECT *를 그대로 사용할 때의 단점을 검토했는지 질문한다. |
| [FC0117](fc/FC0117.md) | [쿼리·데이터 조작](07-data-query.md) | 예약과 대기를 상태로만 구분한다면, 예약 존재 여부 조회에서도 RESERVED 상태만 검증해야 하지 않는지 질문했다. |
| [FC0118](fc/FC0118.md) | [쿼리·데이터 조작](07-data-query.md) | cartIds를 먼저 추출하는 대신 고객 이름으로 고객 ID를 구한 뒤 해당 고객의 장바구니 항목을 직접 조회하는 방식을 제안했다. |
| [FC0119](fc/FC0119.md) | [쿼리·데이터 조작](07-data-query.md) | 조회 결과에 covid.id와 programmer.id를 모두 포함하기보다 둘 중 하나만 사용해도 된다고 제안했다. |
| [FC0120](fc/FC0120.md) | [쿼리·데이터 조작](07-data-query.md) | existReservationByTimeId 함수가 항상 true를 반환하는 것은 아닌지 확인을 요청했다. |
| [FC0121](fc/FC0121.md) | [쿼리·데이터 조작](07-data-query.md) | 간단하게 표현할 수 있는 쿼리는 직접 작성하는 대신 Spring Data JPA의 기능을 더 활용해 볼 것을 제안했다. |
| [FC0122](fc/FC0122.md) | [쿼리·데이터 조작](07-data-query.md) | 모든 SQL 파라미터를 String으로 변환해 setString으로 바인딩하면 어떤 문제가 생길 수 있는지 질문했다. |
| [FC0123](fc/FC0123.md) | [쿼리·데이터 조작](07-data-query.md) | 구간을 변경할 때 기존 구간을 삭제하고 두 구간을 삽입하는 대신, 하나는 삽입하고 하나는 갱신하는 방식을 검토하자는 제안이다. |
| [FC0124](fc/FC0124.md) | [쿼리·데이터 조작](07-data-query.md) | 간단한 존재 여부 조회는 직접 쿼리를 작성하는 대신 existsByEmailAndPassword 형태의 메서드를 사용하는 대안도 검토하자는 제안이다. |
| [FC0126](fc/FC0126.md) | [쿼리·데이터 조작](07-data-query.md) | 인기 테마를 하나의 쿼리로 조회한 이유와, 예약 조회 후 테마 ID로 테마를 일괄 조회하는 대안을 검토했는지 논의했다. |
| [FC0127](fc/FC0127.md) | [쿼리·데이터 조작](07-data-query.md) | INNER JOIN을 선택한 이유와 LEFT JOIN과의 결과 차이, 시간 정보가 누락된 예약의 조회 결과를 질문했다. |
| [FC0128](fc/FC0128.md) | [쿼리·데이터 조작](07-data-query.md) | 예약 대기 순번을 created_at 대신 자동 증가하는 id 기준으로 계산해도 되는지 검토하자는 논의다. |
| [FC0129](fc/FC0129.md) | [데이터 관계·영속성](08-persistence.md) | 상품의 활성 상태를 장바구니에서 반영하려면 상품 객체 자체가 아니라 ID만 저장하고 필요할 때 상품을 조회하도록 바꾸자고 제안했다. |
| [FC0130](fc/FC0130.md) | [데이터 관계·영속성](08-persistence.md) | 질문과 답변을 일대일로 설정한 이유를 묻고, 실제 서비스 흐름과 가능한 사례를 검토해 연관관계를 결정할 것을 제안했다. |
| [FC0131](fc/FC0131.md) | [데이터 관계·영속성](08-persistence.md) | Reservation이 Payment를 참조하는 대신 Payment가 Reservation을 참조하도록 설계한 이유를 질문했다. |
| [FC0132](fc/FC0132.md) | [데이터 관계·영속성](08-persistence.md) | 향후 변경을 줄이려는 이유로 DB 제약을 생략하거나 요구사항보다 느슨하게 두기보다, 현재 요구사항과 데이터 무결성에 맞춰 제약을 설정해야 하는지 논의했다. |
| [FC0133](fc/FC0133.md) | [데이터 관계·영속성](08-persistence.md) | 예약 시간을 삭제할 때 연결된 예약까지 삭제해야 하는 요구사항이 있는지 확인하고, 예약이 남아 있으면 오류로 삭제를 막는 방안을 제안했다. |
| [FC0134](fc/FC0134.md) | [데이터 관계·영속성](08-persistence.md) | 연관 도메인을 객체로 참조해야 하는지, ID 참조만으로 충분한지 설계할 때 검토해보라고 제안했다. |
| [FC0135](fc/FC0135.md) | [데이터 관계·영속성](08-persistence.md) | MenuProduct가 Menu를 다대일로 참조하는 대신 Menu가 MenuProduct를 일대다로 참조하도록 선택한 이유를 물었다. |
| [FC0136](fc/FC0136.md) | [데이터 관계·영속성](08-persistence.md) | Reservation의 연관관계를 항상 객체 참조로 표현해야 하는지, Member 객체 대신 회원 ID만 보유하는 약한 연관관계로 설계할 수도 있는지 고민해 보도록 제안했다. |
| [FC0137](fc/FC0137.md) | [데이터 관계·영속성](08-persistence.md) | 엔티티 매핑의 `@Table`과 `@Column`을 생략할 수 있다는 의견을 제시한다. |
| [FC0138](fc/FC0138.md) | [데이터 관계·영속성](08-persistence.md) | @JoinColumn의 name을 생략했을 때 어떻게 동작하는지 확인하도록 제안했다. |
| [FC0139](fc/FC0139.md) | [데이터 관계·영속성](08-persistence.md) | OrderTable이 TableGroup을 객체 연관관계로 보유하도록 선택한 이유를 질문했다. |
| [FC0140](fc/FC0140.md) | [데이터 관계·영속성](08-persistence.md) | @ManyToOne 단방향 매핑을 선택한 이유와 양방향 매핑에서 고려해야 할 구체적인 문제를 질문했다. |
| [FC0141](fc/FC0141.md) | [데이터 관계·영속성](08-persistence.md) | @ManyToOne의 fetch를 LAZY로 선택한 이유와 기본값이 EAGER인 이유를 질문했다. |
| [FC0142](fc/FC0142.md) | [데이터 관계·영속성](08-persistence.md) | Section이 Line과 Station의 ID만 보유하기보다 해당 객체를 직접 보유하는 관계 표현을 제안한다. |
| [FC0143](fc/FC0143.md) | [데이터 관계·영속성](08-persistence.md) | 엔티티의 생성 시간과 마지막 수정 시간을 관리해야 한다면 수동 처리 대신 Auditing으로 자동 관리하도록 제안했다. |
| [FC0144](fc/FC0144.md) | [데이터 관계·영속성](08-persistence.md) | JPA 엔티티에 기본 생성자가 필요한 이유를 설명해 달라고 질문했다. |
| [FC0145](fc/FC0145.md) | [데이터 관계·영속성](08-persistence.md) | 이미 특정 구간에 속한 역을 삭제할 때 어떻게 처리되는지 확인한다. |
| [FC0146](fc/FC0146.md) | [의존성·교체 가능성](09-dependency.md) | 인터페이스를 분리한 뒤에도 알고리즘 변경 시 서비스 내부 구현을 수정해야 하는 의존 구조를 검토하고, OCP 관점에서 교체 가능한 구조를 고민하도록 제안한다. |
| [FC0147](fc/FC0147.md) | [의존성·교체 가능성](09-dependency.md) | Caffeine을 Redis 및 다른 로컬 캐시 구현체와 비교해 선택 근거와 특징을 설명하도록 요청한다. |
| [FC0149](fc/FC0149.md) | [의존성·교체 가능성](09-dependency.md) | 컨트롤러 인스턴스를 매번 새로 생성해야 하는지 검토하고, 싱글턴으로 재사용하는 방식을 고려해볼 것을 제안했다. |
| [FC0150](fc/FC0150.md) | [의존성·교체 가능성](09-dependency.md) | 컨트롤러의 실제 인스턴스를 만들지 않고 클래스 타입만 보관하도록 구현한 이유를 질문한다. |
| [FC0151](fc/FC0151.md) | [의존성·교체 가능성](09-dependency.md) | JPA 리포지터리를 직접 사용하지 않고 구현체에 주입해서 사용하는 이유를 물었다. |
| [FC0152](fc/FC0152.md) | [의존성·교체 가능성](09-dependency.md) | 의존 객체를 new로 직접 생성하는 대신 의존성 주입을 사용하는 이유를 설명해 달라고 묻는다. |
| [FC0153](fc/FC0153.md) | [의존성·교체 가능성](09-dependency.md) | 외부에서 의존성을 주입받는 구조가 되었으므로 일부 클래스를 제외하면 mvc로 옮겨도 mvc가 app을 의존하지 않을 것으로 보인다고 확인했다. |
| [FC0154](fc/FC0154.md) | [의존성·교체 가능성](09-dependency.md) | 구현체가 하나인 서비스에도 인터페이스를 두는 기준과 인터페이스를 사용하기 적절한 시점을 질문했다. |
| [FC0155](fc/FC0155.md) | [의존성·교체 가능성](09-dependency.md) | DispatcherServlet에서 특정 매핑 구현체를 직접 생성하는 대신 HandlerMapping 구현체를 리플렉션으로 찾는 방식을 고려해 보자는 의견이다. |
| [FC0156](fc/FC0156.md) | [의존성·교체 가능성](09-dependency.md) | 도메인 Member가 MemberEntity를 받아 변환하면 MemberEntity의 변경이 도메인에 영향을 준다는 의존성 문제를 짚었다. |
| [FC0157](fc/FC0157.md) | [의존성·교체 가능성](09-dependency.md) | LocalDateTime.now()처럼 제어하기 어려운 요소를 밖으로 분리해 테스트 가능한 영역을 확보하자는 제안이다. |
| [FC0158](fc/FC0158.md) | [의존성·교체 가능성](09-dependency.md) | 구현체가 하나인 Repository에 인터페이스가 필요한지, 분리의 이점을 현재 누리거나 앞으로 누릴 가능성을 납득할 근거가 있는지 검토하도록 했다. |
| [FC0159](fc/FC0159.md) | [의존성·교체 가능성](09-dependency.md) | SQL에 사용할 값을 PreparedStatementSetter를 통해 전달받는 방식도 구현해 볼 것을 제안한다. |
| [FC0160](fc/FC0160.md) | [의존성·교체 가능성](09-dependency.md) | Repository를 직접 호출하는 대신 도메인별 서비스를 주입해 재사용하고 직접 의존성을 줄이는 방안을 검토하도록 제안했다. |
| [FC0161](fc/FC0161.md) | [의존성·교체 가능성](09-dependency.md) | HandlerAdaptors가 JsonView의 내부 약속인 "model" 키를 알고 값을 넣어야 하는 결합을 우려했다. |
| [FC0162](fc/FC0162.md) | [의존성·교체 가능성](09-dependency.md) | Service 간 의존을 허용할 조건과 Service 사이의 계층을 표현하는 방법을 고민해 보도록 제안했다. |
| [FC0164](fc/FC0164.md) | [의존성·교체 가능성](09-dependency.md) | 서비스에서 사용하는 DTO를 ui 패키지에 두면 서비스가 컨트롤러 계층에 의존하는 형태가 되는 것 아닌지 구성 이유를 질문한다. |
| [FC0165](fc/FC0165.md) | [의존성·교체 가능성](09-dependency.md) | AppUserService가 UserService 대신 Service 인터페이스를 구현한 것이 의도된 선택인지 물었다. |
| [FC0166](fc/FC0166.md) | [의존성·교체 가능성](09-dependency.md) | DataSource를 받아 내부에서 JdbcTemplate을 생성하는 UserDao 생성자를 제거하고 JdbcTemplate을 직접 주입받도록 한 이유를 논의했다. |
| [FC0167](fc/FC0167.md) | [의존성·교체 가능성](09-dependency.md) | ReservationRepository가 JpaRepository 대신 Repository 인터페이스를 상속한 이유를 질문했다. |
| [FC0168](fc/FC0168.md) | [의존성·교체 가능성](09-dependency.md) | CartController에 H2CartDao 구현체가 직접 주입되고 있음을 지적한다. |
| [FC0170](fc/FC0170.md) | [의존성·교체 가능성](09-dependency.md) | 도메인 객체가 요청 DTO에 의존하면 DTO 변경이 도메인에도 영향을 줄 가능성이 있는데, 이 의존 관계가 적절한지 질문했다. |
| [FC0171](fc/FC0171.md) | [의존성·교체 가능성](09-dependency.md) | 서비스 테스트에서 mocking 라이브러리나 실제 객체 대신 직접 구현한 Fake 객체를 선택한 이유와 유지관리 부담을 논의한다. |
| [FC0172](fc/FC0172.md) | [의존성·교체 가능성](09-dependency.md) | ReservationDateService가 ReservationRepository에 의존하는 방향이 자연스러운지 물었다. |
| [FC0173](fc/FC0173.md) | [의존성·교체 가능성](09-dependency.md) | 필드 주입 대신 생성자 주입을 사용하고 그 이유도 함께 고민하도록 요청한다. |
| [FC0174](fc/FC0174.md) | [의존성·교체 가능성](09-dependency.md) | 서비스가 다른 서비스를 의존하는 구조는 허용할 수 있지만 순환 참조가 생기지 않도록 관리해야 한다는 의견이다. |
| [FC0175](fc/FC0175.md) | [의존성·교체 가능성](09-dependency.md) | 도메인이 데이터 계층을 모르게 하는 레포지토리 패턴을 적용하려면 도메인 측 인터페이스와 데이터 계층 구현체로 의존 방향을 분리해야 한다고 설명했다. |
| [FC0176](fc/FC0176.md) | [의존성·교체 가능성](09-dependency.md) | 애플리케이션에서도 InMemoryUserRepository 대신 DB에 연결된 UserDao를 사용하도록 바꾸는 것을 제안한다. |
| [FC0177](fc/FC0177.md) | [의존성·교체 가능성](09-dependency.md) | 서비스가 DAO를 직접 의존하는 방식과 다른 서비스를 의존하는 방식의 차이를 고민하도록 질문한다. |
| [FC0178](fc/FC0178.md) | [의존성·교체 가능성](09-dependency.md) | 여러 HTTP 클라이언트 중 RestClient를 선택한 이유를 질문했다. |
| [FC0180](fc/FC0180.md) | [의존성·교체 가능성](09-dependency.md) | DAO를 인터페이스로 분리해 어떤 이점을 얻었는지 질문했다. |
| [FC0181](fc/FC0181.md) | [의존성·교체 가능성](09-dependency.md) | 스캔 대상 패키지를 바꿀 때 DispatcherServlet 코드를 수정하지 않도록 상수 대신 애플리케이션 실행 패키지를 기준으로 동적으로 정하는 방안을 제안했다. |
| [FC0182](fc/FC0182.md) | [의존성·교체 가능성](09-dependency.md) | ManualHandler가 ModelAndView를 알고 있어도 괜찮은 의존 관계인지 질문했다. |
| [FC0184](fc/FC0184.md) | [의존성·교체 가능성](09-dependency.md) | 추가 결제수단에서 요청 내용이 달라질 경우에도 현재 PaymentClient 인터페이스를 그대로 구현할 수 있는지 물었다. |
| [FC0185](fc/FC0185.md) | [의존성·교체 가능성](09-dependency.md) | 일부 도메인에는 Repository를 정의하면서 다른 부분에서는 DAO를 직접 사용하는 설계 이유를 설명해 달라고 요청했다. |
| [FC0186](fc/FC0186.md) | [의존성·교체 가능성](09-dependency.md) | Order에서 OrderTable을 향한 의존성은 인터페이스로 끊고 반대 방향 의존성은 남겨 둔 이유를 묻는다. |
| [FC0187](fc/FC0187.md) | [의존성·교체 가능성](09-dependency.md) | RedisSerializer 구현체 중 GenericJackson2JsonRedisSerializer를 선택한 이유를 묻고, JdkSerializationRedisSerializer와의 차이와 절충점을 검토한다. |
| [FC0188](fc/FC0188.md) | [의존성·교체 가능성](09-dependency.md) | 여러 캐시 구현 중 Caffeine을 선택한 이유를 물었다. |
| [FC0190](fc/FC0190.md) | [의존성·교체 가능성](09-dependency.md) | 이번 단계부터 Lombok을 도입한 이유를 질문했다. |
| [FC0191](fc/FC0191.md) | [의존성·교체 가능성](09-dependency.md) | 사용하지 않는 의존성과 import 정리를 요청했고, 후속 리뷰에서는 HandlerMappers의 java.util.Objects import가 남아 있다고 지적했다. |
| [FC0192](fc/FC0192.md) | [문서·개발·학습 과정](10-workflow.md) | 직접 작성하지 않은 기존 코드의 문제도 프로젝트에 도움이 된다면 드러내고 수정할지 판단하자. |
| [FC0193](fc/FC0193.md) | [문서·개발·학습 과정](10-workflow.md) | 설명한 패키지 이동이 코드에 보이지 않아 관련 커밋이 누락되었는지 확인을 요청했다. |
| [FC0194](fc/FC0194.md) | [문서·개발·학습 과정](10-workflow.md) | 우선 스프링의 다양한 기능을 활용하고, 궁금한 기능이 생기면 코드를 따라가며 학습하는 방식을 제안했다. |
| [FC0195](fc/FC0195.md) | [문서·개발·학습 과정](10-workflow.md) | 이해가 부족한 지점을 확인하기 위해 동료에게 설명하고 토론하며, 같은 미션의 다른 구현을 함께 비교하는 학습을 권했다. |
| [FC0196](fc/FC0196.md) | [문서·개발·학습 과정](10-workflow.md) | 다음 리뷰 요청 때 변경 반영뿐 아니라 설계나 구현을 선택한 이유도 PR 설명에 적어 달라고 요청했다. |
| [FC0197](fc/FC0197.md) | [문서·개발·학습 과정](10-workflow.md) | 가능하다면 다음 리뷰 요청에는 진행한 학습 테스트도 포함해 달라고 제안했다. |
| [FC0198](fc/FC0198.md) | [문서·개발·학습 과정](10-workflow.md) | 서로 관련 없는 변경을 하나의 커밋에 섞지 않고 커밋 메시지가 실제 작업 범위를 드러내도록 하자는 제안이다. |
| [FC0199](fc/FC0199.md) | [문서·개발·학습 과정](10-workflow.md) | README의 기능 요구사항 목록에서 완료한 항목을 체크해 달라고 요청했다. |
| [FC0200](fc/FC0200.md) | [문서·개발·학습 과정](10-workflow.md) | 테스트와 운영 코드 작성에 하나의 정답을 찾기보다 다음 단계에서 우선 구현해 보며 자신의 방식을 찾아가도록 권했다. |
| [FC0201](fc/FC0201.md) | [문서·개발·학습 과정](10-workflow.md) | API 문서화에 Swagger를 선택한 이유와 REST Docs를 대안으로 고려했는지 설명을 요청한다. |
| [FC0202](fc/FC0202.md) | [문서·개발·학습 과정](10-workflow.md) | 구현할 사항을 더 잘 정리할 수 있도록 README의 요구사항을 명확하게 작성하자고 제안했다. |
| [FC0203](fc/FC0203.md) | [도메인 모델·값 표현](11-domain-model.md) | ID만 받고 나머지 필드를 null로 두는 `Member` 생성자가 왜 필요한지 질문하며 어색하다는 의견을 제시했다. |
| [FC0204](fc/FC0204.md) | [도메인 모델·값 표현](11-domain-model.md) | 주문 테이블에 updated_at이 필요한지 확인하고, 수정 가능한 데이터와 수정하지 않는 이력 데이터를 구분해 판단하도록 논의했다. |
| [FC0205](fc/FC0205.md) | [도메인 모델·값 표현](11-domain-model.md) | 복잡한 비즈니스 로직에서 객체 상태 변화로 코드가 복잡해지는 점을 고려하여 도메인 객체를 가능한 한 불변 객체로 만들어 보자는 제안이다. |
| [FC0206](fc/FC0206.md) | [도메인 모델·값 표현](11-domain-model.md) | 도메인과 엔티티를 어떻게 정의하며, Cart에 별도 조건이나 로직이 없다는 이유로 도메인 모델을 두지 않는 판단이 적절한지 논의했다. |
| [FC0207](fc/FC0207.md) | [도메인 모델·값 표현](11-domain-model.md) | 문자열로 지정하는 ContentType을 HttpStatusCode처럼 enum으로 관리하자고 제안했다. |
| [FC0208](fc/FC0208.md) | [도메인 모델·값 표현](11-domain-model.md) | 상품 가격을 int로 표현하는 대신 BigDecimal 사용을 고려하자고 제안했다. |
| [FC0209](fc/FC0209.md) | [도메인 모델·값 표현](11-domain-model.md) | 날짜 정보를 문자열로 취급하는 대신 LocalDate로 표현하는 방식을 제안했다. |
| [FC0210](fc/FC0210.md) | [도메인 모델·값 표현](11-domain-model.md) | Line의 이름과 색상을 변경하는 setter 사용을 지양하는 것이 어떨지 제안했다. |
| [FC0211](fc/FC0211.md) | [도메인 모델·값 표현](11-domain-model.md) | Reservation과 ReservationWaiting이 거의 동일한 도메인인 현재 구조에서, 대기를 예약의 상태로 표현하지 않은 이유를 물었다. |
| [FC0212](fc/FC0212.md) | [도메인 모델·값 표현](11-domain-model.md) | Reservation이 status로 예약과 예약 대기를 표현하는 것을 어색하게 느낀 이유를 묻고, 취소 예약까지 고려해 모델 분리 기준을 검토하도록 제안한다. |
| [FC0213](fc/FC0213.md) | [도메인 모델·값 표현](11-domain-model.md) | HTTP의 method, uri, version은 헤더가 아닌 Request Line에 속하므로 HttpRequestHeader와 다른 객체에서 표현하는 방안을 제안했다. |
| [FC0214](fc/FC0214.md) | [도메인 모델·값 표현](11-domain-model.md) | 타입에 따라 사용하지 않는 값이 생기는 쿠폰 테이블에서, 기본값과 NOT NULL 제약이 값의 부재 가능성을 가려 혼선을 줄 수 있다는 우려다. |
| [FC0215](fc/FC0215.md) | [도메인 검증](12-validation.md) | 예약 저장 시 과거 날짜뿐 아니라 이미 지난 예약 시간도 검증해야 하는지 검토를 요청했다. |
| [FC0216](fc/FC0216.md) | [도메인 검증](12-validation.md) | 요청 데이터 검증 로직이 없는 상태에서 null 저장을 의도한 것인지 질문했다. |
| [FC0217](fc/FC0217.md) | [도메인 검증](12-validation.md) | 요청 객체뿐 아니라 도메인 객체에서도 값을 검증해야 하는지 검토하도록 질문했다. |
| [FC0218](fc/FC0218.md) | [도메인 검증](12-validation.md) | 쿼리 문자열에 키만 있고 값이 없을 때 파싱이 어떻게 동작하는지 확인을 요청했다. |
| [FC0219](fc/FC0219.md) | [도메인 검증](12-validation.md) | 구간의 두 역 이름이 중복되는지 검사하는 유효성 검증을 Section 객체 생성 시 수행하면 어떨지 제안했다. |
| [FC0220](fc/FC0220.md) | [도메인 검증](12-validation.md) | 요청 유효성 검증 방법 중 하나인 @Validated를 추가로 학습해 보자고 제안했다. |
| [FC0221](fc/FC0221.md) | [도메인 검증](12-validation.md) | DTO에서 입력을 검증하더라도 도메인 자체의 검증이 필요하며, Reservation 외 다른 도메인도 확인하자고 요청했다. |
| [FC0222](fc/FC0222.md) | [도메인 검증](12-validation.md) | @NotBlank의 검증 구현이 null도 검사하므로 함께 사용한 @NotNull은 생략할 수 있다는 의견을 제시한다. |
| [FC0223](fc/FC0223.md) | [도메인 검증](12-validation.md) | 생성 시 검증으로 보장할 수 있다면 예약 변경 메서드의 검증이 불필요하지 않은지 논의했다. |
| [FC0224](fc/FC0224.md) | [도메인 검증](12-validation.md) | 입력이 없어 readLine()이 null을 반환하는 경우를 고려해 요청 줄에 대한 null 방어를 추가하자고 제안했다. |
| [FC0225](fc/FC0225.md) | [도메인 검증](12-validation.md) | 나이를 입력하지 않았을 때 0으로 처리되는 구조라면 버그가 발생할 가능성을 제기했다. |
| [FC0226](fc/FC0226.md) | [도메인 검증](12-validation.md) | 예약 생성 시 수행하는 검증을 `updateReservation`에서도 수행해야 하지 않는지 질문했다. |
| [FC0227](fc/FC0227.md) | [도메인 검증](12-validation.md) | 주문 준비 검증에 OrderTable이 empty인 경우에 대한 검증을 추가해 달라고 요청했다. |
| [FC0228](fc/FC0228.md) | [도메인 검증](12-validation.md) | 중복 이름 금지를 DB 유니크 제약 오류에만 맡기기보다 서비스 계층에서 검증하고 예외를 발생시키는 방식을 검토하자고 제안한다. |
| [FC0229](fc/FC0229.md) | [도메인 검증](12-validation.md) | 사용 중이지 않은 테마만 삭제할 수 있다는 규칙에 맞게 테마 삭제 로직을 수정해 달라고 요청했다. |
| [FC0230](fc/FC0230.md) | [도메인 검증](12-validation.md) | 장바구니 수량 변경 요청의 quantity에 음수도 입력될 수 있다는 지적이다. |
| [FC0231](fc/FC0231.md) | [도메인 검증](12-validation.md) | public인 addMenuProduct로 외부에서 상품을 추가할 때 가격 제약조건을 별도로 검증해야 하지 않는지 질문했다. |
| [FC0232](fc/FC0232.md) | [도메인 검증](12-validation.md) | 노선 이름 수정 시 다른 노선의 기존 이름으로 변경하여 중복이 생기는 경우를 검증해야 한다고 지적했다. |
| [FC0233](fc/FC0233.md) | [도메인 검증](12-validation.md) | 이미 존재하는 account로 재가입하면 기존 회원 정보가 덮어써지는 문제를 지적했다. |
| [FC0234](fc/FC0234.md) | [도메인 검증](12-validation.md) | reservation 테이블의 time_id와 theme_id에도 NOT NULL 제약이 필요한지 질문했다. |
| [FC0235](fc/FC0235.md) | [도메인 검증](12-validation.md) | 요청 필드의 빈값과 null 등에 대한 기본 검증을 추가하는 것이 좋지 않은지 질문했다. |
| [FC0236](fc/FC0236.md) | [도메인 검증](12-validation.md) | 발급일을 포함해 7일간 사용할 수 있는 쿠폰이라면 만료일 계산에서 7일이 아니라 6일을 더해야 하는지 확인했다. |
| [FC0237](fc/FC0237.md) | [도메인 검증](12-validation.md) | Email 값에 정규표현식 등을 활용한 간단한 이메일 형식 검증을 추가하도록 제안했다. |
| [FC0238](fc/FC0238.md) | [도메인 검증](12-validation.md) | 문자열 입력이 공백으로만 이루어진 경우도 검증해야 하지 않는지 묻는다. |
| [FC0239](fc/FC0239.md) | [도메인 검증](12-validation.md) | TokenRequest에 Java Bean Validation을 적용해 null 여부 등의 입력 검증을 수행해보자는 제안이다. |
| [FC0240](fc/FC0240.md) | [예외·실패 계약](13-errors.md) | IllegalArgumentException만 처리하는 예외 처리 클래스에서 다른 예외가 발생하면 어떻게 되는지 검토하도록 질문했다. |
| [FC0241](fc/FC0241.md) | [예외·실패 계약](13-errors.md) | 입력 예외가 사용되는 상황에 맞게 예외 메시지도 수정할 필요가 있다고 제안했다. |
| [FC0242](fc/FC0242.md) | [예외·실패 계약](13-errors.md) | SQLException을 그대로 던지지 않고 RuntimeException으로 감싸서 던지는 이유를 설명해 달라고 요청했다. |
| [FC0243](fc/FC0243.md) | [예외·실패 계약](13-errors.md) | 요청 처리 중 잡힌 모든 예외를 Bad Request 응답으로 처리하는지 질문했다. |
| [FC0244](fc/FC0244.md) | [예외·실패 계약](13-errors.md) | 오류 처리에 ResponseErrorHandler를 채택한 이유와 검토한 대안을 질문했다. |
| [FC0245](fc/FC0245.md) | [예외·실패 계약](13-errors.md) | 외부 API에서 예상치 못한 응답이 오면 JSON 파싱이 실패할 수 있으므로 오류 응답 처리에서 이 경우도 방어하도록 제안했다. |
| [FC0246](fc/FC0246.md) | [예외·실패 계약](13-errors.md) | queryForObject의 조회 결과가 없을 때 null을 직접 반환하기보다 Optional로 부재를 표현하거나 예외를 던지는 방안을 제안했다. |
| [FC0247](fc/FC0247.md) | [예외·실패 계약](13-errors.md) | 단건 조회 결과가 없을 때 null을 반환하면 호출자에게 의도하지 않은 NullPointerException이 발생할 수 있으므로 다른 처리 방식을 검토하자고 제안했다. |
| [FC0248](fc/FC0248.md) | [예외·실패 계약](13-errors.md) | 검증 실패 시 고정된 예외 메시지 대신 검증 오류가 가진 메시지를 꺼내 전달하는 방식을 제안했다. |
| [FC0249](fc/FC0249.md) | [예외·실패 계약](13-errors.md) | 예상하지 못한 예외의 원래 메시지를 응답으로 그대로 전달하기보다, 상세 내용은 로그로 확인하고 클라이언트에는 일반적인 오류 메시지를 제공하도록 제안했다. |
| [FC0250](fc/FC0250.md) | [예외·실패 계약](13-errors.md) | 일반 Exception 처리 응답을 500에서 400으로 바꾼 이유와 예상치 못한 서버 오류를 클라이언트의 잘못된 요청으로 응답하는 것이 적절한지 확인한다. |
| [FC0251](fc/FC0251.md) | [예외·실패 계약](13-errors.md) | 예외가 발생했을 때 HTTP 오류 상태를 담은 에러 응답을 내려주는 방식을 제안했다. |
| [FC0252](fc/FC0252.md) | [예외·실패 계약](13-errors.md) | 정적 리소스 요청을 검증하고 올바르지 않은 경우 404를 응답하는 방안을 제안했다. |
| [FC0253](fc/FC0253.md) | [예외·실패 계약](13-errors.md) | 존재하지 않는 예약 시간을 삭제할 때 예외를 낼지는 비즈니스 영향에 따라 판단하되, 현재처럼 삭제된 상태 자체가 목적이면 오류를 내지 않아도 된다는 의견을 제시했다. |
| [FC0255](fc/FC0255.md) | [예외·실패 계약](13-errors.md) | 로그인 실패 시 401.html로 리다이렉트한다는 요구사항 대신 401 응답으로 구현한 이유를 묻는다. |
| [FC0257](fc/FC0257.md) | [프론트엔드 상태](14-frontend-state.md) | 화면에서 사용할 gameId는 숨겨진 태그보다 자바스크립트 변수로 보관하는 편을 제안한다. |
| [FC0258](fc/FC0258.md) | [프론트엔드 상태](14-frontend-state.md) | 매번 GET으로 존재 여부를 확인하는 대신 프론트엔드에서 상품 존재 여부와 수량을 캐싱해 표시하고, 결제 시점에 다시 검증하는 방식을 대안으로 제시했다. |
| [FC0262](fc/FC0262.md) | [로그·관측](15-observability.md) | 현재 로그만으로는 어떤 예외가 발생했는지 확인할 수 없으므로 발생한 오류를 식별할 수 있는 정보를 남기도록 제안했다. |
| [FC0263](fc/FC0263.md) | [로그·관측](15-observability.md) | 로그인 처리 코드에 남아 있는 console.log 콘솔 출력을 지적했다. |
| [FC0264](fc/FC0264.md) | [로그·관측](15-observability.md) | 로그를 남겨야 하는 상황과 목적, 현재 로깅을 적용한 판단 기준을 설명해 달라고 질문했다. |
| [FC0265](fc/FC0265.md) | [성능·측정](16-performance.md) | 성능 관점의 적절한 커넥션 풀 크기는 직접 측정해 판단해야 한다는 의견을 제시한다. |
| [FC0266](fc/FC0266.md) | [성능·측정](16-performance.md) | 저장한 Payment 객체를 그대로 사용해 ID로 다시 조회하는 불필요한 조회를 없애자는 제안이다. |
| [FC0267](fc/FC0267.md) | [성능·측정](16-performance.md) | `Arrays.asList(mappings)`를 세 번 생성하지 말고 한 번 만든 변수를 재사용할 것을 제안했다. |
| [FC0268](fc/FC0268.md) | [성능·측정](16-performance.md) | 질문과 답변을 한 번의 쿼리로 조회해야 하는 실제 성능상 필요가 있는지 확인하고, 조기 최적화로 코드 복잡도를 높이지 않는 방안을 고려하자. |
| [FC0269](fc/FC0269.md) | [성능·측정](16-performance.md) | rowsExpected로 ArrayList의 초기 용량을 설정한 목적이 최적화인지, 그렇다면 어떤 근거로 작성했는지 질문했다. |
| [FC0270](fc/FC0270.md) | [성능·측정](16-performance.md) | 도메인 이벤트를 통한 지연된 검증 전에 비용이 큰 작업이 실행된다면, 뒤늦은 검증 실패로 불필요한 비용이 발생할 수 있다고 우려했다. |
| [FC0271](fc/FC0271.md) | [성능·측정](16-performance.md) | 단순 반복에서 for와 forEach를 선택할 때 가독성과 컬렉션·스트림 생성 비용이 실제 서비스에 미치는 영향을 논의한다. |
| [FC0272](fc/FC0272.md) | [성능·측정](16-performance.md) | 대기 순번 계산의 성능 우려를 구체화하고, 실제 쿼리 실행 계획을 확인한 뒤 데이터베이스 최적화 가능성을 검토하자는 제안이다. |
| [FC0273](fc/FC0273.md) | [성능·측정](16-performance.md) | 요청을 처리할 때마다 컨트롤러 인스턴스를 새로 생성해야 하는지 질문했다. |
| [FC0274](fc/FC0274.md) | [성능·측정](16-performance.md) | 장바구니 항목을 순회하며 상품을 개별 조회하는 쿼리를 한 번의 조회로 줄이는 방식을 제안했다. |
| [FC0275](fc/FC0275.md) | [성능·측정](16-performance.md) | 리다이렉트 응답을 만드는 과정에서 /404.html 파일을 미리 읽어올 필요가 있는지 질문했다. |
| [FC0276](fc/FC0276.md) | [성능·측정](16-performance.md) | 즐겨찾기 조회 과정에서 쿼리가 여러 번 발생하는 비효율을 줄여 최소한의 쿼리로 처리하도록 제안했다. |
| [FC0277](fc/FC0277.md) | [성능·측정](16-performance.md) | 조회 시 캐시 미스로도 캐싱할 수 있는데 생성 시점에도 캐싱하는 전략을 선택한 이유를 질문한다. |
| [FC0278](fc/FC0278.md) | [성능·측정](16-performance.md) | enum을 순회해 값을 찾는 대신 미리 만든 Map으로 조회하는 대안을 소개하고, 메모리 비용을 고려해 필요한 곳에만 적용하는 방향을 논의한다. |
| [FC0279](fc/FC0279.md) | [성능·측정](16-performance.md) | 예약 시간 조회에서 findAll로 모든 예약을 메모리에 올리는 대신 DB에서 필요한 데이터를 필터링하는 방안을 검토하도록 제안했다. |
| [FC0280](fc/FC0280.md) | [성능·측정](16-performance.md) | HandlerExecution 생성자에서 컨트롤러 인스턴스를 받아 매 요청마다 인스턴스를 생성하지 않는 방안에 대한 의견을 물었다. |
| [FC0281](fc/FC0281.md) | [성능·측정](16-performance.md) | 예약 하나를 조회할 때 실행되는 쿼리 수와 불필요한 조회 여부를 확인하고, 추가 조회를 필요한 시점에만 수행하는 방법을 검토하도록 요청했다. |
| [FC0282](fc/FC0282.md) | [성능·측정](16-performance.md) | 요청마다 생성되는 JsonView와 함께 ObjectMapper도 새로 생성하지 말고 재사용하도록 제안했다. |
| [FC0283](fc/FC0283.md) | [성능·측정](16-performance.md) | 핸들러 어댑터 탐색에서 findFirst와 findAny의 차이를 살펴보고 findAny 사용을 고려하도록 제안한다. |
| [FC0284](fc/FC0284.md) | [성능·측정](16-performance.md) | OFFSET 페이지네이션의 동작 방식과 부하 측면의 문제 가능성을 더 검토하도록 질문했다. |
| [FC0285](fc/FC0285.md) | [성능·측정](16-performance.md) | 인덱스 적용 후에도 느리다면 조회 컬럼 수의 영향을 고려해 필요한 컬럼만 가져오는 인라인 뷰로 쿼리를 바꾸는 접근을 제안했다. |
| [FC0286](fc/FC0286.md) | [성능·측정](16-performance.md) | 역마다 개별 조회 쿼리를 실행하는 대신 역들을 한 번에 조회해 처리하여 쿼리 수를 줄이는 방안을 고려하자. |
| [FC0287](fc/FC0287.md) | [성능·측정](16-performance.md) | 반복 처리 중 DB를 조회한다면 데이터를 한 쿼리로 가져온 뒤 처리하여 반복 조회를 줄이도록 제안한다. |
| [FC0289](fc/FC0289.md) | [성능·측정](16-performance.md) | 이메일 검증에 정규식을 사용할 때 주의할 점이 무엇인지 질문했다. |
| [FC0290](fc/FC0290.md) | [성능·측정](16-performance.md) | hasJsessionId()의 키 존재 검사와 getValue() 내부의 containsKey() 검사가 중복된다. |
| [FC0292](fc/FC0292.md) | [성능·측정](16-performance.md) | 역과 노선의 변경이 드물다면 그래프를 매번 구성하는 대신 애플리케이션 시작 시나 첫 경로 조회 시 생성해 재사용하는 방안을 고민해 보자고 제안했다. |
| [FC0293](fc/FC0293.md) | [성능·측정](16-performance.md) | 메뉴 생성 과정에서 요청한 상품 수만큼 개별 조회 쿼리가 실행되는 N+1 가능성을 지적한다. |
| [FC0296](fc/FC0296.md) | [성능·측정](16-performance.md) | MenuProduct 생성 시 이미 조회한 Product를 가격 검증 과정에서 다시 조회할 필요가 있는지 검토해 달라는 질문이다. |
| [FC0297](fc/FC0297.md) | [가독성·명명](17-readability.md) | idMap처럼 자료형을 포함하는 변수명 대신 의미를 더 명확하게 드러내는 이름을 고민하도록 요청했다. |
| [FC0298](fc/FC0298.md) | [가독성·명명](17-readability.md) | verifyLogin이라는 이름만으로 반환하는 값을 예측하기 어려우므로, 반환 동작을 더 직관적으로 드러내는 이름으로 변경하도록 요청한다. |
| [FC0299](fc/FC0299.md) | [가독성·명명](17-readability.md) | 기존 코드에 남아 있는 var 사용도 작성자가 정한 타입 표기 컨벤션에 맞춰 일관되게 정리하자는 제안이다. |
| [FC0300](fc/FC0300.md) | [가독성·명명](17-readability.md) | Answer에서 toString을 제거한 이유를 묻는다. |
| [FC0301](fc/FC0301.md) | [가독성·명명](17-readability.md) | instantiateBean 메서드도 역할 분리 등의 방법으로 가독성을 개선해 보자고 제안했다. |
| [FC0302](fc/FC0302.md) | [가독성·명명](17-readability.md) | findNextStation이 조회뿐 아니라 전달받은 result에 요소를 추가하므로, 실제 동작을 더 잘 드러내는 이름이 있는지 질문했다. |
| [FC0303](fc/FC0303.md) | [가독성·명명](17-readability.md) | 삭제 후 조회 결과가 비어 있음을 검증할 때 hasSize(0) 대신 isEmpty()로 표현할 수도 있다고 제안했다. |
| [FC0304](fc/FC0304.md) | [가독성·명명](17-readability.md) | SQL을 별도 상수로 추출할 필요가 있는지 질문했다. |
| [FC0305](fc/FC0305.md) | [가독성·명명](17-readability.md) | 코드 전반에서 컨벤션에 맞지 않는 부분을 확인해 달라고 요청했다. |
| [FC0306](fc/FC0306.md) | [가독성·명명](17-readability.md) | 반복되는 문자열을 상수로 추출하도록 요청했다. |
| [FC0307](fc/FC0307.md) | [가독성·명명](17-readability.md) | result보다 stations처럼 담고 있는 데이터를 드러내는 변수명이 적합한지 고민하도록 제안한다. |
| [FC0308](fc/FC0308.md) | [가독성·명명](17-readability.md) | 조회 결과를 User 리스트로 변환하는 반복문을 stream과 flatMap을 활용해 더 읽기 쉽게 작성해 보라고 제안한다. |
| [FC0309](fc/FC0309.md) | [가독성·명명](17-readability.md) | 클래스 이름을 명사형으로 표현하도록 CheckAdminInterceptor 대신 AdminCheckInterceptor를 제안했다. |
| [FC0310](fc/FC0310.md) | [가독성·명명](17-readability.md) | registerOrder 메서드가 길어 보이므로 분리할 방법을 검토하자고 제안했다. |
| [FC0311](fc/FC0311.md) | [가독성·명명](17-readability.md) | LoginResult 클래스가 사용되지 않고 있음을 지적했다. |
| [FC0312](fc/FC0312.md) | [가독성·명명](17-readability.md) | ID 비교식의 == 연산자 앞뒤 공백을 맞춰 코드 컨벤션을 지키도록 제안한다. |
| [FC0313](fc/FC0313.md) | [가독성·명명](17-readability.md) | initialize 안에서 RequestMapping이 있는 메서드를 추출하는 부분을 별도 메서드로 분리하자는 제안이다. |
| [FC0314](fc/FC0314.md) | [가독성·명명](17-readability.md) | 사용하지 않는 코드를 삭제하도록 요청했다. |
| [FC0315](fc/FC0315.md) | [가독성·명명](17-readability.md) | Authorization 헤더명을 문자열로 쓰는 대신 HttpHeaders.AUTHORIZATION 상수를 활용하자고 제안했다. |
| [FC0316](fc/FC0316.md) | [가독성·명명](17-readability.md) | 멀티 모듈 구조가 복잡하게 느껴지는 이유가 도메인 모듈 아래에 추가된 한 단계의 깊이 때문인지 살펴본다. |
| [FC0317](fc/FC0317.md) | [가독성·명명](17-readability.md) | 사용하지 않는 import 문을 제거하고 패키지 최상단에서 일괄 정리하는 방법을 활용하라고 제안했다. |
| [FC0318](fc/FC0318.md) | [가독성·명명](17-readability.md) | 사용하지 않는 주석 처리된 코드를 삭제하도록 요청했다. |
| [FC0319](fc/FC0319.md) | [가독성·명명](17-readability.md) | 겹치는 역이 있는지 찾는 동작이 드러나도록 haveStation보다 적절한 메서드 이름을 검토해 보라고 제안했다. |
| [FC0320](fc/FC0320.md) | [가독성·명명](17-readability.md) | 주문 조회 테스트의 주문 번호에 매직 넘버를 피하면 의미가 더 명시적으로 드러날 것이라고 제안했다. |
| [FC0321](fc/FC0321.md) | [가독성·명명](17-readability.md) | @GetMapping("")의 빈 문자열 인자를 생략해 @GetMapping으로 간결하게 표현하도록 제안했다. |
| [FC0322](fc/FC0322.md) | [가독성·명명](17-readability.md) | 검증 대상을 알 수 있도록 verifyRequest를 더 의미 있는 메서드 이름으로 바꾸자고 제안했다. |
| [FC0323](fc/FC0323.md) | [가독성·명명](17-readability.md) | findVerifiedStationByName이라는 메서드 이름에 어떤 의도를 담았는지 질문했다. |
| [FC0324](fc/FC0324.md) | [가독성·명명](17-readability.md) | 컨트롤러만 검증하는 테스트로 오해하지 않도록 테스트 클래스와 패키지 이름이 실제 통합 테스트 범위를 드러내는지 검토하자고 제안했다. |
| [FC0325](fc/FC0325.md) | [가독성·명명](17-readability.md) | 다른 변수 선언과의 일관성을 위해 resource 변수에도 final을 붙이는 것을 제안했다. |
| [FC0326](fc/FC0326.md) | [가독성·명명](17-readability.md) | 테스트 코드에서 연속된 빈 줄 대신 빈 줄을 하나씩만 사용하도록 요청했다. |
| [FC0327](fc/FC0327.md) | [가독성·명명](17-readability.md) | 예약 조회 컨트롤러 메서드 이름을 getReservations처럼 동작이 명확하게 드러나도록 바꾸자는 제안이다. |
| [FC0328](fc/FC0328.md) | [가독성·명명](17-readability.md) | 파일 끝에 개행을 추가하는 코드 형식에 주의하도록 제안했다. |
| [FC0329](fc/FC0329.md) | [가독성·명명](17-readability.md) | 테스트 이름을 단순한 단계 번호가 아니라 어떤 내용을 검증하는지 드러나도록 작성하자는 제안이다. |
| [FC0330](fc/FC0330.md) | [가독성·명명](17-readability.md) | SQL 문자열 변수 선언에서 var와 String을 혼용하는 기준이 있는지 물었다. |
| [FC0331](fc/FC0331.md) | [가독성·명명](17-readability.md) | GET 요청이라는 이유로 조회 메서드를 모두 read로 명명하기보다 조회 대상과 역할을 드러내는 이름을 사용하자는 제안이다. |
| [FC0332](fc/FC0332.md) | [가독성·명명](17-readability.md) | validate라는 이름만으로는 검증 대상을 알기 어려우므로 무엇을 검증하는 메서드인지 드러내자고 제안했다. |
| [FC0333](fc/FC0333.md) | [가독성·명명](17-readability.md) | Cart의 컬렉션 필드 이름을 value보다 내용이 명확한 cartItems로 표현하는 것을 제안했다. |
| [FC0334](fc/FC0334.md) | [가독성·명명](17-readability.md) | ConsoleController와 WebController의 이름에 어떤 기능을 담당하는 컨트롤러인지 더 명확히 드러내도록 제안했다. |
| [FC0335](fc/FC0335.md) | [가독성·명명](17-readability.md) | 해당 메서드가 사용되지 않는 것 같다고 지적했다. |
| [FC0336](fc/FC0336.md) | [가독성·명명](17-readability.md) | HandlerExecution의 declaredObject 필드를 역할이 더 명시적인 handler로 명명하는 방안을 제안한다. |
| [FC0337](fc/FC0337.md) | [가독성·명명](17-readability.md) | 요청용 DTO라면 Request를 이름에 포함하고, 필요하면 생성 등 구체적인 용도도 드러내도록 명명하자고 제안했다. |
| [FC0338](fc/FC0338.md) | [가독성·명명](17-readability.md) | 미션에서 요구하는 Google Java Style Guide에 맞춰 wildcard import를 피하고 명시적인 import를 사용한다. |
| [FC0339](fc/FC0339.md) | [가독성·명명](17-readability.md) | 템플릿 이름의 html 확장자 표기에 대해, 템플릿 리졸버가 접미사를 붙이므로 명시하지 않아도 된다는 의견을 제시했다. |
| [FC0340](fc/FC0340.md) | [가독성·명명](17-readability.md) | 사용자 정보를 처리하는 코드의 중첩 깊이가 2 이상이므로 줄여 보자고 제안했다. |
| [FC0341](fc/FC0341.md) | [가독성·명명](17-readability.md) | 실행과 예외 검증을 함께 하는 테스트 구간의 주석을 `when, then`으로 표시하자고 제안했다. |
| [FC0342](fc/FC0342.md) | [가독성·명명](17-readability.md) | 호출부가 서로 다른 색상인지 확인하려는 용도이므로 isSameColor를 isNotSameColor 형태로 바꾸자고 제안한다. |
| [FC0343](fc/FC0343.md) | [가독성·명명](17-readability.md) | 각 테스트에 @DisplayName을 추가해 테스트 설명을 명시하자는 제안이다. |
| [FC0344](fc/FC0344.md) | [렌더링·데이터 로딩](18-rendering.md) | 현재 render 메서드로 View를 처리하는 방식과 스프링의 View 처리 방식에 어떤 차이가 있는지 묻는다. |
| [FC0345](fc/FC0345.md) | [렌더링·데이터 로딩](18-rendering.md) | 반환하는 템플릿 이름을 index가 아닌 /index로 지정한 이유를 묻는다. |
| [FC0346](fc/FC0346.md) | [렌더링·데이터 로딩](18-rendering.md) | 뷰 렌더링에서 응답이 아닌 요청에 속성을 설정하는 이유와 RequestDispatcher 및 forward의 역할을 알아보자고 제안한다. |
| [FC0347](fc/FC0347.md) | [렌더링·데이터 로딩](18-rendering.md) | 브라우저가 index.html을 처음 받은 뒤 HTML에 연결된 CSS와 JS를 어떤 과정으로 추가 요청하는지 묻는다. |
| [FC0348](fc/FC0348.md) | [렌더링·데이터 로딩](18-rendering.md) | 직접 render()를 호출하는 대신 Spring Boot의 Handlebars 지원 기능으로 뷰를 반환하는 방식을 제안한다. |
| [FC0349](fc/FC0349.md) | [렌더링·데이터 로딩](18-rendering.md) | SSR과 CSR을 비교하며 @Controller와 @RestController의 차이, 사용 시점과 뷰가 그려지는 위치를 정리해 보도록 제안한다. |
| [FC0352](fc/FC0352.md) | [렌더링·데이터 로딩](18-rendering.md) | Spring Boot의 Handlebars 지원을 활용해 템플릿 확장자를 html에서 hbs로 바꾸고 파일명을 반환하는 뷰 처리 방식을 안내한다. |
| [FC0353](fc/FC0353.md) | [렌더링·데이터 로딩](18-rendering.md) | Model을 사용하는 응답 방식과 JSON 데이터를 반환하는 방식의 차이를 고민하고 JSON 응답도 고려해 보도록 제안했다. |
| [FC0354](fc/FC0354.md) | [렌더링·데이터 로딩](18-rendering.md) | 방 목록 렌더링에서 각 자식에 고유한 key prop이 필요하다는 경고를 확인하고 수정해 달라는 요청이다. |
| [FC0356](fc/FC0356.md) | [책임·계층 경계](19-responsibility.md) | 컨트롤러 메서드를 가져오는 단계에서 RequestMapping 어노테이션으로 필터링하지 않고 모든 메서드를 가져온 이유를 질문했다. |
| [FC0357](fc/FC0357.md) | [책임·계층 경계](19-responsibility.md) | 요청에서 User를 추출하는 행위와 User를 저장하는 행위를 분리하자고 제안했다. |
| [FC0358](fc/FC0358.md) | [책임·계층 경계](19-responsibility.md) | cart 문자열만 조회하는 대신 Member를 조회해 MemberEntity로 변환하고, 관련 변환 로직을 MemberEntity에 둘 수도 있다고 제안했다. |
| [FC0359](fc/FC0359.md) | [책임·계층 경계](19-responsibility.md) | HttpResponse가 응답 값을 표현하는 것 외에 요청에 맞는 Controller를 찾고 실행하는 책임까지 가져야 하는지 검토한다. |
| [FC0360](fc/FC0360.md) | [책임·계층 경계](19-responsibility.md) | 컨트롤러를 한 번 생성해 재사용하려는 목적이라면 LoginController 자체를 싱글톤으로 구현하는 방안을 논의했다. |
| [FC0361](fc/FC0361.md) | [책임·계층 경계](19-responsibility.md) | LineStationController가 너무 많은 로직을 책임지고 있으므로 비즈니스 로직을 서비스에서 처리하도록 제안했다. |
| [FC0362](fc/FC0362.md) | [책임·계층 경계](19-responsibility.md) | 도메인 객체가 응답 역할까지 과도하게 담당하는지 검토하고 응답 객체 분리를 고려하자. |
| [FC0363](fc/FC0363.md) | [책임·계층 경계](19-responsibility.md) | 컨트롤러에서 도메인과 DTO를 변환하는 대신 서비스가 요청 DTO를 받고 응답 DTO를 반환하는 구조를 검토한다. |
| [FC0364](fc/FC0364.md) | [책임·계층 경계](19-responsibility.md) | 요청 메서드 값을 외부에서 직접 비교하기보다 RequestMethod 객체에 isGet() 메시지를 보내 판단하도록 제안했다. |
| [FC0365](fc/FC0365.md) | [책임·계층 경계](19-responsibility.md) | 도메인 패키지에 여러 개념이 섞이지 않도록 필요해지면 domain.line 같은 개념별 하위 패키지로 분리하자고 제안했다. |
| [FC0366](fc/FC0366.md) | [책임·계층 경계](19-responsibility.md) | RequestMapping 클래스를 controller 패키지에 배치한 특별한 이유가 있는지 질문했다. |
| [FC0367](fc/FC0367.md) | [책임·계층 경계](19-responsibility.md) | HttpRequest가 요청 파싱, 로직 처리, 응답 생성까지 담당하므로 책임을 분리하는 것이 좋겠다는 의견을 제시한다. |
| [FC0368](fc/FC0368.md) | [책임·계층 경계](19-responsibility.md) | 발급을 돕는 CouponIssuer가 쿠폰 한 건에 종속되는 현재 구조 대신, 미리 생성한 발급기를 활용할 수 있는 협력 관계를 고민하도록 제안했다. |
| [FC0369](fc/FC0369.md) | [책임·계층 경계](19-responsibility.md) | 서비스가 예약의 날짜와 시간을 꺼내 과거 예약인지 계산하기보다 Reservation 객체에 판단을 요청하자는 제안이다. |
| [FC0370](fc/FC0370.md) | [책임·계층 경계](19-responsibility.md) | Service 계층의 역할을 정리하고, 현재 구현에서 계층 분리가 필요한지와 미리 분리하는 방식의 장단점을 검토하도록 요청했다. |
| [FC0371](fc/FC0371.md) | [책임·계층 경계](19-responsibility.md) | 서비스 코드에 데이터 액세스 관련 코드가 남아 있으므로 컴포넌트의 위치와 책임을 고려해 분리하도록 제안했다. |
| [FC0372](fc/FC0372.md) | [책임·계층 경계](19-responsibility.md) | Adapter에서 ModelAndView를 얻은 뒤 렌더링은 별도로 수행하는 구조를 확인했다. |
| [FC0373](fc/FC0373.md) | [책임·계층 경계](19-responsibility.md) | 복잡한 조회 로직 때문에 fakeRepository 구현이 어렵다면 Repository의 책임이 많은지 살펴보고 관련 로직을 Service로 옮기는 방안을 제안했다. |
| [FC0374](fc/FC0374.md) | [책임·계층 경계](19-responsibility.md) | Request DTO를 Controller 패키지가 아니라 Service 패키지에 둔 이유와 계층별 DTO 분리 방식을 논의했다. |
| [FC0375](fc/FC0375.md) | [책임·계층 경계](19-responsibility.md) | 도메인 객체가 DAO에 직접 접근해야 하는 이유를 검토하고, 도메인은 판단 결과를 반환하며 서비스가 DAO를 통해 저장하는 역할 분담을 고려하자. |
| [FC0376](fc/FC0376.md) | [책임·계층 경계](19-responsibility.md) | 화면 안내 문구를 action으로 내려주면 UI 문구 변경 때 백엔드와 API 계약도 함께 변경해야 하는 결합이 생길 수 있다. |
| [FC0377](fc/FC0377.md) | [책임·계층 경계](19-responsibility.md) | HandlerMapping과 HandlerAdapter 각각의 역할과, 두 역할을 하나로 합치지 않고 분리한 이유를 설명해 달라고 요청했다. |
| [FC0378](fc/FC0378.md) | [책임·계층 경계](19-responsibility.md) | PathService에서 역을 조회할 때 LineService를 경유하기보다 해당 역할을 맡은 StationService를 활용하자는 제안이다. |
| [FC0379](fc/FC0379.md) | [책임·계층 경계](19-responsibility.md) | 서비스가 컨트롤러와 소통할 때 도메인 객체를 그대로 노출하면 어떤 문제가 생길 수 있는지 질문했다. |
| [FC0380](fc/FC0380.md) | [책임·계층 경계](19-responsibility.md) | 서비스 등에 남아 있는 로직을 도메인 객체에 더 위임할 수 있는지 검토하자는 제안이다. |
| [FC0381](fc/FC0381.md) | [책임·계층 경계](19-responsibility.md) | 조회 결과를 리스트로 반환하는 로직과 executeUpdate 실행 로직이 한 메서드에 있으므로 두 역할을 분리하는 방안을 제안했다. |
| [FC0382](fc/FC0382.md) | [책임·계층 경계](19-responsibility.md) | 컨트롤러가 단일 책임을 지키도록 예외 처리를 분리하고 ControllerAdvice 계열의 활용을 검토하도록 제안한다. |
| [FC0383](fc/FC0383.md) | [책임·계층 경계](19-responsibility.md) | DispatcherServlet과 DispatcherServletInitializer를 app 패키지에 둔 이유를 묻고 mvc 패키지로의 이동을 검토하자고 제안했다. |
| [FC0384](fc/FC0384.md) | [책임·계층 경계](19-responsibility.md) | DAO에 @Repository를 사용한 이유를 묻고 DAO와 Repository의 역할 차이를 논의했다. |
| [FC0385](fc/FC0385.md) | [책임·계층 경계](19-responsibility.md) | 트랜잭션 사용 여부에 따른 커넥션 상태 확인과 처리를 JdbcTemplate이 아닌 DataSourceUtils에 둔 이유를 묻는다. |
| [FC0386](fc/FC0386.md) | [책임·계층 경계](19-responsibility.md) | OrderService의 사용 중이지 않은 테이블에 대한 주문 검증을 Order 생성 시 도메인에서 수행하도록 옮길 것을 제안했다. |
| [FC0387](fc/FC0387.md) | [인증·보안·비밀값](20-security.md) | 응답에서 노출되면 안 되는 정보가 노출되며 실제 서비스에서는 심각한 보안 문제가 될 수 있다고 지적했다. |
| [FC0388](fc/FC0388.md) | [인증·보안·비밀값](20-security.md) | API를 추가할 때마다 로그인 필요 여부를 설정에 수동으로 반영하다가 누락하지 않도록 인증 대상 경로 관리 방식을 개선해보자는 제안이다. |
| [FC0389](fc/FC0389.md) | [인증·보안·비밀값](20-security.md) | 비밀번호와 개인정보를 DB에 평문으로 저장하는 것이 문제이므로 서버에서 저장 전 암호화하는 방식을 고려해야 한다는 의견이다. |
| [FC0390](fc/FC0390.md) | [인증·보안·비밀값](20-security.md) | 토큰에 담긴 생성 시점의 정보만으로 인증하지 말고 인증 시점에도 올바른 접근인지 확인하는 방식을 제안했다. |
| [FC0391](fc/FC0391.md) | [인증·보안·비밀값](20-security.md) | JSESSIONID가 없는 모든 요청이 아니라 로그인 성공 시에만 세션 쿠키를 발급하도록 한 판단 기준을 논의했다. |
| [FC0392](fc/FC0392.md) | [인증·보안·비밀값](20-security.md) | MemberArgumentResolver의 구현이 인증인지 인가인지, 또는 둘 다인지 질문했다. |
| [FC0393](fc/FC0393.md) | [테스트 대상·검증](21-test-behavior.md) | 저장한 User와 ID로 다시 조회한 객체의 동일성을 확인하는 테스트인지, 해당 검증의 의도가 무엇인지 설명을 요청했다. |
| [FC0394](fc/FC0394.md) | [테스트 대상·검증](21-test-behavior.md) | 테스트 코드 추가를 검토하는 것을 제안했다. |
| [FC0395](fc/FC0395.md) | [테스트 대상·검증](21-test-behavior.md) | 테스트 개수보다는 조건에 따라 동작이 달라지는 부분과 실패가 이후 처리에 영향을 주는 부분을 우선 검증하자고 제안했다. |
| [FC0396](fc/FC0396.md) | [테스트 대상·검증](21-test-behavior.md) | Line이 의도한 대로 동작하는지 확인할 테스트를 더 추가하자는 제안이다. |
| [FC0397](fc/FC0397.md) | [테스트 대상·검증](21-test-behavior.md) | 테스트가 거의 없는 것으로 보이는데 구현하지 않은 이유가 있는지 질문했다. |
| [FC0398](fc/FC0398.md) | [테스트 대상·검증](21-test-behavior.md) | 동작이 아니라 구현사항을 확인하는 것으로 보이는 테스트가 왜 필요한지 질문했다. |
| [FC0399](fc/FC0399.md) | [테스트 대상·검증](21-test-behavior.md) | 로직을 검증하는 테스트가 없으므로 테스트를 추가하면 좋겠다고 제안했다. |
| [FC0400](fc/FC0400.md) | [테스트 대상·검증](21-test-behavior.md) | 정적 리소스 핸들러 테스트에서 CSS와 자바스크립트 파일 처리도 검증하면 좋겠다. |
| [FC0401](fc/FC0401.md) | [테스트 대상·검증](21-test-behavior.md) | 노선 목록 조회 테스트에서 응답 본문의 id뿐 아니라 다른 필드 값도 검증하자는 제안이다. |
| [FC0402](fc/FC0402.md) | [테스트 대상·검증](21-test-behavior.md) | JSON 응답 전체 문자열을 비교하기보다 jsonPath 등을 이용해 테스트 대상인 부분만 검증하자고 제안했다. |
| [FC0403](fc/FC0403.md) | [테스트 대상·검증](21-test-behavior.md) | 모든 컨트롤러와 서비스에 통합·슬라이스 테스트를 각각 작성하는 이유와 검증 범위 차이를 묻고, 현재 상황에서는 통합 테스트만 구현하는 방안을 제안했다. |
| [FC0404](fc/FC0404.md) | [테스트 대상·검증](21-test-behavior.md) | 일부 테스트가 실패하고 있다고 보고하며 확인을 요청했다. |
| [FC0405](fc/FC0405.md) | [테스트 대상·검증](21-test-behavior.md) | 해당 컨트롤러 테스트가 무엇을 검증하며 현재도 필요한 테스트인지 묻는다. |
| [FC0406](fc/FC0406.md) | [테스트 대상·검증](21-test-behavior.md) | 서비스 테스트에서 검증하려는 범위를 먼저 명확히 하고, 다른 서비스를 실제로 사용할지 Mock으로 대체할지 결정하자고 제안한다. |
| [FC0407](fc/FC0407.md) | [테스트 대상·검증](21-test-behavior.md) | 의도한 이유로 예외가 발생했는지 확인하도록 테스트에서도 예외 메시지를 검증하자고 제안했다. |
| [FC0408](fc/FC0408.md) | [테스트 대상·검증](21-test-behavior.md) | HttpMethodTest가 호출하는 API가 없어 테스트가 실패한다고 보고하고 확인을 요청했다. |
| [FC0409](fc/FC0409.md) | [테스트 대상·검증](21-test-behavior.md) | 현재 서비스 테스트가 없으며, 다른 리뷰를 반영하면 서비스에서 검증할 대상이 생길 수 있다고 제안한다. |
| [FC0410](fc/FC0410.md) | [테스트 대상·검증](21-test-behavior.md) | 예약 대기를 예약으로 전환할 때 잘못된 객체의 정보를 사용하는 문제가 맞다면 이를 검증하는 테스트를 추가하자고 제안했다. |
| [FC0411](fc/FC0411.md) | [테스트 대상·검증](21-test-behavior.md) | ReservationServiceTest의 테스트가 실패한다고 보고한다. |
| [FC0412](fc/FC0412.md) | [테스트 대상·검증](21-test-behavior.md) | 현재 테스트가 실패하고 있으므로 수정한 뒤 다시 리뷰를 요청해 달라고 요구했다. |
| [FC0413](fc/FC0413.md) | [테스트 대상·검증](21-test-behavior.md) | 인수 테스트에 비해 도메인 클래스 테스트가 부족해 보이므로 도메인 단위 테스트를 추가하자는 제안이다. |
| [FC0414](fc/FC0414.md) | [테스트 대상·검증](21-test-behavior.md) | 실제 DAO를 사용하는 서비스 테스트가 통과해도 DAO 자체의 동작을 충분히 검증했다고 볼 수 없으므로 계층별 단위 테스트가 필요하다는 의견이다. |
| [FC0415](fc/FC0415.md) | [테스트 대상·검증](21-test-behavior.md) | RequestMethod를 지정하지 않았을 때 모든 HTTP 메서드를 지원하는지 검증하는 테스트를 추가하자는 제안이다. |
| [FC0416](fc/FC0416.md) | [테스트 대상·검증](21-test-behavior.md) | 각 메서드를 한 가지 상황으로만 테스트하는 것으로 보이는데, 다른 상황도 테스트할 필요가 없는지 질문했다. |
| [FC0417](fc/FC0417.md) | [테스트 대상·검증](21-test-behavior.md) | 서비스 테스트에서 Fake Repository가 중요한 DB 접근 동작을 가려 의미 있는 검증이 부족하다고 지적하고 실제 Repository를 사용하는 통합 테스트를 제안했다. |
| [FC0418](fc/FC0418.md) | [테스트 대상·검증](21-test-behavior.md) | JdbcTemplateTest를 작성해 JdbcTemplate의 동작을 검증해보자는 제안이다. |
| [FC0419](fc/FC0419.md) | [테스트 대상·검증](21-test-behavior.md) | 여러 검증이 나열된 테스트에서 assertAll 같은 방식을 활용하자고 제안했다. |
| [FC0420](fc/FC0420.md) | [테스트 대상·검증](21-test-behavior.md) | 주문에 지정된 주문 테이블을 찾을 수 없을 때 예외가 발생하는 경우도 테스트하자는 제안이다. |
| [FC0421](fc/FC0421.md) | [테스트 준비·격리](22-test-isolation.md) | 해당 테스트 설정을 인수 테스트에서만 사용하는 이유를 질문했다. |
| [FC0422](fc/FC0422.md) | [테스트 준비·격리](22-test-isolation.md) | 테스트 데이터 때문에 단건 조회 결과가 여러 개 나오는 문제는 테스트 코드를 수정하는 방향으로 해결하도록 제안했다. |
| [FC0423](fc/FC0423.md) | [테스트 준비·격리](22-test-isolation.md) | 테스트에서만 사용하는 생성자 대신 이미 마련된 정적 팩토리 메서드로 테스트 객체를 생성하는 것을 제안한다. |
| [FC0424](fc/FC0424.md) | [테스트 준비·격리](22-test-isolation.md) | 생성한 데이터를 지울 수 없어 테스트 사이에 의존이 생긴다는 문제에 대해 @Sql로 테스트별 필요한 SQL을 실행하는 방안을 제안한다. |
| [FC0425](fc/FC0425.md) | [테스트 준비·격리](22-test-isolation.md) | 테스트 코드가 전반적으로 동작하지 않는 것 같다며 작성자 환경에서는 정상적으로 실행되는지 확인을 요청했다. |
| [FC0426](fc/FC0426.md) | [테스트 준비·격리](22-test-isolation.md) | 현재 사용하는 데이터가 테스트용 데이터가 아니라는 점을 들어 다음 단계에서 테스트 데이터 구성을 변경해 보자고 제안했다. |
| [FC0427](fc/FC0427.md) | [테스트 준비·격리](22-test-isolation.md) | Mock 사용의 장단점을 인정하면서 Mocking 연습은 유지하되, 서비스 테스트 중 하나는 Mock 없이 작성해보도록 제안한다. |
| [FC0428](fc/FC0428.md) | [테스트 준비·격리](22-test-isolation.md) | DB 테스트 격리와 초기 데이터 구성 방식들의 장단점을 학습한 뒤 상황에 맞게 선택하자는 제안이다. |
| [FC0429](fc/FC0429.md) | [테스트 준비·격리](22-test-isolation.md) | 테스트 설정을 위해 별도 프로필이 필요한지, 테스트 모듈의 properties만으로 해결할 수 없는지 검토한다. |
| [FC0430](fc/FC0430.md) | [테스트 준비·격리](22-test-isolation.md) | JDBC 저장소 테스트에서 @SpringBootTest 대신 @JdbcTest 사용을 고려했는지 질문했다. |
| [FC0432](fc/FC0432.md) | [테스트 준비·격리](22-test-isolation.md) | 삭제 테스트에서 `/times/1`처럼 ID를 직접 지정하지 말고 삽입된 데이터의 ID를 받아 사용하도록 제안했다. |
| [FC0433](fc/FC0433.md) | [테스트 준비·격리](22-test-isolation.md) | 평소 Mockito 등의 모킹을 테스트에 사용하는지, 이번 TransactionManager 테스트에서 모킹을 선택한 이유는 무엇인지 질문했다. |
| [FC0434](fc/FC0434.md) | [테스트 준비·격리](22-test-isolation.md) | 테스트 수행 전마다 동일한 테이블을 새로 생성하기보다 테스트 전용 truncate SQL로 데이터를 초기화하는 방식을 제안했다. |
| [FC0435](fc/FC0435.md) | [테스트 준비·격리](22-test-isolation.md) | 다른 테스트와 유사하게 @BeforeEach를 사용하지 않고 준비 코드를 별도 메서드로 분리한 판단 과정을 묻는다. |
| [FC0437](fc/FC0437.md) | [테스트 준비·격리](22-test-isolation.md) | 타임아웃 동작을 확인하고 싶다면 가상 웹 서버로 지연 응답을 만들고, 자동화가 어렵다면 실제 Mock 서버를 띄워 인수테스트하는 방법을 제안했다. |
| [FC0438](fc/FC0438.md) | [테스트 준비·격리](22-test-isolation.md) | 테스트에서 비슷한 객체를 반복 생성하는 대신 Test Fixture를 만들어 재사용하자는 제안이다. |
| [FC0439](fc/FC0439.md) | [테스트 준비·격리](22-test-isolation.md) | 전체 테스트 실행 시 실패가 발생한다고 보고하고 그 원인을 살펴보도록 요청했다. |
| [FC0440](fc/FC0440.md) | [테스트 준비·격리](22-test-isolation.md) | CURRENT_DATE 기준으로 최근 7일을 조회하는 테스트에 고정된 예약 날짜를 사용하면 시간이 지나 실패하므로, 시간 기준과 테스트 데이터 설정 방식을 검토하도록 요청했다. |
| [FC0441](fc/FC0441.md) | [테스트 준비·격리](22-test-isolation.md) | 테스트 전용 생성자를 추가하기보다 객체 생성이 번거로운 경우 픽스처를 활용하는 방안을 제안했다. |
| [FC0442](fc/FC0442.md) | [테스트 준비·격리](22-test-isolation.md) | given().willReturn으로 반환값을 설정하기 전에 orderTable의 setEmpty를 호출하는 편이 더 자연스럽다고 제안했다. |
| [FC0443](fc/FC0443.md) | [테스트 준비·격리](22-test-isolation.md) | 애플리케이션을 실행한 상태에서도 테스트를 실행할 수 있는지 확인하도록 질문했다. |
| [FC0447](fc/FC0447.md) | [테스트 준비·격리](22-test-isolation.md) | 인수 테스트의 요청 본문을 Map 대신 LineRequest 객체로 구성할 수 있다고 제안했다. |
| [FC0448](fc/FC0448.md) | [테스트 준비·격리](22-test-isolation.md) | 해당 테스트뿐 아니라 다른 테스트의 데이터 준비에도 Repository를 사용하도록 함께 정리할 것을 제안한다. |
| [FC0449](fc/FC0449.md) | [테스트 준비·격리](22-test-isolation.md) | 외부 API의 실제 동작을 확인하면서도 반복 실행 테스트가 외부 서버 상태나 호출 제한에 좌우되지 않도록 테스트 실행 방식을 고민하자는 논의다. |
| [FC0450](fc/FC0450.md) | [트랜잭션·자원 수명](23-transaction.md) | @Transactional의 동작과 다른 서비스 메서드에도 트랜잭션을 적용할 필요가 있는지 검토해 달라는 질문이다. |
| [FC0451](fc/FC0451.md) | [트랜잭션·자원 수명](23-transaction.md) | DataSourceUtils.releaseConnection에서 connection.getAutoCommit()이 true일 때만 커넥션을 닫도록 한 이유를 질문했다. |
| [FC0452](fc/FC0452.md) | [트랜잭션·자원 수명](23-transaction.md) | try-with-resources 밖에서 생성한 ResultSet을 수동으로 닫아야 하는지 확인을 요청했다. |
| [FC0453](fc/FC0453.md) | [트랜잭션·자원 수명](23-transaction.md) | 읽기 DB 조회 실패 후 쓰기 DB를 조회하는 경로에서 의도한 트랜잭션이 동작하는지와 그 원인을 확인해 달라고 요청했다. |
| [FC0455](fc/FC0455.md) | [타입·타입 테스트](24-type-safety.md) | 배열을 스트림으로 변환할 때 Stream.of와 Arrays.stream 중 무엇을 선택할지, 입력 타입 변경을 감지할 수 있는지를 고려해 논의한다. |
| [FC0456](fc/FC0456.md) | [타입·타입 테스트](24-type-safety.md) | basePackage의 타입을 Object 대신 String으로 제한하여 타입 오류를 컴파일 시점에 확인하는 방안에 대한 의견을 물었다. |
| [FC0457](fc/FC0457.md) | [타입·타입 테스트](24-type-safety.md) | DTO와 PathVariable에서 기본형 타입을 사용하는 이유를 질문했다. |
| [FC0458](fc/FC0458.md) | [타입·타입 테스트](24-type-safety.md) | CouponType의 할인액은 int인데 CouponTypeEntity에서는 Integer로 설정한 이유를 질문했다. |
| [FC0459](fc/FC0459.md) | [타입·타입 테스트](24-type-safety.md) | 삭제 요청의 값은 null로 들어오지 않을 것으로 보이므로 nullable 타입의 필요성을 재검토하는 의견이다. |
| [FC0462](fc/FC0462.md) | [타입·타입 테스트](24-type-safety.md) | 포트 번호가 정수만 허용한다면 run이 문자열을 받아 변환하기보다 정수 타입으로 받는 방안을 제안했다. |
| [FC0464](fc/FC0464.md) | [타입·타입 테스트](24-type-safety.md) | ID 타입으로 Long 대신 long을 선택한 이유와 null 허용 조건을 확인했다. |
| [FC0465](fc/FC0465.md) | [타입·타입 테스트](24-type-safety.md) | TxExecutor에 @FunctionalInterface 어노테이션을 붙이자고 제안했다. |
| [FC0467](fc/FC0467.md) | [UI 동작·사용성](25-ui-behavior.md) | 방 이름 입력을 취소하면 null 이름의 방이 생성되므로, 입력하지 않은 경우 방이 생성되지 않도록 하자. |
| [FC0468](fc/FC0468.md) | [UI 동작·사용성](25-ui-behavior.md) | 오류 메시지가 실패 이유뿐 아니라 사용자가 다음에 어떻게 행동해야 하는지도 안내하는지 검토하도록 제안했다. |
| [FC0469](fc/FC0469.md) | [UI 동작·사용성](25-ui-behavior.md) | 이미지 처리에서 불필요한 404를 보내지 않는 방향을 고려하며, 현재의 기본 이미지 표시 방식도 적절한 선택으로 볼 수 있다. |
| [FC0470](fc/FC0470.md) | [UI 동작·사용성](25-ui-behavior.md) | 킹을 잡아 게임이 종료되었을 때 추가 제출 없이 종료 여부와 우승자를 안내하도록 개선하자는 제안이다. |
| [FC0471](fc/FC0471.md) | [UI 동작·사용성](25-ui-behavior.md) | ID가 없는 ProductDto로도 화면이 정상적으로 표시되는지 확인한다. |
| [FC0472](fc/FC0472.md) | [UI 동작·사용성](25-ui-behavior.md) | 콘솔에서도 웹과 동일하게 우승자와 최종 이동거리를 출력하라는 요구가 이동거리를 숫자로 표시하라는 의미인지 논의한다. |
| [FC0473](fc/FC0473.md) | [UI 동작·사용성](25-ui-behavior.md) | 상품 조회 실패 메시지에서 사용자에게 id라는 내부 용어를 알릴 필요가 있는지 묻는다. |
| [FC0476](fc/FC0476.md) | [UI 동작·사용성](25-ui-behavior.md) | 로그인 페이지에 연결된 링크로 이동하면 회원가입 페이지가 보이지 않는 문제를 보고하고 확인을 요청했다. |
| [FC0477](fc/FC0477.md) | [UI 동작·사용성](25-ui-behavior.md) | 예약이 걸려 있지 않은 시간 슬롯을 삭제하려 해도 오류가 발생한다고 보고했다. |
| [FC0478](fc/FC0478.md) | [UI 동작·사용성](25-ui-behavior.md) | 404.html에서 이미지가 깨져 보이는 문제를 보고하고 수정을 요청했다. |
| [FC0479](fc/FC0479.md) | [UI 동작·사용성](25-ui-behavior.md) | 앱에서 구간 관리의 구간 추가 버튼을 눌러도 반응이 없으며, 모달 관련 로직이 누락된 것 같다는 문제 보고다. |
| [FC0480](fc/FC0480.md) | [UI 동작·사용성](25-ui-behavior.md) | 예약 완료 알림과 화면 표시 외에도 사용자가 자신의 예약을 다시 조회하거나 취소할 수 있는 사용자 친화적 흐름을 고민하도록 제안했다. |
| [FC0481](fc/FC0481.md) | [UI 동작·사용성](25-ui-behavior.md) | 대기 취소 시 해당 DOM 항목만 제거하면 같은 슬롯의 남은 대기 순번이 화면에서 갱신되지 않을 수 있으므로, 취소 성공 후 목록을 다시 조회하거나 순번을 재계산하는 방안을 제안했다. |
