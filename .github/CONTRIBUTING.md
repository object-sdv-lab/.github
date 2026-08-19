## 개발 절차

1. 이슈 생성
2. 브랜치 생성
3. 구현
4. 풀 리퀘스트 생성
5. 코드 리뷰
6. 머지

## 네이밍 룰

### 브랜치
- 기능 개발: `feature/123-vehicle-state-monitor`
- 오류 수정: `fix/456-sensor-timeout`
- 문서 추가·수정: `docs/789-update-driving-mode-guide`

### 커밋 메시지
- 기능 추가: `feat: 차량 상태 모니터링 기능 추가`
- 오류 수정: `fix: 센서 데이터 수신 지연 시 잘못된 상태 전이 수정`
- 리팩토링: `refactor: 차량 상태 검증 로직 분리`
- 문서 추가·수정: `docs: 주행 모드 전환 절차 보완`
- 테스트 추가·수정: `test: 통신 단절 및 재연결 시나리오 추가`
- 개발 환경 및 기타 유지보수: `chore: 개발 도구 설정 갱신`

### 코드
| 대상 | 예시 |
| --- | --- |
| 클래스, 구조체, 열거형, 타입 별칭 | `VehicleStateMonitor`, `SensorStatus` |
| 인터페이스 | `IVehicleStateMonitor`, `ISensorGateway` |
| 함수, 메서드 | `update_vehicle_state()`, `is_signal_valid()` |
| 지역 변수, 매개변수 | `vehicle_speed_kph`, `sensor_status` |
| 클래스 멤버 변수 | `vehicle_speed_kph_`, `sensor_status_` |
| 상수, 상수 표현식, 매크로 | `MAX_VEHICLE_SPEED_KPH`, `SENSOR_TIMEOUT_MS`, `VEHICLE_CONTROL_ENABLED` |
| 네임스페이스 | `vehicle_control`, `sensor_gateway` |
