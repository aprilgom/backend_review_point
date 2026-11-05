# 백엔드 FC 예시 코드 체크리스트

## 분야별 문서

[FC 번호로 찾기](FC_INDEX.md)

분야 목차에서 각 FC의 독립 문서로 이동할 수 있습니다. FC 문서에는 소속 분야, 이전·다음 FC, 관련 FC 링크가 있습니다. 모든 문서 링크는 이 폴더 안에서 연결됩니다.

| 분야 | FC 수 | 함께 볼 분야 |
| --- | ---: | --- |
| [추상화·중복](01-abstraction.md) | 32 | [의존성·교체 가능성](09-dependency.md) · [책임·계층 경계](19-responsibility.md) |
| [접근성·의미론](02-accessibility.md) | 3 | [렌더링·데이터 로딩](18-rendering.md) · [UI 동작·사용성](25-ui-behavior.md) |
| [API·공개 인터페이스 계약](03-api-contract.md) | 18 | [예외·실패 계약](13-errors.md) · [인증·보안·비밀값](20-security.md) · [타입·타입 테스트](24-type-safety.md) |
| [빌드·환경·배포](04-build-config.md) | 20 | [로그·관측](15-observability.md) · [테스트 준비·격리](22-test-isolation.md) |
| [비동기·동시성](05-concurrency.md) | 15 | [성능·측정](16-performance.md) · [트랜잭션·자원 수명](23-transaction.md) |
| [엔티티 동등성·식별](06-identity.md) | 4 | [데이터 관계·영속성](08-persistence.md) · [도메인 모델·값 표현](11-domain-model.md) |
| [쿼리·데이터 조작](07-data-query.md) | 12 | [데이터 관계·영속성](08-persistence.md) · [성능·측정](16-performance.md) |
| [데이터 관계·영속성](08-persistence.md) | 17 | [엔티티 동등성·식별](06-identity.md) · [쿼리·데이터 조작](07-data-query.md) · [트랜잭션·자원 수명](23-transaction.md) |
| [의존성·교체 가능성](09-dependency.md) | 40 | [추상화·중복](01-abstraction.md) · [책임·계층 경계](19-responsibility.md) · [테스트 준비·격리](22-test-isolation.md) |
| [문서·개발·학습 과정](10-workflow.md) | 11 | [가독성·명명](17-readability.md) · [테스트 대상·검증](21-test-behavior.md) |
| [도메인 모델·값 표현](11-domain-model.md) | 12 | [엔티티 동등성·식별](06-identity.md) · [도메인 검증](12-validation.md) · [책임·계층 경계](19-responsibility.md) |
| [도메인 검증](12-validation.md) | 25 | [도메인 모델·값 표현](11-domain-model.md) · [예외·실패 계약](13-errors.md) · [인증·보안·비밀값](20-security.md) · [테스트 대상·검증](21-test-behavior.md) |
| [예외·실패 계약](13-errors.md) | 15 | [API·공개 인터페이스 계약](03-api-contract.md) · [도메인 검증](12-validation.md) · [로그·관측](15-observability.md) · [트랜잭션·자원 수명](23-transaction.md) |
| [프론트엔드 상태](14-frontend-state.md) | 2 | [렌더링·데이터 로딩](18-rendering.md) · [UI 동작·사용성](25-ui-behavior.md) |
| [로그·관측](15-observability.md) | 3 | [빌드·환경·배포](04-build-config.md) · [예외·실패 계약](13-errors.md) · [성능·측정](16-performance.md) |
| [성능·측정](16-performance.md) | 28 | [비동기·동시성](05-concurrency.md) · [쿼리·데이터 조작](07-data-query.md) · [로그·관측](15-observability.md) |
| [가독성·명명](17-readability.md) | 47 | [문서·개발·학습 과정](10-workflow.md) · [타입·타입 테스트](24-type-safety.md) |
| [렌더링·데이터 로딩](18-rendering.md) | 9 | [접근성·의미론](02-accessibility.md) · [프론트엔드 상태](14-frontend-state.md) · [UI 동작·사용성](25-ui-behavior.md) |
| [책임·계층 경계](19-responsibility.md) | 31 | [추상화·중복](01-abstraction.md) · [의존성·교체 가능성](09-dependency.md) · [도메인 모델·값 표현](11-domain-model.md) |
| [인증·보안·비밀값](20-security.md) | 6 | [API·공개 인터페이스 계약](03-api-contract.md) · [도메인 검증](12-validation.md) |
| [테스트 대상·검증](21-test-behavior.md) | 28 | [문서·개발·학습 과정](10-workflow.md) · [도메인 검증](12-validation.md) · [테스트 준비·격리](22-test-isolation.md) |
| [테스트 준비·격리](22-test-isolation.md) | 24 | [빌드·환경·배포](04-build-config.md) · [의존성·교체 가능성](09-dependency.md) · [테스트 대상·검증](21-test-behavior.md) · [트랜잭션·자원 수명](23-transaction.md) |
| [트랜잭션·자원 수명](23-transaction.md) | 4 | [비동기·동시성](05-concurrency.md) · [데이터 관계·영속성](08-persistence.md) · [예외·실패 계약](13-errors.md) · [테스트 준비·격리](22-test-isolation.md) |
| [타입·타입 테스트](24-type-safety.md) | 8 | [API·공개 인터페이스 계약](03-api-contract.md) · [가독성·명명](17-readability.md) |
| [UI 동작·사용성](25-ui-behavior.md) | 13 | [접근성·의미론](02-accessibility.md) · [프론트엔드 상태](14-frontend-state.md) · [렌더링·데이터 로딩](18-rendering.md) |
