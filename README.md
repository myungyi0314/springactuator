## # 감사로그를 수집하는 방법

1. ` AOP (Aspect-Oriented Programming)`: AOP를 사용하여 감사 로그를 캡슐화하고 여러 컴포넌트에 적용할 수 있습니다. Spring의 AOP 기능을 사용하여 로깅 어드바이스를 작성하고,
   필요한
   컴포넌트 또는 메소드에 어드바이스를 적용하여 감사 로그를 수집합니다. 예를 들어, 메소드 실행 전후에 로그를 작성하거나, 예외가 발생할 때 로그를 기록할 수 있습니다.

2. `Interceptors`: Spring의 Interceptor를 사용하여 요청 전후에 로그를 작성할 수 있습니다. HandlerInterceptor 인터페이스를 구현하여 요청을 가로채고 필요한 로그를 작성할 수
   있습니다. 예를 들어, 인증 정보, 요청 URL, 요청 매개변수 등을 로그에 기록할 수 있습니다.

3. `ApplicationEvent 및 ApplicationListener`: Spring의 이벤트 기능을 사용하여 감사 로그를 수집할 수 있습니다. ApplicationEvent를 상속받은 사용자 정의 이벤트를
   정의하고,
   ApplicationListener 인터페이스를 구현하여 이벤트를 수신하고 필요한 로그를 작성할 수 있습니다. 예를 들어, 애플리케이션 내의 특정 이벤트 발생 시 로그를 작성할 수 있습니다.

4. `Logging 프레임워크`: Spring Boot는 로깅을 위해 다양한 로깅 프레임워크를 지원합니다. Logback, Log4j, SLF4J 등을 사용하여 감사 로그를 수집할 수 있습니다. 로깅 프레임워크를
   설정하고 로깅
   레벨을 조정하여 필요한 정보를 로그로 기록할 수 있습니다.

5. `Spring Boot Actuator`: spring actuator를 사용하여 감사 로그를 수집할 수 있습니다. Actuator는 애플리케이션의 모니터링 및 관리를 위한 엔드포인트를 제공하며, 기본적으로 액세스 로그를 수집합니다. Actuator
엔드포인트를 통해 감사 로그 데이터를 확인하고 이를 원하는 저장소에 저장하거나 처리할 수 있습니다.