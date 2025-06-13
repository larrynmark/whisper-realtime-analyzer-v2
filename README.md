# Whisper Realtime Analyzer

실시간 음성 인식과 AI 분석을 통한 대화 시각화 도구

## 🎯 주요 기능

- **실시간 STT**: Whisper 엔진을 사용한 고정밀 음성 인식
- **AI 분석**: OpenAI GPT를 활용한 키워드 추출 및 주제 분석
- **실시간 시각화**: 키워드 클라우드와 주제 변화 시각화
- **유연한 설정**: 분석 주기, API 설정 등 사용자 맞춤 설정
- **크로스 오디오**: 마이크 및 시스템 오디오 캡처 지원

## 🛠 기술 스택

- **Frontend**: React 18 + TypeScript + Material-UI
- **Desktop**: Electron
- **STT**: faster-whisper
- **AI**: OpenAI GPT API
- **시각화**: D3.js, Recharts
- **상태 관리**: Zustand

## 📋 시스템 요구사항

- **macOS**: 11.0 이상
- **Node.js**: 16.0 이상
- **Python**: 3.8 이상 (faster-whisper 용)
- **RAM**: 최소 8GB 권장
- **Storage**: 2GB 이상 여유 공간

## 🚀 설치 및 실행

### 1. 의존성 설치
```bash
npm install
```

### 2. 개발 모드 실행
```bash
npm run dev
```

### 3. 프로덕션 빌드
```bash
npm run build
npm run dist
```

## ⚙️ 설정

### OpenAI API 설정
1. 애플리케이션 실행 후 설정 메뉴 진입
2. OpenAI API Key 입력
3. Base URL 설정 (프록시 사용 시)
4. 분석 주기 설정 (기본: 60초)

### 오디오 설정
- 마이크 권한 허용 필요
- 시스템 오디오 캡처 시 추가 권한 필요

## 📊 사용법

1. **음성 인식 시작**: 녹음 버튼 클릭
2. **실시간 분석**: 설정한 주기마다 자동 분석
3. **시각화 확인**: 키워드 클라우드 및 주제 변화 확인
4. **설정 조정**: 필요시 분석 주기 및 API 설정 변경

## 🔧 개발 가이드

### 프로젝트 구조
```
src/
├── main/           # Electron 메인 프로세스
├── renderer/       # React 렌더러 프로세스  
└── shared/         # 공통 타입 및 인터페이스
```

### 주요 컴포넌트
- **AudioCapture**: 오디오 스트림 캡처
- **WhisperSTT**: 음성 인식 처리
- **OpenAIAnalyzer**: 텍스트 분석
- **Visualizer**: 실시간 시각화

### 개발 명령어
```bash
npm run dev          # 개발 모드
npm run build        # 프로덕션 빌드
npm run lint         # 코드 검사
npm run test         # 테스트 실행
```

## 📝 라이선스

MIT License

## 🤝 기여하기

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📞 지원

이슈가 있으시면 GitHub Issues를 통해 문의해주세요.