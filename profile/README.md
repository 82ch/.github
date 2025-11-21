# 82ch

<p align="center">
  <img src="https://github.com/user-attachments/assets/64407558-fe51-4960-862c-05024ab1a912" width="200" height="200" />
</p>

<p align="center">
  <strong>MCP Security Framework</strong><br>
  Model Context Protocol 통신을 위한 실시간 보안 모니터링 및 위협 탐지 시스템
</p>

<p align="center">
  <a href="#-features">Features</a> •
  <a href="#-architecture">Architecture</a> •
  <a href="#-projects">Projects</a> •
  <a href="#-quick-start">Quick Start</a>
</p>

---

## What is 82ch?

82ch는 AI 에이전트와 외부 도구 간의 통신 프로토콜인 **MCP(Model Context Protocol)**의 보안을 강화하는 통합 프레임워크입니다. MCP 통신을 실시간으로 모니터링하고, 다양한 보안 위협을 탐지하여 AI 시스템의 안전성을 보장합니다.

## Features

### Real-time Security Monitoring
- HTTP+SSE, STDIO 등 다양한 MCP 전송 프로토콜 지원
- 실시간 요청/응답 인터셉션 및 검증
- 보안 이벤트의 자동 로깅 및 분석

### Multi-Engine Threat Detection

#### Signature-based Detection
- **Sensitive File Detector**: 민감한 파일 접근 탐지 (.env, credentials 등)
- **Command Injection Detector**: 명령어 주입 공격 패턴 탐지
- **File System Exposure Detector**: 파일 시스템 노출 위험 모니터링

#### LLM-based Semantic Analysis
- **Tools Poisoning Detector**: AI를 활용한 의미적 불일치 탐지
  - 도구 명세와 실제 사용 간의 semantic gap 분석
  - 4가지 차원의 정밀 스코어링 (Domain, Operation, Argument, Consistency)
  - 자동 심각도 분류 (none/low/medium/high)

### Desktop UI Dashboard
- React 기반 실시간 모니터링 대시보드
- 탐지 결과 시각화 및 상세 분석
- 이벤트 히스토리 조회 및 필터링

## Projects

### [mcp-dandan](https://github.com/82ch/mcp-dandan)
메인 프로젝트 - MCP Security Framework의 전체 구현체

**Key Components:**
- Observer: MCP 프록시 및 트래픽 인터셉터
- Engine: 다중 탐지 엔진 시스템
- EventHub: 중앙 이벤트 라우터
- Desktop UI: React 기반 모니터링 대시보드

## Documentation

자세한 문서는 각 프로젝트의 README를 참조하세요:
- [MCP-DANDAN Documentation](https://github.com/82ch/mcp-dandan/blob/main/README.md)

## License

각 프로젝트의 라이선스를 따릅니다.

---

<p align="center">
  Built with by 82ch Team
</p>
