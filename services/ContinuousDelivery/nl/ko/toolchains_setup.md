---

copyright:
  years: 2016

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 도구 체인 시작하기
{: #toolchains-setup}

마지막 업데이트 날짜: 2016년 4월 28일
{: .last-updated}  

두 가지 방법으로 도구 체인을 작성할 수 있습니다. 즉, 템플리트를 사용하여 도구 체인을 작성하거나 앱에서 도구 체인을 작성할 수 있습니다. 사용하는 템플리트 또는 도구 체인에 따라 도구 체인에 앱 스타터 코드로 채워지는 GitHub 저장소(repo)와 사전 구성된 Delivery Pipeline이 포함될 수 있습니다. 도구 체인의 GitHub 저장소에 변경사항을 푸시하면 Delivery Pipeline이 자동으로 앱을 빌드하고 {{site.data.keyword.Bluemix}}에 배치합니다.
{: shortdesc}  

**중요**: 이 기능은 시범 기능입니다. 도구 체인은 안정적이지 않을 수 있으며 이전 버전과 호환되지 않도록 변경될 수 있습니다. 프로덕션 환경에서 도구 체인을 사용하지 않는 것이 좋습니다. 도구 체인을 사용하려면 일회성 [액세스 요청](https://new-console.ng.bluemix.net/devops?cm_mmc=IBMBluemixGarageMethod-_-MethodSite-_-10-19-15::12-31-18-_-toolchains-welcome-page){: new_window}을 작성해야 합니다. 달라스 지역에서만 도구 체인을 사용할 수 있습니다. 

##템플리트에서 도구 체인 작성   
{: #creating_a_toolchain_from_a_template}

도구 체인에 대한 액세스 요청이 승인되면 템플리트를 시작점으로 사용하여 특정 도구 통합 세트를 포함하는 도구 체인을 작성할 수 있습니다. 

1. DevOps 대시보드의 **도구 체인** 탭에서 **도구 체인 작성**을 클릭하여 첫 번째 도구 체인을 작성하십시오. 도구 체인이 이미 있는 경우에는 추가 단추(+)를 클릭하여 다른 도구 체인을 작성하십시오. 
1. 도구 체인 템플리트를 클릭하십시오. 예를 들어, 온라인 상점 샘플을 사용하여 도구 체인을 작성하려면 **마이크로서비스용 클라우드 고유 도구 체인**을 클릭하십시오.  
1. 도구 체인 작성 페이지에서 작성하려는 도구 체인의 다이어그램을 검토하십시오. 다이어그램은 도구 체인에서 해당 라이프사이클 단계(Phase)에 있는 각 도구 통합을 보여줍니다. 다음 이미지의 다이어그램을 예로 들 수 있습니다. 도구 체인을 작성할 때 다이어그램은 도구 체인의 일부인 각 도구 통합을 표시합니다.
![도구 체인 다이어그램](images/toolchain_diagram.png)

1. 도구 체인 설정에 대한 기본 정보를 검토하십시오. 도구 체인의 이름은 {{site.data.keyword.Bluemix}}에서 해당 도구 체인을 식별합니다. 해당 이름을 가진 도구 체인이 이미 있거나 다른 이름을 사용하려는 경우에는 도구 체인의 이름을 변경하십시오.   
1. 도구 통합을 구성하기 전에 도구 체인을 작성하려면 **작성**을 클릭하고 도구 통합 없이 도구 체인을 작성하려 함을 확인하십시오. 계속해서 도구 체인을 자동으로 설정하는 단계에 대해 설명하는 [도구 체인 작성](#creating_a_toolchain) 섹션을 진행하십시오.   
1. 도구 체인을 작성하기 전에 도구 통합을 구성하려면 구성 가능한 통합 섹션에서 구성하려는 각 도구 통합을 선택하십시오. 도구 통합 구성에 대한 정보는 [도구 통합 구성](../toolchains/toolchains_integrations.html){: new_window}의 내용을 참조하십시오. 

##앱에서 도구 체인 작성
{: #creating_a_toolchain_from_an_app}

도구 체인에 대한 액세스 요청이 승인되면 앱에서 도구 체인을 작성할 수 있습니다. 도구 체인은 지속적인 개발, 배치, 모니터링 등을 지원할 수 있으며 앱과 연관됩니다. 각 앱을 도구 체인과 연관시킬 수 있습니다. 도구 체인의 GitHub 저장소에 변경사항을 푸시하면 파이프라인이 자동으로 앱을 빌드하고 배치합니다.  

1. 앱 개요 페이지의 Continuous Delivery 타일에서 **도구 체인 추가**를 클릭하십시오. 또는 Bluemix Classic Experience에서 **GIT 추가**를 클릭하십시오. 앱 스타터 코드로 채워지는 새 GitHub 저장소에서 Continuous Delivery가 가능하도록 앱이 구성됩니다. 
1. 도구 체인 작성 페이지에서 작성하려는 도구 체인의 다이어그램을 검토하십시오. 다이어그램은 도구 체인에서 해당 라이프사이클 단계(Phase)에 있는 각 도구 통합을 보여줍니다. 
1. 도구 체인 설정에 대한 기본 정보를 검토하십시오. 도구 체인의 이름은 {{site.data.keyword.Bluemix}}에서 해당 도구 체인을 식별합니다. 해당 이름을 가진 도구 체인이 이미 있거나 다른 이름을 사용하려는 경우에는 도구 체인의 이름을 변경하십시오. 
1. 구성 가능한 통합 섹션에서 도구 체인에 구성하려는 각 도구 통합을 선택하십시오. 도구 통합 구성에 대한 정보는 [도구 통합 구성](../toolchains/toolchains_integrations.html){: new_window}의 내용을 참조하십시오.

## 도구 체인 설정
{: #setting_up_a_toolchain}

도구 체인을 아직 작성하지 않은 경우에는 **작성**을 클릭하십시오. 다음과 같은 여러 단계가 자동으로 실행되어 도구 체인을 설정합니다. 

 * 도구 체인이 작성됩니다. 
 * Delivery Pipeline 도구 통합을 구성한 경우 파이프라인이 트리거됩니다. 
 * Sauce Labs 도구 통합을 구성한 경우, 파이프라인에 작업을 추가하고 테스트를 실행하도록 Sauce Labs 통합이 구성됩니다. 
 * PagerDuty 도구 통합을 구성한 경우, Slack에서 구성한 채널에 알림을 전송하도록 PagerDuty 통합이 구성됩니다. 이러한 알림은 문제점이 발생한 시점을 표시합니다. 
 * Slack 도구 통합을 구성한 경우, Slack에서 구성한 채널에 알림을 전송하도록 Slack 통합이 구성됩니다. 이러한 알림은 배치의 진행상태(예: `프로젝트 XYZ와 연결됨`, `파이프라인이 구성됨` 및 `'빌드' 단계가 시작됨`)를 표시합니다. 
 * GitHub 도구 통합을 구성한 경우, 사용하는 GitHub 계정에 샘플 GitHub 저장소가 복제됩니다.   
 
##도구 체인 보기
{: #viewing_a_toolchain}

도구 체인과 모든 도구 통합이 구성되면 도구 통합 페이지가 열립니다. 

1. 페이지를 검토하여 앱에서 사용할 도구 체인의 시각적 표시를 확인하십시오. 
1. 도구 체인에 있는 도구 통합에 액세스하려면 도구 타일을 클릭하십시오.  
 
 **팁**: 둘 이상의 GitHub 저장소가 있는 경우 저장소마다 자체 파이프라인이 필요하므로 동일한 도구 통합에 여러 개의 타일이 있을 수 있습니다. 