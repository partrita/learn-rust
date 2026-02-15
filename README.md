# 슈퍼이지러스트 (Learn Rust)

데이브 매클라우드(Dave MacLeod)의 "Easy Rust"를 읽고 학습한 내용을 정리한 Quarto 기반의 러스트(Rust) 학습 노트입니다.

## 주요 특징

- **대화형 코드 실행**: `evcxr`(Rust Jupyter Kernel)을 사용하여 문서 내에서 직접 러스트 코드를 실행하고 결과를 확인할 수 있습니다.
- **의존성 관리**: `pixi`를 사용하여 Rust 도구 체인, Quarto 및 기타 의존성을 일관되게 관리합니다.
- **자동 배포**: GitHub Actions를 통해 변경 사항이 푸시될 때마다 GitHub Pages로 자동 배포됩니다.

## 프로젝트 구조

- `mybook/`: Quarto 책의 소스 코드(.qmd 파일들)가 포함되어 있습니다.
- `pixi.toml`: 프로젝트의 의존성 및 태스크 정의 파일입니다.
- `.github/workflows/`: GitHub Actions 배포 워크플로우 정의 파일이 포함되어 있습니다.

## 로컬 개발 설정

이 프로젝트를 로컬에서 실행하려면 [pixi](https://pixi.sh/)가 설치되어 있어야 합니다.

1. **의존성 설치 및 커널 등록**:
   ```bash
   pixi run install
   ```

2. **Quarto 책 렌더링**:
   ```bash
   pixi run render
   ```

3. **미리 보기 (Preview)**:
   ```bash
   pixi run quarto preview mybook
   ```

## 기술 스택

- **Language**: Rust
- **Documentation**: Quarto (Book type)
- **Interactive Engine**: Jupyter (evcxr 커널)
- **Dependency Manager**: Pixi
- **Deployment**: GitHub Actions & GitHub Pages
