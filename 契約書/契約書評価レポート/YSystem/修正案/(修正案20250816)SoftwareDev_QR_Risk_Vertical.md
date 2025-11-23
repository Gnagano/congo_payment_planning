# YSystemソフトウェア開発契約リスク評価レポート（修正案）
## QRコード決済機能開発契約 - リスク項目と修正提案

作成日: 2025-08-16  
評価対象: YSystem_SoftwareDevelopment_QRPaymentFeature.md  
評価視点: Curiox Solutions Limitedに不利な条項の特定と修正提案

## エグゼクティブサマリー

本レポートは、YSystemとのソフトウェア開発契約において、Curioxに不利となる可能性のある条項を特定し、具体的な修正案を提示します。主要なリスク項目は以下の通りです：

### 🚨 主要リスク項目
1. **サポート期間の短さ**: 60日間・10時間制限
2. **保証期間の不足**: 60日間のみの動作保証
3. **責任制限の不十分さ**: 支払額上限の制限
4. **補償条件の厳格さ**: 重過失・故意のみ対象
5. **納期管理の曖昧さ**: 参考値扱いでペナルティなし
6. **準拠法の不明確さ**: 後日協議での決定
7. **受領条件の不利さ**: 本番利用で自動受領

## 1. 詳細リスク分析と修正提案

### 1.1 サポート期間・時間制限 🔴 高リスク

#### 原文抜粋
```
For a period 60 days after delivery … limited to a maximum of 10 hours total of support and training combined.
```

#### 日本語訳
納品後60日間、サポートとトレーニングを合わせて最大10時間のみ提供する。

#### リスク説明
- バグ修正や運用不具合が60日以降は有償
- 10時間では実運用サポートが不足
- 銀行システムの安定稼働に必要な期間として不十分

#### 修正案
```
The Developer shall provide 12 months of warranty support, including unlimited remote bug fixes and up to 40 hours of training, at no additional cost.
```

**日本語訳**: 開発者は、追加費用なしで、納品後12か月間の保証サポート（リモートによるバグ修正は無制限、トレーニングは最大40時間まで）を提供するものとする。

### 1.2 動作保証期間 🔴 高リスク

#### 原文抜粋
```
The Software will operate according to the Specifications for 60 days after delivery.
```

#### 日本語訳
ソフトウェアは納品後60日間のみ仕様どおりに動作することを保証する。

#### リスク説明
- 実稼働フェーズの欠陥が保証対象外になる恐れ
- 銀行システムとして保証期間が短すぎる
- 長期運用での問題発見時に対応困難

#### 修正案
```
The Developer warrants that the Software will conform to the Specifications for one (1) year from the acceptance date, and will correct defects at no cost within that period.
```

**日本語訳**: 開発者は、ソフトウェアが受領日から1年間、仕様に適合することを保証し、その期間内に発見された不具合を無償で修正する。

### 1.3 責任制限条項 🟡 中リスク

#### 原文抜粋
```
The Developer's total liability … shall not exceed the total amount paid by the Client under this agreement.
```

#### 日本語訳
開発者の累積責任は、クライアントが支払った金額が上限となる。

#### リスク説明
- 損害が支払総額を上回っても補償されない
- 銀行システム障害による損失は契約額を大幅に超える可能性
- 重大な過失の場合でも制限が適用される

#### 修正案
```
Total liability shall not exceed 200% of the amounts paid or USD 500,000, whichever is higher, and the cap shall not apply in cases of gross negligence or wilful misconduct.
```

**日本語訳**: 総賠償責任額は支払総額の200％または50万米ドルのいずれか高い方を上限とし、ただし重過失または故意の場合はこの上限を適用しない。

### 1.4 補償条件の制限 🟡 中リスク

#### 原文抜粋
```
Developer agrees to indemnify … only in cases of gross negligence or willful misconduct.
```

#### 日本語訳
開発者が補償を行うのは「重過失または故意」の場合に限る。

#### リスク説明
- 通常過失でも第三者訴訟が起きればクライアントが負担
- 知的財産権侵害のリスクが高い
- 立証責任がクライアント側に偏重

#### 修正案
```
The Developer shall fully indemnify and defend the Client against any third-party IP infringement claims arising from the Software, regardless of fault, except where the claim results from the Client's unauthorised modifications.
```

**日本語訳**: 開発者は、ソフトウェアに起因する第三者の知的財産権侵害請求について、過失の有無を問わずクライアントを全面的に補償・防御するものとし、ただしクライアントによる無断改変が原因の場合は除く。

### 1.5 納期管理とペナルティ 🟡 中リスク

#### 原文抜粋
```
The dates listed in Exhibit B … are for reference only. The Developer will inform the Client of the actual delivery dates.
```

#### 日本語訳
付属書Bのマイルストンは参考値であり、実際の納期は開発者が後で通知する。

#### リスク説明
- 納期遅延に対して契約上のペナルティがない
- プロジェクト計画の確実性が低い
- 遅延による機会損失の補償なし

#### 修正案
```
Milestone dates in Exhibit B shall be binding. Failure by the Developer to meet a milestone by more than 10 business days shall entitle the Client to liquidated damages of 1% of the milestone fee per week of delay.
```

**日本語訳**: 付属書Bに記載されたマイルストン日は拘束力を有するものとし、開発者が当該期日から10営業日を超えて遅延した場合、クライアントは1週間の遅延につきマイルストン報酬の1％の違約金を請求できる。

### 1.6 準拠法・管轄の不明確性 🟡 中リスク

#### 原文抜粋
```
The governing law and jurisdiction … shall be determined through mutual consultation.
```

#### 日本語訳
準拠法と裁判管轄は後日協議で決定する。

#### リスク説明
- 紛争時に適用法が不明確で手続きが長期化
- 法的予見可能性の欠如
- 紛争解決コストの増大

#### 修正案
```
This Agreement shall be governed by and construed in accordance with the laws of Japan, and the Tokyo District Court shall have exclusive jurisdiction over any dispute.
```

**日本語訳**: 本契約は日本法を準拠法とし、その解釈も同法に従うものとする。また、本契約に関して生じる一切の紛争については東京地方裁判所を専属的合意管轄裁判所とする。

### 1.7 受領条件の不利性 🟡 中リスク

#### 原文抜粋
```
The Software will not be deemed accepted until the Client signs the Acceptance Certificate; however, use in production constitutes acceptance.
```

#### 日本語訳
受入証明書に署名していなくても、本番利用した時点で受領とみなされる。

#### リスク説明
- 試験的運用でも「受領済み」とされ、保証請求が困難
- 検収プロセスの形骸化
- 不具合発見時の対応権利の喪失

#### 修正案
```
Use in production shall not constitute acceptance unless and until the Client signs the Acceptance Certificate, which may be withheld until all critical defects are resolved.
```

**日本語訳**: クライアントが受入証明書に署名し、重大な欠陥がすべて解消されるまで、本番環境での使用は受領とみなされないものとする。

## 2. リスク評価マトリクス

| リスク項目 | 影響度 | 発生可能性 | 総合リスク | 優先度 |
|-----------|--------|-----------|-----------|--------|
| サポート期間制限 | 高 | 高 | 🔴 高 | 1 |
| 動作保証期間 | 高 | 中 | 🔴 高 | 2 |
| 責任制限 | 中 | 中 | 🟡 中 | 3 |
| 補償条件制限 | 中 | 中 | 🟡 中 | 4 |
| 納期管理 | 中 | 中 | 🟡 中 | 5 |
| 準拠法不明確 | 中 | 低 | 🟡 中 | 6 |
| 受領条件 | 中 | 低 | 🟡 中 | 7 |

## 3. 推奨対応策

### 即座に対応すべき項目（高優先度）
1. **サポート期間の延長**: 12ヶ月・40時間への変更
2. **動作保証期間の延長**: 1年間への変更

### 交渉で改善すべき項目（中優先度）
3. **責任制限の緩和**: 上限額の引き上げと例外条項
4. **補償条件の拡大**: 知的財産権侵害の全面補償
5. **納期管理の強化**: 拘束力のあるマイルストンとペナルティ

### 契約締結前に確定すべき項目
6. **準拠法の明確化**: 日本法での統一
7. **受領条件の明確化**: 本番利用≠自動受領

## 4. 総合評価

### 契約締結の可否: **条件付き推奨** ⭐⭐⭐☆☆

#### 推奨条件
1. 上記修正案の採用（最低限、高優先度項目）
2. 詳細仕様書（別紙A）の事前確認
3. 開発環境・前提条件の明確化

#### 結論
現状の契約書には複数の不利な条項が含まれており、そのまま締結することは推奨できません。特にサポート期間と動作保証期間の短さは、銀行システムとして致命的なリスクとなる可能性があります。上記修正案を基に再交渉を行い、少なくとも高優先度項目については改善を図ることを強く推奨します。

---

*本評価は契約書の実務的観点からの分析であり、法的助言ではありません。最終的な判断は法務専門家と相談の上で行ってください。*
