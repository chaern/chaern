# chaern

**전장 하드웨어 · 산업 자동화 · 임베디드 제어**

전장 하드웨어 개발 실무에서 회로·부품과 PCB 변경 사항을 검토했습니다. 인텔 AI 융합 DX 과정에서는 PLC 순차제어, 서보 위치결정, 협동로봇 이송을 실습했습니다.

[**Intel DX 실습 포트폴리오**](https://github.com/chaern/intel_dx)

## PARK:ON · AI 스마트 주차장 통합관제

카메라와 AI로 실물·가상 주차장의 상태를 확인하는 6인 팀 프로젝트입니다. 사용자 웹·모바일과 관리자 관제 화면을 맡았고, 시연용 API·Docker 통합과 다국어 챗봇 사용성 개선을 진행했습니다. [팀 프로젝트 저장소](https://github.com/intel7-smart-parking-ai/smart-parking-ai)

| 담당 영역 | 구현 내용 | 병합 PR |
| --- | --- | --- |
| 사용자 웹·모바일 | 빈자리·전용칸을 표시하는 주차 지도, 차량 위치·이용 시간·요금 조회, 무료 회차 안내, 모의 결제·영수증 화면을 구현했습니다. | [#52](https://github.com/intel7-smart-parking-ai/smart-parking-ai/pull/52) · [#138](https://github.com/intel7-smart-parking-ai/smart-parking-ai/pull/138) · [#150](https://github.com/intel7-smart-parking-ai/smart-parking-ai/pull/150) |
| 관리자 통합관제 | 현재 입차와 출차 이력, 고객 호출, 월별 매출·안전 현황을 표시했습니다. 확인이 필요한 주차면을 빈자리와 구분하고 대피 경보 중 결제를 차단했습니다. | [#52](https://github.com/intel7-smart-parking-ai/smart-parking-ai/pull/52) · [#100](https://github.com/intel7-smart-parking-ai/smart-parking-ai/pull/100) · [#126](https://github.com/intel7-smart-parking-ai/smart-parking-ai/pull/126) |
| API·배포 통합 | 기존 점유 엔진에 세션·요금·경보 API를 연결하고, SQLite 이벤트 복구와 Docker Compose 기반 웹·API·관리자 인증 구성을 추가했습니다. | [#53](https://github.com/intel7-smart-parking-ai/smart-parking-ai/pull/53) · [#54](https://github.com/intel7-smart-parking-ai/smart-parking-ai/pull/54) |
| 다국어 챗봇 UI | 웹·모바일 채팅 화면을 정리하고 한국어·영어·중국어·일본어 응답 표시, 음성 입력 자동 전송, iPhone Safari 기기 음성 선택을 적용했습니다. | [#74](https://github.com/intel7-smart-parking-ai/smart-parking-ai/pull/74) · [#144](https://github.com/intel7-smart-parking-ai/smart-parking-ai/pull/144) · [#152](https://github.com/intel7-smart-parking-ai/smart-parking-ai/pull/152) |

- **기술 스택** · React, Vite, FastAPI, SQLite, Docker Compose, Nginx
- **검증** · 통합 시연 환경에서 입차 → 요금 조회 → 모의 결제 → 출차와 경보 중 결제 차단, API 재시작 후 상태 보존을 확인했습니다. Docker 통합 PR에는 백엔드 테스트 350개, iPhone 음성 개선 PR에는 프론트엔드 테스트 90개 통과를 기록했습니다. [#54](https://github.com/intel7-smart-parking-ai/smart-parking-ai/pull/54) · [#152](https://github.com/intel7-smart-parking-ai/smart-parking-ai/pull/152)
- **공동 담당** · 차량 번호 스티커 인식 AI는 팀원과 공동 담당했습니다. [팀 역할 분담](https://github.com/intel7-smart-parking-ai/smart-parking-ai/blob/main/README.md#3-팀-구성-및-담당-업무)

## 자동화 프로젝트

| 프로젝트 | 수행 내용 | 실습 자료 |
| --- | --- | --- |
| **Factory I/O 금속·비금속 분류** | 가상 컨베이어 공정을 PLC와 연결하고, 비전 센서의 4비트 출력으로 작업물을 구분하는 제어를 실습했습니다. | [센서·입출력 정리](https://github.com/chaern/intel_dx/blob/main/PLC/1007/sensor.txt) |
| **Indy7 로봇 이송·격자 적재** | 실제 로봇으로 물체를 집어 이송하고 반복 적재했습니다. 교육 코드에는 5×5 격자 좌표 계산과 PLC 워드 명령을 작업 위치로 변환하는 로직이 담겨 있습니다. | [격자 적재 코드](https://github.com/chaern/intel_dx/blob/main/robot/0908/25repeat.py) · [PLC 명령 처리 코드](https://github.com/chaern/intel_dx/blob/main/robot/1002/plc_slide.py) |
| **MELSEC-Q 서보 위치결정** | PLC와 위치결정 모듈을 사용해 원점복귀, JOG 운전, 위치 티칭을 실습했습니다. | [서보 실습 문서](https://github.com/chaern/intel_dx/blob/main/PLC/0901/README.md) |

## 임베디드 프로젝트

- **ATmega128 디지털 도어락** · 팀장으로 키패드 입력 문제를 팀원들과 분석했습니다. 제어 순서와 지연시간을 수정해 동작을 확인하고 비밀번호 재설정·초기화 기능을 추가했습니다.
- **8×8×8 LED Cube** · 회로 제작과 납땜, LED 출력 제어 로직을 맡았습니다. 패턴별 출력 순서와 지연시간을 조정하고 반복 구동으로 동작을 확인했습니다.

## 학습 저장소

[PLC 제어 실습](https://github.com/chaern/intel_dx/tree/main/PLC) · [로봇 제어 실습](https://github.com/chaern/intel_dx/tree/main/robot) · [Python·AI 실습](https://github.com/chaern/intel_dx/tree/main/AI_PGM)
