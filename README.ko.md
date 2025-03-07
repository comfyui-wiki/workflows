# ComfyUI Wiki 워크플로우
🌐 다국어 지원: [English](README.md) | [中文](README.zh.md) | [Español](README.es.md) | [Français](README.fr.md) | [日本語](README.ja.md)

이 저장소는 [ComfyUI-Wiki.com](https://comfyui-wiki.com/ko)의 모든 워크플로우 파일을 포함합니다. 각 워크플로우에는 미리보기 이미지(메타데이터 포함)와 JSON 파일이 함께 제공되며, 두 형식 모두 ComfyUI로 직접 드래그하여 로드할 수 있습니다.

## 시작하기

### 필수 조건
- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) 설치 완료
- 새로 설치하는 경우 [ComfyUI Wiki 설치 가이드](https://comfyui-wiki.com/ko/install/install-comfyui)를 따르세요

## 누락된 모델 처리
워크플로우 로드 시 ComfyUI는 자동으로 누락된 모델을 감지하고 알림을 표시합니다:
![누락된 모델 알림](/readme_images/missing_models.png)

### ComfyUI 데스크톱 사용자
1. 알림 대화상자에서 다운로드 버튼 클릭
2. 중요 사항:
   - [CivitAI](https://civitai.com) 및 [Hugging Face](https://huggingface.co/) 모델만 지원
   - 해당 플랫폼에 대한 네트워크 접근 확인 필요
   - 지원되지 않는 파일 형식(예: .pth)은 별도 안내 제공

### 기타 버전(포터블/수동 설치)
1. 브라우저에 저장된 다운로드 파일 확인
2. `ComfyUI/models/` 하위 디렉토리에 수동으로 이동

설정 후 예시 구조:
```bash
ComfyUI/
└── models/
    ├── checkpoints/
    │   └── dreamshaper_8.safetensors
    └── loras/
        ├── blindbox_ViMix.safetensors
        └── MoXinV1.safetensors
```
> 파일 이동 후 ComfyUI 재시작/새로고침 필요

## 누락된 노드 해결
![누락된 노드 알림](/readme_images/missing_node_types.png)

### 문제 해결 단계
1. **핵심 노드 누락**: [ComfyUI 업데이트](https://comfyui-wiki.com/ko/tutorial/basic/how-to-update-comfyui)
2. **커스텀 노드 누락**: ComfyUI Manager 통해 설치

### 설치 가이드
![ComfyUI Manager 인터페이스](/readme_images/comfyui_manager.png)
1. ComfyUI에서 `Manager` 버튼 클릭
2. `Install missing nodes` 선택
3. 대화상자에서 `Install` 클릭

![노드 설치 데모](/readme_images/install_missing_nodes.jpg)

### 중요 사항
- 자동 설치를 위해 GitHub 접근 필요
- 제한된 네트워크 환경을 위한 수동 설치 가이드: [커스텀 노드 설치](https://comfyui-wiki.com/ko/install/install-custom-nodes)
- 개별 워크플로우별 노드 정보는 해당 README 파일에서 확인 가능

> 모든 워크플로우는 보안 검사를 거쳤습니다. 모델은 공식 출처에서만 획득하세요. 