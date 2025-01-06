Azure-pyk4a

    https://github.com/etiennedub/pyk4a/
 

# 1. Installization

### 1.1 Azure Kinect SDK
       
    https://learn.microsoft.com/en-us/previous-versions/azure/kinect-dk/sensor-sdk-download


### 1.2 Azure Kinect Body Tracking SDK (선택 사항)
   
- Body Tracking이 필요한 경우

      https://learn.microsoft.com/en-us/previous-versions/azure/kinect-dk/body-sdk-download


### 1.3 Visual Studio 설치
   
- Visual Studio 2022 또는 2019 설치

- 설치 시 C++ 데스크톱 개발 워크로드와 MSVC 빌드 도구 선택.

- 필수로 깔아야하는 것: C++ 데스크톱 개발, 개별 구성 요소(CMake, Windows 10 SDK)

      https://visualstudio.microsoft.com/ko/vs/


### 1.4 Python 설치
   
- Python 3.8 ~ 3.10 버전 중 하나를 설치합니다.

- 설치 중 PATH에 추가(Add to PATH) 옵션 활성화 필수.

-------------

# 2. 필수 환경변수 설정
### 2.1 Azure Kinect SDK 환경변수 추가:
  
- K4A_PLUGIN_PATH:
 
      C:\Program Files\Azure Kinect SDK v1.4.1\sdk\windows-desktop\amd64\release\bin
  
- PATH: 위 SDK 경로를 포함.

### 환경변수 설정 방법:

- "시작 메뉴" → "환경 변수 편집" 검색 → "환경 변수" 클릭

- 시스템 변수에서 PATH 항목 편집 → 위 경로 추가

- 새 시스템 변수로 K4A_PLUGIN_PATH 생성 후 값 추가

-------------
# 3. pyk4a 설치
### 3.1 의존성 설치

- 최신 pip, setuptools, wheel 업데이트
 
      pip install --upgrade pip setuptools wheel
  
- cmake 및 pybind11 설치

    pip install cmake pybind11

### 3.2 pyk4a 설치

pyk4a는 PyPI에서 설치하거나 Git에서 소스를 직접 빌드해 설치할 수 있다.

- 방법1. PyPI에서 설치(cmd)

      pip install pyk4a

- 방법2. 소스에서 설치
 
-- 1. GitHub에서 pyk4a 저장소를 클론:
      git clone https://github.com/etiennedub/pyk4a.git

      cd pyk4a

-- 2. 소스에서 설치
    pip install .



