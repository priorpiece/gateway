# Gateway Service

모든 클라이언트 요청의 진입점. 로드밸런싱을 담당.

## 기술 스택

| 항목 | 내용 |
|------|------|
| Language | Kotlin |
| Framework | Spring Cloud Gateway (WebFlux) |
| 인증 | JWT (jjwt) |
| 로드밸런싱 | Spring Cloud LoadBalancer |
| 서비스 등록 | Netflix Eureka Client |

## 주요 기능

- 클라이언트 요청을 각 마이크로서비스로 라우팅
- JWT 토큰 기반 인증 필터 처리
- Eureka를 통한 서비스 디스커버리 및 로드밸런싱
- 포트: `8000`