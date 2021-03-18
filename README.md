# btc_img_realtime_prediction

비트코인 가격 이미지 데이터를 활용한 비트코인 가격 예측
1. 학습 데이터 기간 선정
2. 특정 기간의 비트코인 가격을 이미지로 변환 
3. 해당 이미지와 유사한 이미지를 과거 비트코인 가격 이미지에서 검색
4. 유사한 이미지의 다음 이미지를 예측값으로 return  

URL : http://115.85.180.168:8787/files/app/btc_img_finder_20210306.html

### To-Do-List

<ul>
 
<li> buy and sell signal </li>
<li> back-tesing function </li>
<li> master application -> monitoring tx_tracker and img_finder if one of them dead, run it again: monitoring time_interval = 10min </li>
<li> password website by shiny </li>
<li> (statics) seller's address forcasting index based on tx -> count of more than -5% drops within 6/12 hours </li>
<li> (ml) seller's address predictor -> based on tx, Y: count of -5% drops within 6/12 hours, Xs: address and amount of btc sented within the time interval </li>
<li> connet with upbit api </li>
<li> export preidction </li>
<li> network error count 오작동 수정하기 </li>
<li> network error occasionally (작업 중) </li>
<li> auto eval function 생성 -> 기존 ssim range01 resacle해서, prediction and realY의 scaled ssim 이 0.6이상이면 o, 아니면 x </li>

</ul>

# Recent Changes

### v0.0.3 - 2021/3/14

#### new features 

<ul>

<li> 상승장('20.09.01 - '21.03.15), 상승장2, 하락장, 횡보장 TAB 생성</li>
<li> tx summary table에 location 추가 </li>
<li> if amount btc > 1000, one warninng icon </li>

</ul>

### v0.0.2 - 2021/3/9

#### new features 

<ul>

<li> (plot) 30분/1시간/3시간/12시간/24시간 예측모델 </li>
<li> (print) network error count </li>

</ul>

### v0.0.1 - 2021/2/27

#### new features 

<ul>

<li> (function) btc tx real-time downloader </li>
<li> (function) btc real-time price downlaoder </li>
<li> (function) ssim index calculator </li>
<li> (function) data to img converter </li>
<li> (function) similar img finder </li>
<li> (data) btc address mapping(mapping btc unknown address -> known player) table </li>
<li> (data) btc historical price data updated (2020.09 - 2021.03) </li>
<li> (plot) 30 mins preidction </li>
<li> (print) ssim table   
  
</ul>
