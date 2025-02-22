---
further_reading:
- link: https://www.datadoghq.com/blog/dashboard-sharing/
  tag: 블로그
  text: 조직 외부인과 안전하게 대시보드 공유하기
- link: https://www.datadoghq.com/blog/template-variable-associated-values/
  tag: 블로그
  text: 관련된 템플릿 변수를 사용해 대시보드 정리하기
- link: https://learn.datadoghq.com/courses/building-better-dashboards
  tag: 학습 센터
  text: 더 나은 대시보드 빌드
- link: /dashboards/
  tag: 설명서
  text: 대시보드 기본
- link: /notebooks/
  tag: 설명서
  text: 노트북으로 데이터와 관련한 맥락 추가하기
- link: /monitors/
  tag: 설명서
  text: 모니터링, SLO, 알림, 다운타임, 인시던트
- link: https://dtdg.co/fe
  tag: 기반 활성화
  text: 대시보드를 통해 보다 나은 시각화를 위한 대화형 세션 참여
title: 대시보드 시작하기
---

{{< learning-center-callout header="Join an enablement webinar session" hide_image="true" btn_title="Sign Up" btn_url="https://www.datadoghq.com/technical-enablement/sessions/?tags.topics-0=Dashboarding">}}
  파운데이션 활성화 세션을 살펴보고 등록하세요. 라이브러리의 시각화 및 드래그 앤 드롭 방식의 대시보드 빌더를 사용하여 대시보드 을 사용자 지정하는 방법을 알아보세요. 보고서, 공개 URL 및 노트북 을 통해 이해관계자들과 데이터를 공유하여 팀의 성공을 지원하세요.
{{< /learning-center-callout >}}

## 개요

대시보드를 시작하는 핵심은 스스로에게 정기적으로 어떤 종류의 질문을 하는지를 파악하는 것입니다. 고객이 직면하는 일반적인 문제는 무엇인가요? 문제가 발생하면 어떤 질문이 해결책을 찾는 데 도움을 주나요?

좋은 대시보드를 만드는 것은 이러한 질문에 대한 답을 수면 위로 끌어올리는 것입니다. 또한 모든 생각을 같은 대시보드에 담지 않는 것도 중요합니다. 서로 다른 문제를 정확히 파악하기 위해 별도의 대시보드를 만들면 빠르게 답을 찾을 수 있습니다.

이 가이드는 대시보드를 만드는 방법을 안내합니다. 이러한 기본 대시보드 을 통해 팀 토론을 활성화하고 문제 해결 속도를 높일 수 있습니다.

## 사전 필수 조건

아직 만들지 않았다면 [Datadog 계정][1]을 만드세요. 호스트 및 호스트에서 실행되는 통합에서 에이전트를 설치합니다.

## 계획

생성 중인 대시보드의 목적을 결정합니다. 대시보드를 통해 여러분과 팀원들이 올바른 업무에 집중할 수 있습니다. 팀 대시보드는 높은 우선 순위 작업, 주의 사항 및 성공 대상에 대해 알려줍니다. 사람들이 가장 자주 찾는 정보로 팀 대시보드를 여러 가지로 만들어 보세요. SLO 및 SLI 세부 정보로 훌륭한 팀 대시보드를 마들어 보세요.

대시보드가 실시간 데이터에 연결되면 상사나 매니저와 대화할 때 큰 도움이 됩니다. 적절한 _관리직 대시보드_가 구성되면 작업의 중요도와 서비스 실행 비용, 목표의 진척 상황, SLO 달성률, 확장 효과의 측정 결과 등을 명확하게 파악할 수 있습니다. 관리직 대시보드에서 방금 언급된 항목에 대한 답변을 개략적으로 표시하고, 그 답을 비교 분석하기 위해 여러 대시보드를 상호 연결했을 때 가장 효과적입니다.

대시보드는 빈번하게 발생하는 문제를 추적하고 수정할 때도 도움이 됩니다. _트러블슈팅 대시보드_는 먼저 알고 있는 정보를 메모하는 단계에서 시작하여, 서서히 다양한 발견 사항을 추가하여 정보를 기록하는 장소로 기능합니다. 예를 들면 다른 대시보드나 보기 화면에서 문제를 알려주는 그래프나 위젯을 살펴보는 단계에서 시작하여, 이 정보를 바탕으로 세밀하게 문제를 분석하고 해결책을 찾을 수 있습니다.

## 바로 사용 가능한 대시보드 살펴보기

Datadog는 바로 사용 가능한 기능 및 통합용 대시보드를 다양하게 지원합니다. 모니터링하는 인프라스트럭처가 있는 경우 Datadog의 바로 사용 가능한 대시보드를 살펴보세요.

1. Datadog에서 [대시보드 목록 페이지][2]로 이동한 다음 추가한 통합 이름을 검색합니다. 예를 들어 `Redis` 또는 `RUM` 등 사용하는 기능이 될 수 있습니다.
2. 검색 에서 *사전 설정*으로 표시된 대시보드 의 결과를 찾아보고 그래프 중 적어도 일부에 원하는 답이 표시되어 있는지 확인합니다.
3. 즉시 사용 가능한 대시보드의 제목 드롭다운 메뉴에서 링크를 탐색하여 자세한 활용 방법을 찾아보세요.

## 다른 대시보드를 재사용하는 단계부터 시작하기

대시보드를 시작하는 일반적인 방법은 이미 사용 중인 유사한 대시보드를 발견하여 필요에 맞게 조정하는 것입니다. 대시보드에서 답변하고 싶은 많은 질문에 대한 답변을 제공하는 대시보드를 찾으면 됩니다. 

1. 대시보드를 열고 설정 작업 메뉴(오른쪽의 설정 버튼)에서 **Clone dashboard**를 선택하여 복제합니다. 그러면 연결되지 않은 대시보드 복사본이 생성되므로 새 복사본에서 변경한 내용은 소스 위젯에 영향을 주지 않습니다.
  {{< img src="getting_started/dashboards/configure_clone_dashboard.png" alt="설정 작업 메뉴의 대시보드 옵션 복제" style="width:100%;" >}}
2. 복사본을 열고 **Edit widgets**를 클릭해 내용을 수정하세요.
3. 위젯의 설정 메뉴에서 **Delete**를 눌러 필요하지 않은 위젯을 삭제합니다.
4. 필요에 맞게 항목을 이동하세요. 그룹 및 개인 위젯 은 대시보드에서 새로운 위치에 끌어다 놓을 수 있습니다.
5. 다른 대시보드에서 위젯 위에 커서를 올린 다음 `Command + C`(윈도우즈(Windows)의 경우에는 `Ctrl + C`)를 눌러 위젯을 복사하세요. 대시보드를 열고 `Command + V`(윈도우즈의 경우에는 `Ctrl + V`)를 입력해 붙여넣습니다.
5. 많은 Datadog 보기에서 제공하는 ** 대시보드로 내보내기** 옵션을 사용하여 표시되는 데이터를 내보냅니다. 예를 들어, 로그 탐색기 및 로그 분석 보기에는 로그 목록 및 메트릭을 대시보드로 내보내는 공유 옵션이 있습니다.

## 메트릭 자세히 알아보기

통합을 통해 Datadog는 인프라스트럭처 및 애플리케이션에서 [메트릭][3]을 수집합니다. 수집된 메트릭은 통합의 README 파일에 기록됩니다. [메트릭 탐색기][4]에서 메트릭을 발견했거나 대시보드에서 생성하여 해당 메트릭이 어떤 메트릭인지 알아보려면 통합 설명서에서 찾아보세요.

예를 들어, `aws.s3.first_byte_latency` 메트릭의 시간 그래프를 보고 있다고 가정합니다. Amazon S3 통합 README의 [수집된 데이터][5] 섹션으로 이동하여 이 설명을 확인합니다. `The average per-request time from the complete request being received by a bucket to when the response starts to be returned. Shown as millisecond.`

## 위젯 추가 및 표시 방법 설정

대시보드에 몇몇 메트릭을 추가하한 후, 다양한 [위젯 유형][6], [쿼리][8] 및 [집계 접근 방식][9]으로 실험하여 질문에 대한 최상의 답을 제공할 수 있는 방법으로 데이터를 표시하세요.

템플릿 변수를 지정하여 여러 시나리오에 대한 답변을 단일 대시보드에서 확인할 수 있습니다. 예를 들어, 대시보드 변수 드롭다운에서 아용자가 선택한 특정 데이터 센터 지역 또는 모든 데이터 센터의 지연 메트릭을 표시하는 시간 그래프를 생성할 수 있습니다. 자세한 정보는 [템플릿 변수][10]를 참조하세요.

Y축 범위, 색상 또는 레전드를 조정하여 그래프를 더 쉽게 읽을 수 있도록 만들 수 있습니다. 또는 마커나 이벤트 오버레이를 추가할 수도 있습니다. [시계열][12] 및 [기타 위젯][6]을 커스터마이즈하고 세분화할 수 있는 모든 방법은 [대시보드 설명서][11]를 참조하세요.

이러한 기법에 대한 자세한 설명과 예시는 온라인 학습 과정 [더 나은 대시보드 빌드][13]에 등록하세요.

## 기타 위젯 사용해보기

메트릭의 시계열 그래프도 유용하지만 대시보드에는 중요한 정보를 전달하기 위해 다양한 유형의 위젯 를 포함할 수 있습니다. 다음을 사용해 보세요.

 - **경고값과 점검 상태**: 숫자를 큰 빨강, 노랑, 초록색으로 표시하여 작업이 순조로운지, 문제가 발생했는지 여부를 쉽게 알 수 있습니다.
 - **히트맵**: 직관적인 색상 강도 그래프를 사용하여 여러 태그에 걸쳐 복잡한 메트릭-인프라스트럭처 관계를 표시합니다.
   {{< img src="getting_started/dashboards/heatmap_widget.png" alt="Heatmap 예시" >}}
 - **iFrames, 서식 있는 텍스트 및 이미지**: 대시보드 콘텐츠에 대한 설명 및 추가 리소스 제공을 위해 웹사이트와 유사한 세부 정보를 얼마든지 표시할 수 있습니다.
 - **표**: 메트릭 목록을 태그 키별로 그룹화하여 표시합니다.
 - **상위 목록**: 예를 들어 가장 용량이 적은 호스트, 가장 많은 오류가 발생하는 서비스, 404를 가장 많이 반환하는 URL 등을 표시할 수 있습니다.
 - **호스트 맵**: 호스트 통합 또는 서비스 상태를 색상별로 나타내는 등, 인프라스트럭처의 호스트를 다이어그램으로 표시합니다.
 - **서비스 수준 목표(SLO)**: SLO 위젯을 통해 목표 대비 팀 성과를 표시하고 추가 위젯을 그룹화하여 SLI 메트릭에 대한 상세 정보를 표시할 수 있습니다.
 - **분포**: 컨테이너화된 환경에서 발생하는 다양한 이벤트 수와 각 서비스의 주요 오류 개수, 웹사이트 플로우(2페이지, 3페이지, 4페이지를 연 사용자 수), 레이턴시의 백분위 버킷 등을 히스토그램으로 보여줍니다.

이러한 그래프를 설정하는 방법에 대한 자세한 정보와 예시는 [위젯][6]을 참조하세요.

## 정렬, 연결, 분석

대시보드를 이용하는 작업이나 대화의 흐름에 맞게 그래프를 옮겨보세요. 위젯은 드래그 앤 드롭으로 배치할 수 있습니다. 스크린보드에서는 프리 텍스트(Free Text) 위젯을 사용하여 머리말 아래 섹션을 정리할 수 있습니다. 타임보드에서는 여러 위젯을 포괄하는 그룹(Group) 위젯을 추가하고, 대시보드를 볼 때 접을 수 있습니다.

대시보드에서 타겟 URL로 연결되는 링크를 생성하는 방법은 두 가지입니다.

 - 링크 등의 마크다운 서식 설정 텍스트를 포함할 수 있는 노트 & 링크(Notes and Links) 위젯을 추가합니다. 위젯 편집기에는 마크다운 서식 설정 팁이 안내되어 있습니다.
 - 위젯의 설정(기어) 메뉴에서 커스텀 링크를 생성합니다. 커스텀 링크는 변수와 템플릿 변수를 보간(interpolate )합니다. 따라서 사용자가 선택한 콘텐츠에 따라 링크가 달라지며, 데이터를 분석하거나 수정하기 위해 적절한 위치로 이동시킬 수 있습니다.
     {{< img src="getting_started/dashboards/opening_custom_link.mp4" alt="커스텀 링크 열기" video=true >}}

## 다음 단계

### Datadog 사이트 외부로 대시보드 공유하기

대시보드 내보내기 메뉴에서 **공용 URL 설정**을 클릭하여 큰 화면에 공유하려거나 Datadog 계정이 없는 사람들에게 공유할 URL을 생성하세요. 자세한 정보는 [대시보드 공유하기][14]를 참조하세요.

[Slack 통합][15]을 사용해 팀과의 커뮤니케이션을 통합하여 대시보드와 기타 Datadog 기능을 가져오세요. 모니터와 인시던트 등을 Slack 채널로 가져올 수 있습니다.

### 여러 대시보드를 빠르게 만들기

모든 대시보드는 JSON으로 표현됩니다. 따라서 설정 메뉴에서 복사하거나 내보낼 수 있습니다. 대시보드의 각 위젯도 JSON 정의를 사용하며, 위젯 편집기(연필 아이콘)를 열고 **Graph your data** 아래 JSON 탭을 클릭하여 확인하고 편집할 수 있습니다.

모든 위젯과 대시보드가 JSON으로 표시되므로 프로그래밍 방식으로 [대시보드 API]를 사용해 생성할 수 있습니다. 그러므로 팀이 새로운 프로젝트를 시작하거나, 인시던트가 있을 때 또는 SLP를 규격화할 때 등 대시보드를 생성해야 할 때 유용합니다.

### Datadog 모바일 앱에서 대시보드 보기

[Apple 앱 스토어][18] 및 [Google Play 스토어][19]에서 이용 가능한 [Datadog 모바일 앱][17]을 사용해 모바일 장치에서 대시보드를 봅니다.

모바일 앱을 사용하면 Datadog 조직에서 액세스 권한이 있는 모든 대시보드를 보고 검색할 수 있으며, Datadog 웹 앱에서 사용하는 것과 동일한 템플릿 변수를 사용하여 필터링할 수 있습니다.

{{< img src="dashboards/dashboards-list-mobile.png" style="width:100%; background:none; border:none; box-shadow:none;" alt="iOS와 Android의 대시보드">}}

## 참고 자료

{{< partial name="whats-next/whats-next.html" >}}

[1]: https://app.datadoghq.com/
[2]: https://app.datadoghq.com/dashboard/lists
[3]: /ko/metrics/introduction/
[4]: /ko/metrics/explorer/
[5]: /ko/integrations/amazon_s3/#data-collected
[6]: /ko/dashboards/widgets/
[7]: /ko/dashboards/querying/
[8]: /ko/dashboards/functions/
[9]: /ko/metrics/distributions/
[10]: /ko/dashboards/template_variables/
[11]: /ko/dashboards/
[12]: /ko/dashboards/widgets/timeseries/
[13]: https://learn.datadoghq.com/courses/building-better-dashboards/
[14]: /ko/dashboards/sharing/
[15]: /ko/integrations/slack/
[16]: /ko/api/v1/dashboards/
[17]: /ko/mobile/
[18]: https://apps.apple.com/app/datadog/id1391380318
[19]: https://play.google.com/store/apps/details?id=com.datadog.app