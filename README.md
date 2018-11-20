# KakaoSnackGame
제 1회 카카오스낵게임 공모전 응시작.
<hr>
<pre>
플레이 진행 플로우

1. 초기화면
화면구성 : 도움말 버튼, 사운드 버튼, 게임시작 버튼
1) 도움말 버튼을 통해 게임 진행 방법을 익힐 수 있음
2) 사운드 버튼을 클릭해 사운드 On, Off 선택
3) 게임시작 버튼 클릭 후 게임 진행

2. 게임화면
화면구성 : 체력게이지, 획득한 코인량, 스테이지 상태, 벌레, 게임 진행 시간, 게임 아이템, 일시정지 버튼

1) 화면상에 임의의 방향에서 3가지 종류의 벌레가 나타납니다.
2) 시간이 흐를수록 체력게이지가 감소합니다.
3) 각 스테이지 마다 지정된 플레이 시간이 경과 후 자동으로 
다음 스테이지로 전환되며 벌레들의 속도 및 전체 벌레 종류별 개체 비율이 바뀌며 
체력 게이지가 감소하는 속도가 증가합니다.
4) 사용자는 일시정지 버튼을 통해 게임을 잠시 멈출 수 있으며 
이어서 진행, 게임 새로 시작, 초기 화면으로 이동 등을 선택할 수 있습니다.

3. 게임진행

1) 화면상에 나타나는 벌레를 잡기 위해 사용자는 자신이 원하는 영역을 
터치하며 터치 시 해당 영역에 있는 벌레들이 죽습니다.

1-1) 파리 : 처치 시 소량의 체력 회복 및 소량의 코인 증가
1-2) 황금파리 : 처치 시 다량의 코인 증가
1-3) 무당벌레 : 처치 시 체력게이지 대량 감소

2) 플레이어는 벌레 사냥을 통해 획득한 코인으로 아이템을 구매해 더 오래 살아남을 수 있습니다.

2-1) 끈끈이 : 임의의 좌표에 끈끈이가 소환되어 벌레들의 움직임을 제한합니다.
2-2) 포션 : 소량의 체력을 회복합니다.
2-3) 스프레이 : 모든 벌레를 제거하며 감소된 체력을 모두 회복합니다.

3) 체력게이지는 지속해서 감소하며 일정 수준 미만으로 떨어질 경우 경고음과 함께 
체력게이지가 반짝이며 화면 하단의 과일바구니의 상태가 변화합니다.

4) 체력게이지가 모두 감소 시 게임이 종료되며 사용자의 플레이 타임이 게임 종료 화면에 출력됩니다. 
사용자의 플레이 타임이 일종의 점수가 되어 가장 오래 살아남은 사람이 승자입니다.
</pre>
<hr> 
개발 
<hr>
<pre>
Server 단은 스프링 프레임워크 기반으로 제작하였고, 
Front 단은 부트스트랩 프레임워크 기반으로 제작했습니다.
Howler JS를 이용하여 사운드 효과를 구현하였으며, 
각 벌레의 랜덤한 방향과 움직임을 위해 알고리즘을 구현하였습니다.
멀티스레드를 구현하기 위해 WebWoker를 이용하였고, 
다양한 브라우저나 기기에서의 원활한 플레이를 위해 최적화에 최대한 힘썼습니다.
</pre>
