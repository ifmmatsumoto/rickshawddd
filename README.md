人力車
===
人力車の業務をモデリングする。

## ゴール
人力車の業務で発生する売上を管理する

## 業務内容
売上方法は以下の4パターン  
 1.道行く人に声をかける→乗車してもらう  
 2.旅行会社から予約が入る   
 3.会社へ個人への指名の予約が入る  
 4.会社へ予約が入る（指名なし）
 
## 料金体系
- XXXXコース  
 XXXX円  
- XXXXコース  
 XXXX円  
- XXXX分コース  
 XXXX円  
 ※一人乗りの場合は半額になる

## 登場人物
- 車夫  
- マネージャー  
- お客さん  

## 売上計算方法  
- ※車夫の場合  
- 自分の売り上げの計算方法は以下の5パターン  
    1. 自分の営業でのご案内→全額が自分の売り上げ  
    2. 誰か(自分以外の車夫またはマネージャー)の営業でのご案内場合  
        平日の場合→料金のX割を自分の売り上げに計上  
        休日の場合→料金のX割を自分の売り上げに計上  
        ※人力車は二人乗りなので、3人以上のお客さんの場合は複数台で案内するので他の車夫に手伝ってもらう  
        ※誰かの営業でも一人乗りを担当の場合は、全額自分の売り上げに計上(一人乗りは半額料金なので)  
        ※差し引いた分の料金は、営業を決めた車夫の売り上げに計上される（マネージャーの計算は方法別なのでマネージャーに計上はされない）  
    3. 旅行会社からの予約の場合→料金からX割引き  
    4. 指名の予約の場合→全額が自分の売り上げ  
    5. 指名なしの予約の場合  
        平日の場合→料金のX割を自分の売り上げに計上  
        休日の場合→料金のX割を自分の売り上げに計上  
- 自分が営業しなくても売り上げが差し引かれないケース  
    1. 一日の時給発生時間は決まっており、その時間を超えたら移動はしない  
    2. 外国人の場合  
    3. 三が日、ゴールデンウィーク、シルバーウィークの期間  
- ※マネージャーの場合  
    1. 自分が営業で決めたご案内の総額※車夫からの移動などは無し  

## 給料計算方法  
- 車夫の場合  
    1. 時給  
         1日の稼働時間は決まっており、その時間分しか時給は発生しない  
         ※稼働時間は月によって変動する。  
    2. 日々ノルマに対する売上のパーセンテージに応じた賞金の合計  
         一人ひとりの一日単位の売上目標金額(全員一律)は決まっており、
         その目標に対して何パーセント売り上げたのかによって決まる  
          100%→XXXX円  
          以後、XX%ごとにXXX円ずつプラス  
         ※目標金額は平日と休日で変動し、月でも変わる  
    3. 月の目標金額に対する売上のパーセンテージに応じたインセンティブ  
         日々の売上目標の総額が月の売上目標金額になる  
         売上目標金額イコール売上なら100%  
         出勤日数は人それぞれなので、月の売上目標金額は人によって異なる  
         インセンティブの支給額は、1出勤あたりパーセンテージに応じてXXX円加算される。 
         出勤数が多ければその分、日数に応じて一日あたりに加算される額が大きくなっていく  
         ※たとえばトータル20日出勤しているとしたら  
         1-5日目は  
          1000円/一日あたり  
         6-10日目は  
          1200円/一日あたり  
      のように出勤日数が多ければ1日当たりの支給額が増える  
      ※"1000円"の部分はパーセンテージによって増減する  
- マネージャーの場合  
    1. 時給  
         1500円一律  
         稼働時間はどの月でも7時間  
    2. 自分の売り上げの5%