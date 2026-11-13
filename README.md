# KobitoKey_QWERTY (DYA Studio / ZMK v0.4 系)

[juichi50iii/KobitoKey_QWERTY](https://github.com/juichi50iii/KobitoKey_QWERTY) のフォーク。
ハードの記述は公式のまま、ファームの構成を moNa2
([Daytona0306/zmk-config-moNa2-v2](https://github.com/Daytona0306/zmk-config-moNa2-v2)) と同じものに載せ替えている。

| | 公式 | このフォーク |
|---|---|---|
| ZMK | zmkfirmware v0.3 (Zephyr 3.5) | Daytona0306/zmk (v0.4 系, Zephyr 4.1) |
| PMW3610 ドライバ | badjeff 版 | cormoran 版 (DYA Studio のセンサータブ対応) |
| 回転・倍率 | sensor_rotation + scaler (固定) | runtime input processor (Studio で調整可) |
| central | 左 | 左 (変更なし) |

- 左ボール = スクロール、右ボール = カーソル + オートマウスレイヤー (公式と同じ役割)
- キー配列はまだ公式の4レイヤーのまま。moNa2 の配列・ジェスチャー・慣性スクロールは未移植
- **トラックボールの向きは実機未確認。** 逆なら DYA Studio のセンサータブで変えて、
  確定値を `boards/shields/KobitoKey/KobitoKey_{left,right}.conf` に反映する
- モジュールの SHA 固定は `tools/west-pins.py` (使い方は moNa2 の README)

以下は公式の README。

---

小人キーや人キーのケース、TypeSurfer各種の3DデータはReleasesよりダウンロード出来ます。
ダサい使い方はしないこと。


Layer 0 QWERTY
<img width="1280" height="690" alt="Image" src="https://github.com/user-attachments/assets/ef0797b7-a63f-4632-912d-9b5d0115769f" />

Layer 1 NUMBER & ARROW
<img width="1280" height="690" alt="Image" src="https://github.com/user-attachments/assets/d6347b3c-a238-4278-bacd-e58195774d0e" />

Layer 2 Bluetooth & FUNCTION
<img width="1280" height="690" alt="Image" src="https://github.com/user-attachments/assets/f1f7cc93-fbd8-4a98-84ea-c8c36ad3952d" />

Layer 3 AUTO MOUSE
<img width="1280" height="690" alt="Image" src="https://github.com/user-attachments/assets/2efe5275-e460-41bc-ae45-0c0665435268" />
