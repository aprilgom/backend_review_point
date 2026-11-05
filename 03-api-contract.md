# API·공개 인터페이스 계약

[전체 목차](README.md) · [FC 번호별 목차](FC_INDEX.md) · [← 이전: 접근성·의미론](02-accessibility.md) · [다음: 빌드·환경·배포 →](04-build-config.md)

**관련 분야:** [예외·실패 계약](13-errors.md) · [인증·보안·비밀값](20-security.md) · [타입·타입 테스트](24-type-safety.md)

## 이 분야의 FC

- [FC0053 · 항상 기본값만 사용하는 것으로 보이는 whiteName과 blackName을 요청 파라미터로 받는 이유를 질문했다.](fc/FC0053.md)

- [FC0054 · JSON 본문을 사용하지 않고 RequestParam으로 입력을 받는다면 application/json 대신 다른 Content-Type을 고려하도록 제안했다.](fc/FC0054.md)

- [FC0057 · 로그인 상태에서 GET /login 요청 시 index.html로 리다이렉트하는 요구사항이 동작하지 않는 것으로 보여 확인을 요청했다.](fc/FC0057.md)

- [FC0058 · RequestUri의 hasRequestParameters 메서드가 테스트에서만 사용되는 메서드임을 지적했다.](fc/FC0058.md)

- [FC0059 · API와 페이지 URL 경로의 결정 기준을 묻고 RESTful 경로 설계와 자신의 선택 기준을 고민해 볼 것을 제안했다.](fc/FC0059.md)

- [FC0061 · 본문을 반환하지 않는 성공 응답에 200을 사용한 이유와 이 경우 적절한 응답 상태 코드를 묻는다.](fc/FC0061.md)

- [FC0063 · RequestMapping의 method가 배열인 만큼 여러 RequestMethod를 입력했을 때의 매핑 동작을 명확히 정해보자고 제안했다.](fc/FC0063.md)

- [FC0055 · HandlerExecution이 String뿐 아니라 ModelAndView 등 여러 반환 타입을 지원하도록 바꾸자고 제안했다.](fc/FC0055.md)

- [FC0066 · 예약 가능 여부를 포함하는 시간 조회 API의 요청과 응답을 현재 형태로 설계한 이유를 질문했다.](fc/FC0066.md)

- [FC0064 · 직접 사용하지 않는 기본 생성자의 접근 제한자를 public에서 protected로 변경할 것을 제안한다.](fc/FC0064.md)

- [FC0067 · API 안정성을 DTO 사용 근거로 들면서 요청에만 DTO를 적용한 이유와, 도메인 변경이 응답 형식에도 영향을 줄 가능성을 질문했다.](fc/FC0067.md)

- [FC0060 · LoginMember 타입만으로 인자 해석 대상을 정하지 말고, hasParameterAnnotation()을 활용해 특정 조건을 만족하는 파라미터에만 로그인 정보를 제공하도록 제안했다.](fc/FC0060.md)

- [FC0069 · 별도 사용처가 없는 기본 생성자의 접근 범위를 protected에서 public으로 넓힌 이유를 질문했다.](fc/FC0069.md)

- [FC0070 · Member의 @NoArgsConstructor에 생성자 접근 수준 설정이 빠져 있다고 지적한다.](fc/FC0070.md)

- [FC0065 · JSON 응답에 Content-Type을 지정했을 때와 지정하지 않았을 때의 차이를 질문했다.](fc/FC0065.md)

- [FC0071 · 정적 팩토리 메서드가 있고 생성자를 별도로 사용하지 않는다면 RequestUri 생성자를 private으로 제한하는 방안을 제안했다.](fc/FC0071.md)

- [FC0072 · 상품 수정 API에서 PUT과 PATCH의 차이를 이해하고 PATCH 사용도 고려했는지 묻는다.](fc/FC0072.md)

- [FC0062 · 쿠키를 세미콜론과 공백 한 개로 분리하면 공백이 없거나 여러 개인 입력을 제대로 파싱하지 못할 수 있으므로 공백을 정리해 처리하도록 제안한다.](fc/FC0062.md)


---

[전체 목차](README.md) · [FC 번호별 목차](FC_INDEX.md) · [← 이전: 접근성·의미론](02-accessibility.md) · [다음: 빌드·환경·배포 →](04-build-config.md)
