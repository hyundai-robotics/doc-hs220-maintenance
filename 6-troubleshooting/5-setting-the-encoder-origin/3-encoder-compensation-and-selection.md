# 6.5.3. 엔코더 보정 및 선택


*	로봇 각 축의 기준 위치에 엔코더 DATA의 보정 작업이 필요합니다.
*	제어기 조작설명서『엔코더 보정』을 참조해서, 엔코더 보정을 해주십시오.

<b>[엔코더 보정화면]</b>

![](../../_assets/그림_6.5_엔코더_보정.png)

표 6-5 리셋 후 DATA 범위
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-wa1i{font-weight:bold;text-align:center;vertical-align:middle}
.tg .tg-jafi{background-color:#f8f8be;color:#000000;font-weight:bold;text-align:center;vertical-align:middle}
.tg .tg-nrix{text-align:center;vertical-align:middle}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-jafi">축</th>
    <th class="tg-jafi">리셋 후 DATA 범위</th>
    <th class="tg-jafi">엔코더 1회전당 PULSE 수</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-wa1i">전 축</td>
    <td class="tg-nrix">0 ~ 8,191</td>
    <td class="tg-nrix">8,192</td>
  </tr>
</tbody>
</table>

<ol style="list-style-type:decimal" start="1">
    <li>
축을 선택하고 [축조작]키로 기준위치로 축을 이동시키고 『[F1]: 단일 초기화』키를 누릅니다.
    </li><br>
    <li>
로봇 전축을 [축조작]키를 이용하여 기준자세로 위치시키고 『[F2]: 전체 초기화』키를 누르면 모든 축에 대해 한번에 엔코더 옵셋 보정이 수행됩니다.
    </li><br>
    <li>
설정 데이터를 저장하기 위해서는 『[F7]: 확인』키를 누릅니다. [ESC]키를 누르면 변경된 데이터가 저장되지 않습니다.
</li>
</ol>

<table>
<thead>
  <tr>
    <td><img src="../../_assets/주의표시.png" width = 60 height = 60> </td>
    <td colspan="4"><b>주의사항</b><br>
    모터 교환 후, 엔코더 DATA 보정을 행하는 경우, 일단 전원 준비를 『ON』상태로 해서 모터에 전원이 들어가는지를 확인해 주십시오.</td>
  </tr>
</thead>
</table>  


