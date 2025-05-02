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
</table>

## 방탈출 예약 관리

- [add 메서드 결과 반환을 위한 재조회 필요성 검토](https://github.com/woowacourse/spring-roomescape-admin/pull/314#discussion_r2059550482)
- [존재 여부 확인을 위한 쿼리 개선, EXISTS vs COUNT(\*), 인덱스](https://github.com/woowacourse/spring-roomescape-admin/pull/314#discussion_r2061297911)
- [메서드의 원자적인 실행을 보장하기 위한 @Transactional](https://github.com/woowacourse/spring-roomescape-admin/pull/314#pullrequestreview-2795982141)

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
</table>

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
