# ComfyUI Wiki 워크플로우
🌐 다국어 지원: [English](README.md) | [中文](README.zh.md) | [Español](README.es.md) | [Français](README.fr.md) | [日本語](README.ja.md)

이 저장소는 [ComfyUI-Wiki.com](https://comfyui-wiki.com/ko)의 모든 워크플로우 파일을 포함하고 있습니다. 각 워크플로우에는 미리보기 이미지(메타데이터 포함)와 JSON 파일이 함께 제공되며, ComfyUI로 직접 드래그 앤 드롭하여 로드할 수 있습니다.

## 시작하기

해당 모델을 다운로드한 후 ComfyUI에 드래그하면 워크플로우를 로드할 수 있습니다. 각 워크플로우 파일에는 모델 다운로드 정보를 기록한 readme.md 파일이 포함되어 있습니다.

### 시스템 요구사항
- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) 설치 완료
- 신규 사용자는 [ComfyUI Wiki 설치 가이드](https://comfyui-wiki.com/ko/install/install-comfyui) 참조

## 누락된 모델 처리
워크플로우 로드 시 ComfyUI가 자동으로 누락된 모델을 감지합니다:
![누락된 모델 알림](/readme_images/missing_models.png)

### ComfyUI 데스크톱 버전 사용자
1. 팝업 창의 다운로드 버튼 클릭
2. 주의사항:
   - 현재 CivitAI와 Hugging Face의 모델만 지원
   - 해당 플랫폼 접속 가능한 네트워크 환경 확인
   - .pth 등 지원하지 않는 형식 파일은 readme.md에 수동 다운로드 안내

### 기타 버전 사용자

1. `Download` 버튼 클릭 후 브라우저에서 다운로드 완료
2. 파일을 `ComfyUI/models/` 디렉토리로 이동

예시 디렉토리 구조:
```bash
ComfyUI/
└── models/
    ├── checkpoints/
    │   └── dreamshaper_8.safetensors
    └── loras/
        ├── blindbox_ViMix.safetensors
        └── MoXinV1.safetensors
```
> 파일 이동 후 재시작/화면 새로고침 필요

## 누락된 노드 처리
![누락된 노드 알림](/readme_images/missing_node_types.png)

### 해결 방법
1. **코어 노드 누락**: [ComfyUI 업데이트](https://comfyui-wiki.com/ko/tutorial/basic/how-to-update-comfyui)
2. **커스텀 노드 누락**: ComfyUI Manager로 설치

### ComfyUI Manager 커스텀 노드 설치 가이드
![ComfyUI Manager 인터페이스](/readme_images/comfyui_manager.png)
1. `Manager` 버튼 클릭
2. `Install missing nodes` 선택
3. 팝업 창에서 `Install` 클릭

![노드 설치 예시](/readme_images/install_missing_nodes.jpg)

### 중요 공지
- 자동 노드 설치 기능은 GitHub 접속 가능한 네트워크 환경 필요
- 제한된 네트워크 사용자는 [수동 설치 가이드](https://comfyui-wiki.com/ko/install/install-custom-nodes) 참조
- 각 워크플로우의 README 파일에 커스텀 노드 URL 제공


제작: [@ComfyUI-Wiki](https://github.com/comfyui-wiki) | [ComfyUI-Wiki](https://comfyui-wiki.com/ko)