## Code 정리 작업
* MapActivty
	- View - MapActivity 는 view 로서의 기능만
	- ViewModel - AAC ViewModel, LiveData 적용하여 Activity life cycle 대응, 유지보수 용이
	- Model - ViewModel(Live data) 과 ROOM 에서 사용하는 데이터를 Data repository 에 통합하여 비행경로, 사용자 정보 등 관리

* 메뉴 구성 개선
	- 진입 화면에서 네트워크 선택 버튼들 없애기
	- 진입 화면에서 기체가 연결되어 있는지 여부 간단한 아이콘으로 표시
	- 중간고도, 이륙고도, 방제폭, 액제선택 버튼, 맨 오른쪽 버튼그룹과 GPX 경로 보기 버튼들은 따로 설정 메뉴 뷰로 빼기(농경지 관리 메뉴 등)
	- 버튼 아이콘 일관성 개선

* MapActivity 내에 사용된 안내용 문자열 string resource 파일로 분리



#
### 기타 기능 추가 및 안정화
    - GPX 로그 다운로드 기능
    - 다각형 자동 방제 (마커 수정 포함)
    - 조종기에 마커찍는 채널 할당(AB 자동방제용)
    - 음성안내, 효과음
    - 카피비행 최적화
    - 메뉴얼 앱에 연동 (각 기능별 도움말)