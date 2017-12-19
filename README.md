# Hiroi-sOJT1
<dt>1.OJT3</dt>  
仕様  
SWを押すとLEDの点灯消灯が切り替わる(RX210)  
  
2.OJTObject5  
製品仕様  
・LEDをふわふわ点灯させる(一番明るいときと消えているときに2～10秒間ふわふわを停止する)  
・SWを押したらLEDがふわふわ点灯開始、もう一度押したら点灯終了  
・電源電圧が4.0V以下になるとマイコンが落ちる  
・環境温度が50℃以上になったらマイコンが落ちる  
・起動時にチェックサムを行う  
ハードウェアセットアップ  
・システムクロックは現状の回路構成で設定可能な最大周波数になるように設定  
・MTUまたはTPUでPWM信号を生成し、Duty更新をバッファ動作で行う  
・独立ウォッチドッグタイマを動作させる  
・AD変換値は移動平均をとる  
・浮動小数点演算は避ける  
