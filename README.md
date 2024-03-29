# PDAO

**PDAO는 포스텍을 거점으로 한 블록체인 커뮤니티 및 오픈소스 재단입니다.**

PDAO를 이해하기 위해 필요한 일련의 문서들은 다음과 같습니다.

- [PDAO 공식 소개글(본 문서)](#pdao): PDAO의 정체성, 목적, 활동 등을 설명합니다.
- [PDAO 공식 홈페이지](https://dao.postech.ac.kr): PDAO의 공식 홈페이지입니다.
- [PDAO: The Multichain DAO](pdao-the-multichain-dao.md): PDAO만의 유니크한 DAO 구조와 그 핵심인 PBC (PDAO Beacon Chain)에 대한 기술적인 오버뷰를 소개합니다.
- [PDAO 헌법 (WIP)](constitution.md): PDAO의 헌법입니다. PDAO의 운영 방식, 규칙 등을 정의합니다.
- [Simperby](https://github.com/postech-dao/simperby): PDAO의 핵심 오픈소스 프로젝트이자 PDAO의 본체인 PDAO Chain을 구동하는 블록체인 엔진입니다.
- [Simperby: Protocol Overview](https://github.com/postech-dao/simperby/blob/main/docs/protocol_overview.md): Simperby의 가버넌스, P2P 채팅, 컨센서스에 대한 프로토콜을 설명합니다.
- [PDAO 공식 발표 슬라이드](https://drive.google.com/file/d/1FHm3I8DTloRAIdkwxFQPk4ILlP2aTQgC/view): 위 내용을 전반적으로 다루는 PDAO 소개자료입니다.

## 들어가며

이 글은 PDAO의 정체성과 목적, 비전을 제시하는 소개 글이자, 공식 런치를 위한 본격적 개발 기간 전 마지막 계획서로서 작성되었습니다.
중요한 아이디어와 의견들 주시고 내용을 검수해 주신 교내외의 많은 분들께 진심으로 감사드립니다.

PDAO 설립자 포항공과대학교 컴퓨터공학과 [양준하](https://junha1.github.io), 2022.05.09 작성 (2022.09.20 최종수정)

PDAO 공식 홈페이지: [https://dao.postech.ac.kr](https://dao.postech.ac.kr)

- [PDAO](#pdao)
  - [들어가며](#들어가며)
  - [PDAO는?](#pdao는)
  - [PDAO는 어떤 활동을 합니까?](#pdao는-어떤-활동을-합니까)
  - [PDAO는 왜 DAO(탈중앙화 조직)여야 합니까?](#pdao는-왜-dao탈중앙화-조직여야-합니까)
  - [DAO는 어떻게 운영됩니까?](#dao는-어떻게-운영됩니까)
    - [DAO는 무엇을 의결할 수 있습니까?](#dao는-무엇을-의결할-수-있습니까)
    - [PDAO에 기부하면 어떤 혜택이 있습니까?](#pdao에-기부하면-어떤-혜택이-있습니까)
  - [향후 계획](#향후-계획)
  - [FAQ](#faq)
    - [왜 동문이 아닌 외부인도 참여 가능한 공개 커뮤니티로 운영합니까?](#왜-동문이-아닌-외부인도-참여-가능한-공개-커뮤니티로-운영합니까)
    - [저는 포항공과대학교의 동문이 아닙니다. 그렇다면 왜 PDAO에 관심을 가져야 합니까?](#저는-포항공과대학교의-동문이-아닙니다-그렇다면-왜-pdao에-관심을-가져야-합니까)
    - [블록체인 안에서 특별히 집중하는 분야가 있습니까?](#블록체인-안에서-특별히-집중하는-분야가-있습니까)
    - [밈토큰은 무엇입니까?](#밈토큰은-무엇입니까)
    - [콜로니 체인에는 무엇이 있습니까?](#콜로니-체인에는-무엇이-있습니까)
  - [끝으로](#끝으로)

## PDAO는?

PDAO는 포스텍을 거점으로 한 블록체인 커뮤니티 및 오픈소스 재단입니다.

## PDAO는 어떤 활동을 합니까?

PDAO는 크게 다음과 같은 일을 합니다.

1. 정보 공유, 친목 및 네트워크를 위한 커뮤니티 운영
   - 아무나 참여할 수 있는 공개 Discord 서버
   - 각종 오픈소스 프로젝트들의 개발 커뮤니케이션 채널
2. 오픈소스 개발
   - PDAO의 대부분 개발은 Github에서 오픈소스로 이뤄짐
   - 범용성이 매우 높은 *Simperby*등의 프로젝트가 포함되어 있음
3. 양질의 교육 콘텐츠 생산 및 블록체인 대중화 활동
   - 공개 자체 세미나 및 외부 연사 초청
   - 대학 내 일반인들을 대상으로 한 이벤트 및 행사 (해카톤, 부스 등)
   - 유튜브 채널 및 위키 운영
   - 밈토큰 및 아트 NFT 발행
4. 연구 활동 지원
   - 스터디 그룹 조성 및 지원
   - 최신 연구주제에 대해 토론할 수 있는 세션 개최 및 소개자 초청
   - 다양한 체인들의 풀노드 운영 및 API 제공
   - 개발 중 나온 자체 연구결과 정리 및 퍼블리시
5. 대학 자체의 본격적인 크립토 채택을 촉진
   - 대학 발전기금을 암호화폐로 기부 받고 보유, 매매하는 프로세스 리서치 및 제안
   - 암호화폐를 통한 동문 기부 활성화 및 장학제도 운영 제안
   - 블록체인 관련 교원 채용을 위한 정보공유
   - 교내 강의 연계

## PDAO는 왜 DAO(탈중앙화 조직)여야 합니까?

PDAO는 이름에서 알 수 있듯이 DAO(Decentralized Autonomous Organization)로 운영됩니다.
PDAO의 목적을 달성하기 위해 재단의 구현체로서 DAO를 선택한 이유는 다음과 같습니다.

1. 블록체인을 다루는 재단이다 보니 수행하는 사업들에 암호화폐가 필요하거나 비용을 암호화폐로 지급할 수 있는 경우가 많습니다. 그렇기에 재단의 자산을 암호화폐로 관리하는 것에 이점이 있으며, 이를 집행할 주체로서 탈중앙화 프로토콜이자 의결기구인 DAO가 적합합니다.
2. 암호화폐를 보유하고 있는 분들로부터의 기부를 더 쉽게 유치할 수 있습니다.
3. 재단법인이 따로 필요 없기 때문에 행정적 절차가 간소화되고 DAO 특성상 매우 투명하고 민주적으로 조직을 운영할 수 있습니다.
4. 구성원들이 직접 DAO라는 탈중앙화 프로토콜을 개발, 기획, 운영함으로써 필요한 기술을 학습하고 크립토 산업 이해도를 갖출 좋은 기회를 제공할 수 있습니다.
5. Treasury, 밈토큰, NFT, 게임 등 탈중앙화 애플리케이션과 직접 연계가 가능합니다.

## DAO는 어떻게 운영됩니까?

- 자체 체인인 **PDAO Chain**이 DAO의 핵심 주체입니다.
- PBC는 PDAO가 유지보수하는 오픈소스 프로젝트이자 블록체인 엔진인 **Simperby**로 구동됩니다.
- PDAO에 있어서 PBC는 5가지로 작용합니다.
   1. 스탠드얼론한 P2P 커뮤니케이션 채널
   2. 가버넌스 플랫폼
   3. 컨센서스와 완결성(Finality)을 제공
   4. 멀티체인 상호운용성
   5. 분산 파일 스토리지
- 동문과 교수를 대상으로, 충분한 기여를 보인 사람은 의결권을 PBC 체인 상에서 의결을 통해 지급하며, 이를 분실하거나 해당 멤버가 부적절한 일을 하였을 때에도 마찬가지로 의결을 통해 무효화됩니다.
- PBC에서 가버넌스와 컨센서스를 거쳐 의결이 된 내용은 영구히 기록되며 멤버들이 운영하는 노드에 검증가능한 방법으로 분산저장됩니다.
- PBC에서 의결된 내용은 신뢰하는 3자의 도움 없이도 다른 상용체인에서 암호학적으로 검증가능합니다. 이를 통해 PDAO는 **멀티체인 DAO**로서 존재합니다. Treasury나 밈토큰과 같은 PDAO의 탈중앙화 애플리케이션은 Ethereum, Solana, Cosmos, Near, Polkadot 등의 다양한 체인에 배치되고, 이를 PBC에서 일괄적으로 관리하면서 다양한 체인의 생태계에 진출하게 됩니다. (이렇게 PDAO가 진출하고 PBC의 가버넌스와 컨센서스로 관리되는 체인들을 *콜로니 체인*이라고 합니다.)

### DAO는 무엇을 의결할 수 있습니까?

- 재단의 자산을 집행하기 위해 콜로니 체인의 Treasury 컨트랙트에서 토큰을 출금하는 것
- 재단의 자산을 운용하기 위해 특정 DeFi 서비스에 토큰을 예치하는 것
- 컨트랙트를 업데이트하거나 파라미터를 수정하는 것
- 의결권을 신규 발급하거나 이미 발급된 의결권을 무효화하는 것
- 밈토큰을 신규 발행하는 것
- 특정 메시지나 강령 등을 체인에 기록하는 것
- 임의의 데이터를 분산 스토리지에 저장하는 것

### PDAO에 기부하면 어떤 혜택이 있습니까?

- 아트 NFT, 밈토큰 지급
- 기부 액수가 충분히 크다면 의결권 NFT 지급
- 기부 시 원하는 짧은 메시지를 트랜잭션에 동봉, DAO 컨트랙트 온체인 상태에 기록 및 웹상에서 표시 (명예의 전당 등)
- 디스코드, 트위터를 비롯한 각종 채널에 해당 내역 업데이트
- 필요하면 PDAO 멤버들과 만날 수 있는 자리 개최 (채용, 네트워킹, 디스커션 등)

## 향후 계획

PDAO는 아직 정식 런치가 되지 않은 상태이며, 2022년 하반기 (12월 예정)에 PBC의 첫 블록을 생성하는 제네시스 행사를 가집니다.

이후에는 위에서 설명한 활동을 본격적으로 진행합니다.

## FAQ

### 왜 동문이 아닌 외부인도 참여 가능한 공개 커뮤니티로 운영합니까?

크립토는 분야 특성상 발전이 빠르고 새로운 정보가 지속적으로 업데이트되며,
다양한 비즈니스가 날이 다르게 생겨나며 궁극적으로는 미래 사회의 큰 패러다임 변화를 일으키고 있습니다.
그렇기에 다른 학교의 구성원이나 현업 혹은 학계 종사자들과 직접 자유로운 주제로 생산적인 정보 공유를
할 수 있는 공개 커뮤니티를 운영하는 것이 상당히 중요할 것으로 판단하였습니다.
이와 별개로 학교 구성원들만 참여 가능한 채널도 존재하지만,
주로 학내 행사 안내나 DAO 운영과 관련된 내용을 위한 것이고 대부분의 주요 채널은 개방적으로 운영됩니다.

### 저는 포항공과대학교의 동문이 아닙니다. 그렇다면 왜 PDAO에 관심을 가져야 합니까?

PDAO는 1차적으로는 학교 내외의 일들을 지원하는 단체지만, 궁극적으로는 크립토 산업의 파이를 키우는 역할을 합니다.
양질의 커뮤니티와 인적 네트워킹 채널을 활성화하고, 포항공과대학교와 구성원들을 주요 목표로 매스어답션을 시도하며,
필요한 사업이나 활동에는 재단으로서 적극적으로 지원하는 이 모든 활동이
결과적으로 미래에 블록체인 기술을 연구하고 크립토 비즈니스에 참여할 수준 높은 인재들의 유입을 촉진할 것입니다.
그렇기에 PDAO의 성공은 대한민국, 나아가 세계의 크립토 산업에 크게 기여할 것이고 동문이 아니신 분들도 관심을 가지실 필요가 있습니다.

### 블록체인 안에서 특별히 집중하는 분야가 있습니까?

블록체인은 기술이자 비즈니스이자 문화이자 금융시스템이자 사상입니다.
그렇기에 다양한 측면에서 접근할 수 있고 PDAO는 이를 모두 가치있게 여깁니다.
다만 이공계 연구중심 대학의 구성원들인 만큼 블록체인 코어 기술과 이를 구현하는 엔지니어링에서 상대적으로 더 큰 메리트를 가질 것으로 기대합니다.

### 밈토큰은 무엇입니까?

PDAO가 발급할 밈토큰은
크립토를 친숙하게 접할 수 있도록 재미와 캐주얼함 위주의 다양한 탈중앙화 활동을 할 수 있는 매개체로써 제공됩니다.
각종 이벤트를 통해 수시로 에어드랍 될 예정이며 이 토큰을 사용할 수 있는 애플리케이션(게임 등)을 직접 개발해 보는 소규모 프로젝트들을 종종 진행할 예정입니다.
락업을 제일 많이 하는 주소에게 재단 이자수익 소량을 분배해주는 등의 소소한 금전적 유틸리티가 예정되어 있으나
이 또한 이벤트성에 지나지 않으며, 진지한 토크노믹스를 통해 비즈니스로 이어가진 않습니다.

### 콜로니 체인에는 무엇이 있습니까?

Rust를 컨트랙트 언어로 사용하는 Polkadot, Cosmos, Near를 1기 콜로니 체인으로 선정해 개발중입니다.

## 끝으로

포항공과대학교는 소규모, 사립, 연구 중심 대학교라는 매우 유니크한 특성을 가지고 있습니다.
PDAO는 이를 이용하여 동문들 간의 강한 유대감을 통해 밀도 있고 생산적인 네트워킹의 장을 조성하며,
수준 높은 연구 및 개발활동과 교육을 다방면으로 지원하고,
더 나아가 블록체인이라는 신생 패러다임을 대학 차원에서 과감하게 수용하는 혁신적인 전략을 채택할 수 있도록 도울 것입니다.

PDAO는 포항공과대학교가 대한민국 블록체인과 크립토의 중심으로 자리 잡을 수 있다고 믿고, 또한 그것을 선도하는 핵심 주체로 발전한다는 목표를 굳게 가지고 있으며 이를 함께할 자발적인 참여자들을 항상 환영합니다.

PDAO 공식 홈페이지: [https://dao.postech.ac.kr](https://dao.postech.ac.kr)
