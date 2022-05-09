# RustWaveTableTest
ウェーブテーブルシンセサイザーを`Rust`で作成してみました。
# Crate
- rodio="0.14.0"
# OverView
``cargo run``で5秒ほど正弦波信号をもとに音を生成します。  

`main.rs`の80行当たりの値を変更することで周波数を変更することができます。
```
set_frequency(100.0);
```
また、86行当たりの`from_secs(5)`の引数の値を変更することで起動させてから鳴りやむまでの時間を設定できます。
```
std::thread::sleep(std::time::Duration::from_secs(5));
```
