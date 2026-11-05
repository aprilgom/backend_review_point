# 비동기·동시성

[전체 목차](README.md) · [FC 번호별 목차](FC_INDEX.md) · [← 이전: 빌드·환경·배포](04-build-config.md) · [다음: 엔티티 동등성·식별 →](06-identity.md)

**관련 분야:** [성능·측정](16-performance.md) · [트랜잭션·자원 수명](23-transaction.md)

## 이 분야의 FC

- [FC0100 · Session 내부 HashMap에도 동시성 고려가 필요한지, 필요하다면 어떤 상황에서 동시 접근이 발생하는지 질문했다.](fc/FC0100.md)

- [FC0103 · 동시 요청이 애플리케이션의 중복 검사를 함께 통과하면 중복 저장이 가능하므로 데이터베이스에서도 정합성을 보장해야 한다는 우려다.](fc/FC0103.md)

- [FC0098 · 요청마다 스레드를 새로 생성하는 방식에서 어떤 문제가 생길 수 있는지 고민해 보도록 권했다.](fc/FC0098.md)

- [FC0104 · 여러 스레드가 동시에 접근하는 세션 저장소를 ConcurrentHashMap으로 처리해 보자고 제안했다.](fc/FC0104.md)

- [FC0101 · 대기 생성 요청이 거의 동시에 들어오는 상황을 검토하고 트랜잭션 격리 수준을 확인해보자는 제안이다.](fc/FC0101.md)

- [FC0106 · 스레드 풀의 최대 스레드 수를 보통 어느 정도로 설정하는지 학습해 보도록 제안했다.](fc/FC0106.md)

- [FC0099 · calculate 메서드에 synchronized를 붙이면 테스트가 통과하는 이유를 질문했다.](fc/FC0099.md)

- [FC0108 · Executors의 여러 스레드 풀 생성 방식 중 FixedThreadPool을 선택한 이유를 질문했다.](fc/FC0108.md)

- [FC0109 · 예약과 대기의 API가 분리된 상태에서 예약 취소와 해당 슬롯의 대기 신청이 동시에 발생해도 문제가 없는지 검토하도록 요청했다.](fc/FC0109.md)

- [FC0097 · 복제 지연 대응으로 reader 조회 결과가 없을 때 writer를 조회하는 방식을 선택한 이유를 묻는다.](fc/FC0097.md)

- [FC0110 · 작업 실행에 submit() 대신 execute()를 선택한 이유를 질문했다.](fc/FC0110.md)

- [FC0111 · Long과 AtomicLong의 차이와 예약 ID 생성에 AtomicLong을 사용하는 이유를 설명하도록 질문했다.](fc/FC0111.md)

- [FC0105 · 학습 차원에서 ThreadLocal이 무엇인지 설명해 달라고 질문했다.](fc/FC0105.md)

- [FC0102 · ArgumentResolver와 Interceptor를 사용할 때 각각 요청이 처리되는 순서를 질문한다.](fc/FC0102.md)

- [FC0107 · RedisTemplate의 내부 호출이 동기인지 비동기인지, 그리고 캐시 TTL 연장 메서드에 비동기를 사용한 이유가 무엇인지 물었다.](fc/FC0107.md)


---

[전체 목차](README.md) · [FC 번호별 목차](FC_INDEX.md) · [← 이전: 빌드·환경·배포](04-build-config.md) · [다음: 엔티티 동등성·식별 →](06-identity.md)
