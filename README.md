# woowacourse-archive

우아한테크코스 7기 BE 기록

# Level 2

> 학습해야 하는 내용의 범위가 넓고 깊다. 절대적인 진리나 정답은 없으며, 왜?를 고민하고 함께 합의하는 과정이 중요하다.

<table>
  <thead>
    <tr>
      <th>미션</th>
      <th>키워드</th>
      <th>PR</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2"><a href="#방탈출-예약-관리">방탈출 예약 관리</a></td>
      <td rowspan="2">Web, HTTP, Spring Boot, Jdbc, RDBMS</td>
      <td><a href="https://github.com/woowacourse/spring-roomescape-admin/pull/265">페어 미션 PR</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/woowacourse/spring-roomescape-admin/pull/314">개인 미션 PR</a></td>
    </tr>
  </tbody>
  <tbody>
    <tr>
      <td rowspan="2"><a href="#방탈출-사용자-예약">방탈출 사용자 예약</a></td>
      <td rowspan="2">예외 처리, Interceptor, Argument Resolver</td>
      <td><a href="https://github.com/woowacourse/spring-roomescape-member/pull/225">페어 미션 PR</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/woowacourse/spring-roomescape-member/pull/283">개인 미션 PR</a></td>
    </tr>
  </tbody>
  <tbody>
    <tr>
      <td rowspan="2"><a href="#방탈출-예약-대기">방탈출 예약 대기</a></td>
      <td rowspan="2">JPA 도입, 도메인 간 강결합</td>
      <td><a href="https://github.com/woowacourse/spring-roomescape-waiting/pull/195">페어 미션 PR</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/woowacourse/spring-roomescape-waiting/pull/261">개인 미션 PR</a></td>
    </tr>
  </tbody>
  <tbody>
    <tr>
      <td rowspan="2"><a href="#방탈출-결제배포">방탈출 결제/배포</a></td>
      <td rowspan="2">외부 API, 배포, 로깅</td>
      <td><a href="https://github.com/woowacourse/spring-roomescape-payment/pull/169">페어 미션 PR</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/woowacourse/spring-roomescape-payment/pull/248">개인 미션 PR</a></td>
    </tr>
  </tbody>
  <tbody>
    <tr>
      <td><a href="#레벨2-글쓰기">레벨2 글쓰기</a></td>
      <td>레벨2까지 나의 성장 여정</td>
      <td><a href="https://github.com/woowacourse/woowa-writing/pull/881">미션 PR</a></td>
    </tr>
  </tbody>
  <tbody>
    <tr>
      <td><a href="#레벨2-파이널-미션">레벨2 파이널 미션</a></td>
      <td>제한시간 내 AI 사용 없이 나만의 예약 서비스 API 제작</td>
      <td><a href="https://github.com/woowacourse/lv2-final-mission/pull/14">미션 PR</a></td>
    </tr>
  </tbody>
</table>

## 방탈출 예약 관리

- [add 메서드 결과 반환을 위한 재조회 필요성 검토](https://github.com/woowacourse/spring-roomescape-admin/pull/314#discussion_r2059550482)
- [존재 여부 확인을 위한 쿼리 개선, EXISTS vs COUNT(\*), 인덱스](https://github.com/woowacourse/spring-roomescape-admin/pull/314#discussion_r2061297911)
- [메서드의 원자적인 실행을 보장하기 위한 @Transactional](https://github.com/woowacourse/spring-roomescape-admin/pull/314#pullrequestreview-2795982141)

## 방탈출 사용자 예약

- [도메인 예외를 따로 추가한 이유](https://github.com/woowacourse/spring-roomescape-member/pull/225#discussion_r2072400381)
- [한방 쿼리에 관하여](https://github.com/YehyeokBang/TIL/issues/3)
- [도메인 객체에도 id가 존재하는 이유](https://github.com/woowacourse/spring-roomescape-member/pull/283#discussion_r2083520362)

## 방탈출 예약 대기

- [무조건 fetch join으로 다 가져오는 것이 좋을까?](https://github.com/woowacourse/spring-roomescape-waiting/pull/195#discussion_r2090449417)
  - 도메인에 대한 이해와 규모에 관한 합의로 결정할 수 있다.
- [XXService를 조회성과 명령성으로 분리](https://github.com/woowacourse/spring-roomescape-waiting/pull/261#discussion_r2100673968)
- [복잡해지는 요구사항 속 도메인 간 강결합 해소](https://velog.io/@hyeok_1212/%EB%B3%B5%EC%9E%A1%ED%95%B4%EC%A7%80%EB%8A%94-%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD-%EC%86%8D-%EB%8F%84%EB%A9%94%EC%9D%B8-%EA%B0%84-%EA%B0%95%EA%B2%B0%ED%95%A9)
  - 이벤트 발행-수신 구조를 활용한 도메인 간 느슨한 결합

## 방탈출 결제/배포

- 외부 API [Connection Timeout, Read Timeout 설정](https://github.com/woowacourse/spring-roomescape-payment/pull/169#discussion_r2113346611)
- 예약 [삭제와 취소의 차이](https://github.com/woowacourse/spring-roomescape-payment/pull/248#discussion_r2132387545)
- [남겨야 할 로그에 대하여](https://github.com/woowacourse/spring-roomescape-payment/pull/248#discussion_r2133995908)
- [@TransactionalEventListener(AFTER_COMMIT)에서 업데이트가 반영되지 않던 문제 분석](https://github.com/woowacourse/spring-roomescape-payment/pull/248#discussion_r2133849471)

## 레벨2 글쓰기

- 완벽한 논리보다, 실패해도 리스크가 작은 선택을 빠르게 시도해 보는 것이 나에게 도움이 될 것 같다.

## 레벨2 파이널 미션

- 내가 성장한 부분과 부족한 부분을 인지하는 미션이었다.
- 기획에서 과도한 설계로 인해 정작 완성하지 못한 부분이 있었다.

# Level 1

> 현장은 클린코드도 중요하지만 마감 시간 내에 동작하는 코드를 구현하는 것이 더 중요하다.

<table>
  <thead>
    <tr>
      <th>미션</th>
      <th>키워드</th>
      <th>PR</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2"><a href="#로또">로또</a></td>
      <td rowspan="2">단위 테스트</td>
      <td><a href="https://github.com/woowacourse/java-lotto/pull/510">페어 미션 PR</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/woowacourse/java-lotto/pull/621 ">개인 미션 PR</a></td>
    </tr>
    <tr>
      <td rowspan="2"><a href="#출석">출석</a></td>
      <td rowspan="2">TDD</td>
      <td><a href="https://github.com/woowacourse/java-attendance/pull/45">페어 미션 PR</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/woowacourse/java-attendance/pull/116">개인 미션 PR</a></td>
    </tr>
    <tr>
      <td rowspan="2"><a href="#블랙잭">블랙잭</a></td>
      <td rowspan="2">클린 코드</td>
      <td><a href="https://github.com/woowacourse/java-blackjack/pull/802">페어 미션 PR</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/woowacourse/java-blackjack/pull/903">개인 미션 PR</a></td>
    </tr>
    <tr>
      <td rowspan="2"><a href="#장기">장기</a></td>
      <td rowspan="2">OOP, DB</td>
      <td><a href="https://github.com/woowacourse/java-janggi/pull/62
">페어 미션 PR</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/woowacourse/java-janggi/pull/112">개인 미션 PR</a></td>
    </tr>
  </tbody>
  <tbody>
    <tr>
      <td><a href="#레벨1-글쓰기">레벨1 글쓰기</a></td>
      <td>유연함 강화 스터디 회고</td>
      <td><a href="https://github.com/woowacourse/woowa-writing/pull/745">미션 PR</a></td>
    </tr>
  </tbody>
</table>

- [Level 1 회고](https://velog.io/@hyeok_1212/%EC%9A%B0%EC%95%84%ED%95%9C%ED%85%8C%ED%81%AC%EC%BD%94%EC%8A%A4-7%EA%B8%B0-%EB%A0%88%EB%B2%A81-%ED%9A%8C%EA%B3%A0)

## 로또

- [인터페이스의 default 메서드와 구현체 검증 책임의 위치 고민](https://github.com/woowacourse/java-lotto/pull/621#discussion_r1958509135)
- 코드의 일관성은 가독성을 높이고, 유지보수성을 높인다.
  - 조건문의 비교 순서, `MAX > MIN` 보단 `MIN < MAX`가 더 직관적이다.
  - 조건문 분리(메서드 또는 변수로 추출) 행위에 관한 일관성을 높인다.

## 출석

- [불변 객체는 항상 좋은가?](https://github.com/YehyeokBang/TIL/issues/2)
- 개행, 공백, 주석, 테스트 코드의 일관성은 신뢰성 측면에서 중요하다.

## 블랙잭

- [추상 클래스 상속 vs 컴포지션](https://github.com/woowacourse/java-blackjack/pull/802#issuecomment-2709474830)
- [split() 메서드를 사용하며 발생한 문제를 해결한 과정](https://github.com/woowacourse/java-blackjack/pull/802#discussion_r1985997871)
  - [String.split() 메서드 학습 로그](https://github.com/YehyeokBang/TIL/blob/main/Java/JavaStringSplitMethod.md)
- [어떤 현상이 문제인지 인지하고 개선하는 것은 매우 중요하다.](https://github.com/woowacourse/java-blackjack/pull/903#discussion_r1998049068)

## 장기

- [새로운 환경에 대한 안내(실행 방법 등)는 당연하게 있어야 한다.](https://github.com/woowacourse/java-janggi/pull/112#discussion_r2020184410)
- [특정 DB의 기능을 사용하여 비즈니스적인 문제를 풀지 않아야 한다.](https://github.com/YehyeokBang/TIL/issues/1)
- 급하게 답변을 남기는 것보다 조금 더 고민하고 일관된 답변을 남기는 것이 좋을 것 같다.

## 레벨1 글쓰기

- 인지하지 못했던 나의 부족한 부분을 인지할 수 있었다.

# 프리코스

> 다양한 사람과 함께 성장하기 위한 준비하는 과정이다. 그 과정에서 나 스스로를 돌아보고 나아질 수 있는 방법을 고민한다.

<table>
  <thead>
    <tr>
      <th>미션</th>
      <th>PR</th>
      <th>회고</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>문자열 덧셈 계산기</td>
      <td><a href="https://github.com/woowacourse-precourse/java-calculator-7/pull/1103">미션 PR</a></td>
      <td><a href="https://velog.io/@hyeok_1212/%EC%9A%B0%EC%95%84%ED%95%9C%ED%85%8C%ED%81%AC%EC%BD%94%EC%8A%A4-7%EA%B8%B0-%ED%94%84%EB%A6%AC%EC%BD%94%EC%8A%A4-1%EC%A3%BC-%EC%B0%A8-BE">회고</a></td>
    </tr>
    <tr>
      <td>자동차 경주</td>
      <td><a href="https://github.com/woowacourse-precourse/java-racingcar-7/pull/1294">미션 PR</a></td>
      <td><a href="https://velog.io/@hyeok_1212/%EC%9A%B0%EC%95%84%ED%95%9C%ED%85%8C%ED%81%AC%EC%BD%94%EC%8A%A4-7%EA%B8%B0-%ED%94%84%EB%A6%AC%EC%BD%94%EC%8A%A4-2%EC%A3%BC-%EC%B0%A8-BE">회고</a></td>
    </tr>
    <tr>
      <td>로또</td>
      <td><a href="https://github.com/woowacourse-precourse/java-lotto-7/pull/565">미션 PR</a></td>
      <td><a href="https://velog.io/@hyeok_1212/%EC%9A%B0%EC%95%84%ED%95%9C%ED%85%8C%ED%81%AC%EC%BD%94%EC%8A%A4-7%EA%B8%B0-%ED%94%84%EB%A6%AC%EC%BD%94%EC%8A%A4-3%EC%A3%BC-%EC%B0%A8-BE">회고</a></td>
    </tr>
    <tr>
      <td>편의점</td>
      <td><a href="https://github.com/YehyeokBang/java-convenience-store-7-YehyeokBang">Repository</a></td>
      <td><a href="https://velog.io/@hyeok_1212/%EC%9A%B0%EC%95%84%ED%95%9C%ED%85%8C%ED%81%AC%EC%BD%94%EC%8A%A4-7%EA%B8%B0-%ED%94%84%EB%A6%AC%EC%BD%94%EC%8A%A4-4%EC%A3%BC-%EC%B0%A8-BE">회고</a></td>
    </tr>
  </tbody>
</table>

## 프리코스 학습 로그

- [[Java] Record 사용하시나요?](https://velog.io/@hyeok_1212/Java-Record-%EC%82%AC%EC%9A%A9%ED%95%98%EC%8B%9C%EB%82%98%EC%9A%94)
- [[Java] Enum 사용하시나요?](https://velog.io/@hyeok_1212/Java-enum-%EC%82%AC%EC%9A%A9%ED%95%98%EC%8B%9C%EB%82%98%EC%9A%94)
