# upgraded 폴더 구조 설명

`upgraded` 폴더는 레거시(`legacy`) 폴더의 전체 파일 및 디렉터리 구조를 복사한 디렉터리입니다. 이 폴더는 Python 2.5 기반의 레거시 프로젝트를 최신 Python 버전으로 업그레이드하는 작업 공간으로 사용됩니다.

## 주요 하위 폴더 및 파일

- `MANIFEST.in`, `README.rst`, `setup.py`, `distribute_setup.py`, `distribute-0.6.10.tar.gz`: 프로젝트 메타 정보 및 설치 관련 파일
- `docs/`: Sphinx 기반 문서화 디렉터리
  - `build/`: 빌드된 문서(HTML, doctree 등)
  - `source/`: 문서 소스(rst, conf.py 등)
- `guachi/`: 주요 Python 패키지 소스 코드
  - `__init__.py`, `config.py`, `database.py`: 핵심 모듈
  - `tests/`: 단위 테스트 및 통합 테스트
- `guachi.egg-info/`: 패키징 정보(egg metadata)

이 구조는 레거시 프로젝트의 모든 코드, 문서, 테스트, 패키징 정보를 포함하며, 업그레이드 작업을 위한 출발점이 됩니다.