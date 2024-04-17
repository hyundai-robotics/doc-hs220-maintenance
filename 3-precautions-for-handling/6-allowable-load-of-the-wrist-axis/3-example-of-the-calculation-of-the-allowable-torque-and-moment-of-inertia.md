# 3.6.3. 허용 토크, 관성 모멘트 계산 예

(1)	Case #1 간단한 2차원 모델

![](../../_assets/그림_3.14_2차원_부하_모델.png)

그림 3.11 2차원 부하 모델



M - 부하 중량

J<sub>xx</sub> - 부하 무게중심에서 X축 방향의 관성 모멘트

J<sub>yy</sub> - 부하 무게중심에서 Y축 방향의 관성 모멘트

J<sub>zz</sub> - 부하 무게중심에서 Z축 방향의 관성 모멘트

J<sub>a4</sub> - R2축 회전 중심에서의 관성 모멘트

J<sub>a5</sub> - B축 회전 중심에서의 관성 모멘트

J<sub>a6</sub> - R1축 회전중심에서의 관성 모멘트


 
<br></br>
☞ 부하조건: 가로, 세로 260mm, 두께 260mm 의 Stainless Steel (Mass 138.15kg)

① 중량제한

부하 중량: 138.15 ≤ 180 kg

   <br>

② 허용 토크 제한

B축 기준 무게중심 위치 L<sub>X</sub> = 350mm, L<sub>Y</sub> = 0mm, L<sub>Z</sub> = -60mm

B, R1축에서 무게중심까지의 거리를 계산하면 아래와 같습니다.

B축 기준 거리  $$L_{B} = \sqrt{0.35^{2} + 0.06^{2}} = 0.355m$$

R1축 기준 거리 $$L_{R1} = 0.06m$$

B축 부하 토크 $$T_{B}=MgL_{B}$$ 

R1축 부하 토크 $$T_{R1}=MgL_{R1}$$

<br>

③ 허용 관성모멘트 제한

무게중심에서 부하의 관성 모멘트  J<sub>xx</sub>= 1.56kgm², J<sub>yy</sub>= 1.56 kgm², J<sub>zz</sub>= 1.56 kgm²
    
B축 관성 모멘트 (Ja5)

$$J_{a5}=ML_{B}^{2}+J_{yy} = 138.15\times 0.355^{2} + 1.56 = 18.97\leq 106kgm^{2}$$

R1축 관성 모멘트 (Ja6)

$$J_{a6}=ML_{R1}^{2}+J_{xx} = 138.15\times 0.06^{2} + 1.56 = 2.06\leq 56kgm^{2}$$

<br>
  
④ 결론

중량, 토크, 관성모멘트 조건 모두 제한 조건을 만족하므로 안전합니다.

<br></br>

(2) Case #2 복잡한 3차원 모델

![](../../_assets/그림_3.15_3차원_부하_모델_2D_형상.png)

그림 3.12 3차원 부하 모델 2D 형상

<br></br>

알루미늄 블록 형상 조합
(σ=0.0027 g/mm<sup>3</sup> : 176.3 kg)

m1 (60×300×300)	 14.6kg

m2 (480×440×220)	125.4kg

m3 (280×300×160)	 36.3kg

<br>

mi  - i 블록 부하 중량

L<sub>xi</sub> - i 블록 X축 방향 무게중심 위치

L<sub>yi</sub> - i 블록 Y축 방향 무게중심 위치

L<sub>zi</sub> - i 블록 Z축 방향 무게중심 위치

<br>

① 중량 제한

부하 중량: 176.3 ≤180 kg

<br>

② 허용 토크 제한

B축 회전 중심에서 전체 부하의 무게중심 위치를 구하면 아래와 같습니다.

$$L_{x}=\frac{\sum_{i}^{}m_{i}L_{xi}}{\sum_{i}^{}m_{i}}=\frac{14.6X250+125.4X460+36.3X840}{176.3}=520.85mm$$

$$L_{y}= 0 mm$$
<p>
(Since the y-axis is symmetrical)

$$L_{z}=\frac{\sum_{i}^{}m_{i}L_{zi}}{\sum_{i}^{}m_{i}}=\frac{14.6X0+125.4X260+36.3X260}{176.3}=238.47mm$$

<br>

블록 전체 B축 기준 무게중심 위치 $$L_{x} = 520.85mm$$, $$L_{y} = 0mm$$, $$L_{z}= -238.47mm$$

<br>

B축에서 무게 중심까지의 거리 $$L_{B} = \sqrt{0.521^{2} + 0.238^{2}} = 0.573m$$

R1축에서 무게 중심까지의 거리 $$L_{R1} = \sqrt{0.238^{2} + 0.0^{2}} = 0.238m$$

<br>

B축 부하 토크 $$T_{B}=MgL_{B} = 101.02kgfm ≤ 110kgfm$$

R1축 부하 토크 $$T_{R1}=MgL_{R1} = 41.96kgfm ≤ 58kgfm$$

<br>

x1 y1 z1 – m1 블록의 x, y, z 방향 길이

x2 y2 z2 – m2 블록의 x, y, z 방향 길이

x3 y3 z3 – m3 블록의 x, y, z 방향 길이

<br>

L<sub>X1</sub>, L<sub>Y1</sub>, L<sub>Z1</sub> - B축 회전 중심에서 m1 블록 무게중심 위치

L<sub>X2</sub>, L<sub>Y2</sub>, L<sub>Z2</sub> - B축 회전 중심에서 m2 블록 무게중심 위치

L<sub>X3</sub>, L<sub>Y3</sub>, L<sub>Z3</sub> - B축 회전 중심에서 m3 블록 무게중심 위치

<br>

J<sub>xx1</sub>, J<sub>yy1</sub>, J<sub>zz1</sub> – m1 블록 무게중심에서의 x, y, z 축 별 관성모멘트

J<sub>xx2</sub>, J<sub>yy2</sub>, J<sub>zz2</sub> – m2 블록 무게중심에서의 x, y, z 축 별 관성모멘트

J<sub>xx3</sub>, J<sub>yy3</sub>, J<sub>zz3</sub> – m3 블록 무게중심에서의 x, y, z 축 별 관성모멘트


![](../../_assets/그림_3.16_3차원_부하_모델_3D_형상.png)

그림 3.13 3차원 부하 모델 3D 형상

<br>

③  허용 관성모멘트 제한

표 3-3 블록별 무게중심에서의 관성 모멘트
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-1e26{background-color:#f8f8be;color:#000000; font-weight:bold;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-amwm{font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-1e26">블록 무게(kg)</th>
    <th class="tg-1e26">무게 중심(L<sub>X</sub>, L<sub>Y</sub>, L<sub>Z</sub>)</th>
    <th class="tg-1e26">J<sub>xx</sub></th>
    <th class="tg-1e26">J<sub>yy</sub></th>
    <th class="tg-1e26">J<sub>zz</sub></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-amwm">m<sub>1</sub>(14.6)</td>
    <td class="tg-baqh">(0.25, 0, 0)</td>
    <td class="tg-baqh">0.219 kgm²</td>
    <td class="tg-baqh">0.114 kgm²</td>
    <td class="tg-baqh">0.114 kgm²</td>
  </tr>
  <tr>
    <td class="tg-amwm">m<sub>2</sub>(125.4)</td>
    <td class="tg-baqh">(0.48, 0, -0.26)</td>
    <td class="tg-baqh">2.530 kgm²</td>
    <td class="tg-baqh">2.915 kgm²</td>
    <td class="tg-baqh">4.433 kgm²</td>
  </tr>
  <tr>
    <td class="tg-amwm">m<sub>3</sub>(36.3)</td>
    <td class="tg-baqh">(0.89, 0, -0.26)</td>
    <td class="tg-baqh">0.350 kgm²</td>
    <td class="tg-baqh">0.314 kgm²</td>
    <td class="tg-baqh">0.509 kgm²</td>
  </tr>
</tbody>
</table>

<br>

B축 관성 모멘트 (J<sub>a5</sub>)

J<sub>a5</sud> = $$\sum_{i}^{}\left [ mi(L_{xi}^{2}+L_{zi}^{2})+j_{yyi} \right ]$$

=[14.6 X (0.25²) + 0.114]+[125.4 X (0.46² + 0.26²) + 2.915]+[36.3 X (0.85² +0.26²) + 0.314] = 67.95 ≤ 106kgm²


<br>

R1축 관성 모멘트 (J<sub>a6</sub>)

J<sub>a6</sud> = $$\sum_{i}^{}\left [ mi(L_{yi}^{2}+L_{zi}^{2})+j_{xxi} \right ]$$

=[14.6 X (0²) + 0.219]+[125.4 X (0.26²) + 2.530]+[36.3 X (0.26²) + 0.350] = 14.03 ≤ 56kgm²

<br>

4.	결론

    중량, 토크, 관성모멘트 조건 모두 제한 조건을 만족하므로 안전합니다. 
