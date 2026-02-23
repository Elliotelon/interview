# swift 문법

Struct vs Class 차이점은?
→ Struct는 값 타입, Class는 참조 타입이며 상속 가능 여부가 다름.

ARC란?
→ 참조 카운트를 기반으로 객체 메모리를 자동 관리하는 방식.

Strong Reference Cycle이란?
→ 서로 강한 참조를 유지해 메모리 해제가 되지 않는 상태.

weak vs unowned 차이?
→ weak는 Optional이며 자동 nil 처리, unowned는 비Optional이고 nil이 되면 크래시.

Optional이란?
→ 값이 있을 수도 없을 수도 있는 타입.

if let과 guard let 차이?
→ guard는 조건 실패 시 조기 종료를 강제한다.

Copy-on-Write란?
→ 실제 수정 시점에만 복사가 일어나는 메모리 최적화 기법.

Protocol이란?
→ 타입이 반드시 구현해야 하는 요구사항 정의.

Protocol Extension의 장점은?
→ 기본 구현 제공으로 코드 재사용 가능.

Generic이란?
→ 타입에 독립적인 재사용 가능한 코드 작성 방식.

@escaping은 언제 쓰는가?
→ 함수 종료 후에도 클로저가 실행될 때.

클로저 Capture란?
→ 클로저가 외부 변수 값을 저장하는 것.

mutating 키워드는?
→ Struct에서 프로퍼티를 변경할 때 사용.

Enum의 Associated Value란?
→ 케이스마다 추가 데이터를 저장하는 기능.

Raw Value와 Associated Value 차이?
→ Raw는 고정값, Associated는 동적 값.

접근제어자 종류는?
→ open, public, internal, fileprivate, private.

open과 public 차이?
→ open은 다른 모듈에서 상속 및 override 가능.

lazy는 언제 사용하는가?
→ 실제 사용 시점에 초기화가 필요할 때.

deinit은 언제 호출되는가?
→ 인스턴스가 메모리에서 해제될 때.

Any와 AnyObject 차이?
→ Any는 모든 타입, AnyObject는 클래스 타입만.

static vs class 차이?
→ static은 override 불가, class는 가능.

Subscript란?
→ 배열처럼 인덱스로 접근 가능하게 하는 기능.

inout 키워드는?
→ 함수 내부에서 외부 변수 값을 직접 변경.

defer란?
→ 스코프 종료 직전에 실행되는 코드 블록.

Error 처리 방식은?
→ do-try-catch 구문 사용.

try?, try!, try 차이?
→ try?는 nil 반환, try!는 크래시 가능.

Equatable이란?
→ 두 인스턴스 비교 가능하게 하는 프로토콜.

Hashable이란?
→ Set이나 Dictionary 키로 사용 가능하게 함.

map과 compactMap 차이?
→ compactMap은 nil 제거.

reduce는 무엇인가?
→ 컬렉션을 하나의 값으로 집계.

고차 함수란?
→ 함수를 인자로 받거나 반환하는 함수.

where절은 언제 사용하는가?
→ 제네릭 타입 제약 조건을 추가할 때.

associatedtype이란?
→ 프로토콜 내부에서 사용하는 추상 타입.

escaping과 non-escaping 기본 차이?
→ 기본은 non-escaping이며 함수 종료 전에 실행됨.

Value Type이 thread-safe한 이유는?
→ 복사되어 사용되기 때문.

is와 as 차이?
→ is는 타입 체크, as는 타입 캐스팅.

as?와 as! 차이?
→ as?는 Optional 반환, as!는 실패 시 크래시.

final 키워드는?
→ 상속이나 override를 금지.

Self와 self 차이?
→ Self는 타입, self는 인스턴스 참조.

required init이란?
→ 서브클래스에서 반드시 구현해야 하는 초기화자.

왜 Struct를 우선 사용해야 하는가?
→ 불변성과 안전성 측면에서 유리하기 때문.

클로저에서 [weak self]를 쓰는 이유는?
→ Retain Cycle 방지.

DispatchQueue.main.async를 쓰는 이유는?
→ UI 업데이트는 메인 스레드에서만 가능하기 때문.

escaping 클로저에서 self 캡처 문제는?
→ strong capture로 인해 메모리 누수 발생 가능.

computed property와 stored property 차이?
→ computed는 저장하지 않고 계산.

property observer란?
→ willSet, didSet으로 값 변경 감지.

Type Property란?
→ 타입 자체에 속하는 프로퍼티.

Convenience init이란?
→ 다른 초기화 생성자를 호출하는 보조 초기화 생성자.

Designated init이란?
→ 모든 프로퍼티를 초기화하는 기본 초기화 생성자.

Swift가 안전한 언어인 이유는?
→ Optional, 타입 안정성, ARC 등으로 런타임 오류를 최소화하기 때문.
