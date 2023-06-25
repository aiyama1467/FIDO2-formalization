# FIDO2-formalization
## プロトコルファイル
- FIDO2_reg.pvl
  - FIDO2 register プロトコル
- FIDO2_auth.pvl
  - FIDO2 authenticate プロトコル
- FIDO2_reg_mac.pvl
  - FIDO2 register 修正プロトコル


## 検証用ファイル
- register.pv
  - register 検証ファイル
- authenticate.pv
  - authenticate 検証ファイル
- authenticate_A3.pv
  - authenticate 安全性 A3 検証用
- authenticate_A4.pv
  - authenticate 安全性 A4 検証用

# 実行方法
### 実行例
```
$ proverif -lib src/register.pvl src/register.pv
```
`-lib`でプロトコルファイル(`.pvl`)を指定。実行対象は検証用ファイル(`.pv`)を用いる。
検証用ファイル内の`at_type`, `au_type`, `ctap_type`, `tr_type`を変更することで様々なモードを検証できる。
