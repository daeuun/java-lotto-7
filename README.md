# 로또
## 기능 목록
### 1. 사용자에게 로또 구입 금액을 입력 받고, 발행한 로또 수량 및 번호를 출력한다.
- 구입 금액은 1,000원 단위로 입력 받는다.
    - `readLine()` 를 사용하여 입력받는다.
    - 1,000원으로 나누어 떨어지지 않는 경우 예외 처리한다.
- 로또 1장의 가격은 1,000원이고, 구입 금액에 해당하는 만큼 로또를 발행한다.
- 1개의 로또를 발행할 때 중복되지 않는 6개의 숫자를 랜덤으로 뽑는다.
- 발행한 로또 번호는 오름차순으로 정렬하여 출력한다.

### 2. 당첨 번호, 보너스 번호를 입력 받는다.

- 입력할 수 있는 로또 번호의 숫자 범위는 1~45까지이다.
- 당첨 번호는 쉼표(,)를 기준으로 구분하여 입력 받는다.
- 입력 받는 당첨 번호 6개와 보너스 번호 1개는 중복되지 않는 숫자여야 한다.

### 3. 로또 번호를 추첨한다.

- 당첨 번호 추첨 시 중복되지 않는 숫자 6개와 보너스 번호 1개를 뽑는다.
    - `pickUniqueNumbersInRange()` 를 사용하여 랜덤값을 추출한다.
- 사용자가 구매한 로또 번호와 추첨한 당첨 번호를 비교한다.
- 당첨 기준에 따라 1등~5등까지 기준에 따라 몇 개의 번호가 일치하는지 당첨 내역을 판정한다.
    - 당첨 기준 정의하는데 `Enum`을 적용한다.

### 4. 당첨 통계를 출력한다.

- 당첨 내역 및 수익률을 출력한다.
- 수익률은 소수점 둘째 자리에서 반올림한다.

### 5. 예외 처리

- 예외 상황 시 에러 문구를 출력해야 한다. 단, 에러 문구는 "[ERROR]"로 시작한다.
