# なぜオブザーバビリティが必要なのか

YouTube の [Developing an Observability Strategy](https://www.youtube.com/watch?v=Ub3ATriFapQ) をご覧ください。

## 本当に重要なことは?

職場で行うすべてのことは、組織のミッションに合致する必要があります。雇用されている私たちはみな、組織のミッションの達成とビジョンの実現に向けて働いています。Amazon では、ミッションは次のように定義されています。

> Amazon は、地球で最も顧客中心的な企業、最高の雇用主、最も安全な職場を目指します。

— [Amazon について](https://www.aboutamazon.com/about-us)

IT において、すべてのプロジェクト、デプロイ、セキュリティ対策、最適化は、ビジネスの成果につながる必要があります。当然のことのようでいて、ビジネスに価値を付加しないことは何一つやるべきではありません。ITIL の言葉を借りれば:

> すべての変更はビジネス価値を提供する必要がある

— ITIL サービス移行、AXELOS、2011 年、44 ページ
— [クラウドにおける変更管理に関する AWS ホワイトペーパー](https://docs.aws.amazon.com/whitepapers/latest/change-management-in-the-cloud/change-management-in-the-cloud.html) を参照

ミッションとビジネス価値は、行うすべてのことの基準となるため重要です。
オブザーバビリティには多くのメリットがあります。

- 可用性の向上
- 信頼性の向上 
- アプリケーションの健全性とパフォーマンスの理解
- コラボレーションの改善
- 問題の予防的検知
- 顧客満足度の向上
- 上市までの期間の短縮
- 運用コストの削減
- 自動化

これらのメリットはすべて、ビジネス価値の提供、つまり顧客または組織に直接的あるいは間接的に利益をもたらす点で共通しています。オブザーバビリティを考える際、すべてアプリケーションがビジネス価値を提供しているかどうかに立ち返る必要があります。

つまり、オブザーバビリティは、ビジネス価値の提供に貢献するものを測定し、ビジネスの成果に焦点を当てる必要があります。成果がリスクにさらされている場合、顧客が何を必要としているかを考える必要があります。

## どこから始めればいいですか?

重要なことがわかったところで、何を測定する必要があるかを考える必要があります。Amazon では、お客様から逆算することから始めます。

> 我々はサービスの改善を内部的に推進しています。必要に迫られる前に、便益と機能を追加しています。必要に迫られる前に、価格を下げ、お客様への価値を高めています。必要に迫られる前に、革新しています。 

— ジェフ・ベゾス、[2012 年株主への手紙](https://s2.q4cdn.com/299287126/files/doc_financials/annual/2012-Shareholder-Letter.pdf)

簡単な例として、EC サイトを使ってみましょう。まず、オンラインで商品を購入する際に、お客様として何が欲しいかを考えてみてください。すべての人が同じというわけではありませんが、おそらくこうしたことを気にかけているでしょう。

- 配送
- 価格
- セキュリティ 
- ページ速度
- 検索 (探している商品が見つかるか)

お客様が何を重要視しているかを知ったら、それらを測定し、ビジネスの結果にどのように影響するかを調べることができます。ページ速度は、コンバージョン率と検索エンジンのランキングに直接影響します。2017 年の調査では、ページの読み込みに 3 秒以上かかると、モバイルユーザーの 53% がそのページを放棄することが示されています。もちろん、ページ速度の重要性を示す研究は多数ありますが、コンバージョンに測定可能な影響を与えるため、これを測定し、改善のためのデータを得る必要があります。

## ワーキングバックワーズ

お客様が重要だと考えていることすべてを知ることは期待できません。これを読んでいるあなたは、技術系の役割にあると思います。組織のステークホルダーと話をする必要があります。これは必ずしも簡単なことではありませんが、重要なことを測定していることを確認するために不可欠です。

Eコマースの例を続けましょう。今回は検索について考えてみましょう。製品を検索して購入するために、お客様が製品を検索できる必要があることは明白ですが、[Forrester Research のレポート](https://www.forrester.com/report/MustHave+eCommerce+Features/-/E-RES89561) によると、訪問者の 43% が即座に検索ボックスに移動し、検索は非検索ユーザーと比較して 2-3 倍の確率でコンバージョンにつながることをご存知でしょうか。検索は本当に重要で、うまく機能させる必要があり、モニタリングする必要があります。ある検索で結果が得られないことを発見し、単純なパターンマッチングから自然言語処理への移行が必要であることがわかる場合があります。これはビジネスの結果を監視し、顧客体験を改善するための行動を取る例です。 

Amazon では:

> 私たちはお客様を深く理解し、痛みの原因から出発して迅速にイノベーションを開発し、お客様の人生に意味のあるソリューションを生み出しています。

— Daniel Slater - Worldwide Lead, Culture of Innovation, AWS in [Elements of Amazon’s Day 1 Culture](https://aws.amazon.com/executive-insights/content/how-amazon-defines-and-operationalizes-a-day-1-culture/)

私たちはお客様から始め、ニーズから逆算しています。これはビジネスで成功する唯一のアプローチではありませんが、オブザーバビリティにとっては良いアプローチです。ステークホルダーと協力して、お客様にとって何が重要かを理解し、そこから逆算していきます。 

付加価値として、お客様とステークホルダーにとって重要なメトリクスを収集することで、これらをリアルタイムのダッシュボードで可視化し、「ランディングページの読み込みにどのくらいの時間がかかっているか」や「ウェブサイトの運用にどのくらいのコストがかかっているか」といったレポートの作成や質問への対応を避けることができます。ステークホルダーや経営陣は、この情報をセルフサービスで入手できる必要があります。

これらは、アプリケーションにとって**本当に重要な**高レベルのメトリクスであり、ほとんどの場合、問題がある最良の指標でもあります。 たとえば、通常期待される注文数よりも少ない注文数を示すアラートは、おそらく顧客に影響を与えている問題があることを示しています。 サーバーのボリュームがほぼ満杯であることや、特定のサービスに対して高い数の 5xx エラーがあることを示すアラートは、修正が必要なものかもしれませんが、それでも顧客への影響を理解して優先順位を決定する必要があります。これには時間がかかる場合があります。

これらの高レベルなビジネスメトリクスを測定すると、顧客に影響を与える問題が発生したときに簡単に特定できます。 これらのメトリクスは、発生している**何**を表しています。 他のメトリクスやトレースやログなどの他の形の可観測性は、**なぜ**これが発生しているのかを表しており、これを修正または改善するために何ができるかを導き出します。

## 観測するもの

ここまでで、お客様にとって何が重要かということがわかりました。次に、重要業績評価指標(KPI)を特定する必要があります。これらはビジネスの成果がリスクにさらされているかどうかを判断する上位指標です。また、それらの KPI に影響を与え得る、多くの異なるソースからの情報を収集する必要があります。これまでに議論したように、5xx エラーの数自体は影響を示すものではありませんが、KPI に影響を与える可能性があります。ビジネスの成果に影響を与えるものから、ビジネスの成果に影響を与え得るものへと逆向きに考えを進めていきます。

収集する必要があるものがわかったら、KPI やその KPI に影響を与え得る関連メトリクスを測定できるメトリクスを提供してくれる情報ソースを特定する必要があります。これが観測するものの基本となります。

このデータはおそらく、メトリクス、ログ、トレースから得られることでしょう。このデータが手に入ったら、成果がリスクにさらされたときにアラートを出すことができます。

その後、影響を評価し、問題を修正しようと試みることができます。ほとんどの場合、このデータは単独の技術的指標(CPU やメモリなど)よりも前に、問題があることを教えてくれます。

観測可能性を使って、ビジネスの成果に影響を与えている問題を反応的に修正したり、顧客の検索エクスペリエンスを改善するなどのように、データを先取り的に利用することができます。

## まとめ

CPU、RAM、ディスク容量などの技術的メトリクスは、スケーリング、パフォーマンス、容量、コストの面で重要ですが、アプリケーションの状況や顧客体験の洞察を示すものではありません。

重要なのはお客様であり、監視すべきはお客様の体験です。

そのため、お客様の要件から逆算し、ステークホルダーと協力して、重要な KPI とメトリクスを確立する必要があります。