# chaern

**전장 하드웨어 · 산업 자동화 · 임베디드 제어**

전장 하드웨어 개발 실무에서 회로·부품과 PCB 변경 사항을 검토했습니다. 인텔 AI 융합 DX 과정에서는 PLC 순차제어, 서보 위치결정, 협동로봇 이송을 실습했습니다.

[**Intel DX 실습 포트폴리오**](https://github.com/chaern/intel_dx)

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
