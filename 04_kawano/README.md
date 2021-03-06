# AJACS36/ge



<p><span style="font-size:25px;display:inline-block;line-height:130%;text-indent:0px">遺伝子発現DB・解析ツールの紹介</span>
<br /></p>
<p>目次</p>
<div class="contents">
<a id="contents_1"></a>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li><a href="#taf036b7"> 遺伝子発現データベースに関する統合TV </a></li>
<li><a href="#bb55f671"> BioGPS </a>
<ul class="list2" style="padding-left:16px;margin-left:16px"><li><a href="#b7dd172e"> 【実習1】BioGPSを使ってある遺伝子の発現プロファイルを調べる </a></li></ul></li>
<li><a href="#h21a5220"> RefEx </a>
<ul class="list2" style="padding-left:16px;margin-left:16px"><li><a href="#d71c8bae"> 【実習2】RefEx を使って、組織特異的遺伝子を検索する </a></li></ul></li>
<li><a href="#x426b06b"> DAVID: The Database for Annotation, Visualization and Integrated Discovery </a>
<ul class="list2" style="padding-left:16px;margin-left:16px"><li><a href="#wd2c65be"> マイクロアレイデータの準備 </a></li>
<li><a href="#t120060f"> 【実習3】DAVIDを用いて、発現データの結果を生物学的に解釈する </a></li></ul></li>
<li><a href="#z337008a"> NCBI Gene Expression Omnibus (GEO) </a>
<ul class="list3" style="padding-left:32px;margin-left:32px"><li><a href="#lca52056"> GEOのエントリについて </a></li></ul>
<ul class="list2" style="padding-left:16px;margin-left:16px"><li><a href="#p112cdc5"> 【実習4】データセットブラウザ(Dataset browser)を利用して、GEOに登録されているマイクロアレイデータを解析する </a></li>
<li><a href="#of4939d3"> 【実習4.5】R/Bioconductorのインストール </a>
<ul class="list3" style="padding-left:16px;margin-left:16px"><li><a href="#k1932fab"> GEOから生データを入手し、自分で（Rを使って）バックグラウンド補正・正規化する </a></li></ul></li>
<li><a href="#u531c825"> 【実習5】GEOのデータをEXCELで解析してみる </a></li>
<li><a href="#r4b74645"> 【実習6】GEO2Rを利用して、GEOに登録されているマイクロアレイデータを解析する </a></li>
<li><a href="#a83d5bfe"> 【実習7】GEOを使って、自分の興味のある遺伝子の（ある実験条件下における）発現状況を調べる </a></li>
<li><a href="#ze44dc22"> 【実習8】GEOを使って、自分の興味のあるマイクロアレイ実験データセットを検索&amp;生データをダウンロードする </a></li></ul></li>
<li><a href="#b6353d6e"> 【参考1】遺伝子発現バンク(GEO)目次、通称「GEO目次」 </a></li></ul>
</div>

<hr class="full_hr" />
<h3 id="content_1_0"><a id="taf036b7" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#taf036b7" title="taf036b7"><span class="sanchor">_</span></a> <span style="font-size:20px;display:inline-block;line-height:130%;text-indent:0px">遺伝子発現データベース</span>に関する統合TV  </h3>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li><a href="http://togotv.dbcls.jp/?category=%C8%AF%B8%BD%BE%F0%CA%F3" rel="nofollow">統合TVの「発現情報」タグ </a>をクリック！</li>
<li><a href="http://togotv-curated.dbcls.jp/contents/category/expression#%E9%81%BA%E4%BC%9D%E5%AD%90%E3%83%BB%E3%82%BF%E3%83%B3%E3%83%91%E3%82%AF%E8%B3%AA%E7%99%BA%E7%8F%BE%E3%82%92%E7%B6%B2%E7%BE%85%E7%9A%84%E3%81%AB%E8%AA%BF%E3%81%B9%E3%81%9F%E3%81%84" rel="nofollow">統合TV Curatedの発現制御解析</a>から探す</li></ul>

<h3 id="content_1_1"><a id="bb55f671" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#bb55f671" title="bb55f671"><span class="sanchor">_</span></a> <a href="http://biogps.org/" rel="nofollow"><span style="font-size:20px;display:inline-block;line-height:130%;text-indent:0px">BioGPS</span></a>  </h3>
<p><span style="color:green">ヒト、マウス、ラットのさまざまな組織や細胞(株)における遺伝子発現プロファイルのデータベース</span></p>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li><a href="http://biogps.org/" rel="nofollow">BioGPS</a>はAffymetrix社製のマイクロアレイであるGeneChipを用いたさまざまな組織や細胞(株)遺伝子発現プロファイルのデータベース。</li>
<li>検索した遺伝子に対して、種々の外部データベースを横断検索することができるだけでなく、それらの設定を保存したり、表示方法を自由にカスタマイズすることができる「Gene annotation portal」。</li>
<li>外部データベースには、Wikipedia(Gene Wiki)、著名な試薬会社の検索窓へのリンク集、pathway、Nature系DB、モデル生物DB、文献DBなど多種多様</li>
<li>マウスのエキソンアレイのデータから遺伝子のスプライシングバリアント(Splicing variant)の発現状況も調べることが可能。最近ではCircadian関係のデータも。</li>
<li>さらに最近のアップデートで、NCBI Gene Expression Omnibus (GEO)中から選抜されたデータセットに切り替えて発現状況を調べることが可能に。</li></ul>

<h3 id="content_1_2"><a id="b7dd172e" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#b7dd172e" title="b7dd172e">_</a> 【実習1】BioGPSを使ってある遺伝子の発現プロファイルを調べる  </h3>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li><a href="http://togotv.dbcls.jp/20120911.html#p01" rel="nofollow">【復習用】遺伝子発現プロファイルデータベースBioGPSを使い倒す2012</a> <a href="http://lifesciencedb.jp/image/small_video_icon.png" rel="nofollow"><img src="http://lifesciencedb.jp/image/small_video_icon.png" alt="http://lifesciencedb.jp/image/small_video_icon.png" /></a></li>
<li><a href="http://togotv.dbcls.jp/20100829.html#p01" rel="nofollow">【以前の講習会動画】遺伝子発現データベースの活用法</a> <a href="http://lifesciencedb.jp/image/small_video_icon.png" rel="nofollow"><img src="http://lifesciencedb.jp/image/small_video_icon.png" alt="http://lifesciencedb.jp/image/small_video_icon.png" /></a></li>
<li>1. <a href="http://biogps.org/" rel="nofollow">http://biogps.org/</a>を開きます。</li>
<li>2.脂肪細胞分化に関係する遺伝子であるPeroxisome Proliferator-Activated Receptor γ (pparg)の発現プロファイルを調べてみましょう。中央の検索窓に「pparg」と入力し、「search」を押します。</li>
<li>3. 表示された検索結果の中から「ID 5468」をクリックします。</li>
<li>4. 最初はヒトのマイクロアレイデータが表示されます。</li>
<li>5. ppargはどの組織、細胞で強く発現しているでしょうか？</li>
<li>6. 画面左側の&quot;Current Gene List&quot;は右上の&lt;&lt;アイコンをクリックすると非表示にできます。非表示にすることで画面を広く使うことができます。</li>
<li>7. ページ内のウインドウは通常のウインドウと同じようにドラッグによる移動やサイズの変更などを行うことができます。 歯車マークのメニューから&quot;Open in browser&quot; を選択すると、新しいタブで表示できます。</li>
<li>8. &quot;Search&quot; と書かれた窓に単語(組織名など)を入力すると、その単語の含まれた部分が赤くハイライト表示されます。今回は &quot;Adipocyte&quot; と入力してみます。</li>
<li>9. &quot;Zoom&quot; のバーを用いることで、グラフの表示範囲を調整することが出来ます。</li>
<li>10. 発現量を示すバーをクリックすると発現強度の値が表示されます。</li>
<li>11. 場合によっては&quot;Probeset&quot;のプルダウンメニューから複数の項目を選択できる場合があります。これはどのようなケースが考えられるでしょうか？</li>
<li>12. &quot;Static Image&quot; をクリックすると、ズームや検索機能などのついていない、画像だけのグラフで表示されます。低スペックなマシンでは、こちらの方が軽快に動作するでしょう。</li>
<li>13. &quot;Correlation&quot;タブをクリックして検索すると、発現パターンが似ている他の遺伝子を検索できますが、どのような遺伝子が出てくるでしょうか？</li>
<li>14. &quot;Downloads&quot; をクリックすると現在表示している遺伝子の発現データを CSV 形式でダウンロードできます。</li>
<li>15. &quot;Dataset&quot;の右にある'change&quot;をクリックすると、デフォルトで用意されているデータセットやNCBI GEO中のデータセットを検索でき、それらのデータに表示を切り替えることができます。&quot;change&quot;をクリックしたあと、&quot;Default Datasets&quot;から&quot;Barcode on normal tissues (262 samples)&quot;を選択します。どのようにデータが変わったでしょうか。</li>
<li>16. さらに&quot;Search&quot;からキーワード検索で、GEOのデータを検索してみましょう。&quot;pparg&quot;と検索するとどのようなデータが選択できるでしょうか。</li>
<li>17. 右上の「default rayout」をクリックすると、検索した遺伝子に関して種々の外部データベースを横断検索できますが、どのようなデータが閲覧できるのか調べてみましょう。</li>
<li>18. マイクロアレイデータ右上の&quot;Species: Hs&quot;をクリックするとマウスやラットを選択できるので、&quot;M. musculus (Mouse)&quot;をクリックしてマウスのデータを表示できます。</li>
<li>19. 左上の「Search」タグをクリックして検索画面にもどり、自分の興味ある遺伝子について同様に検索してみましょう。
すぐに自分の興味ある遺伝子が浮かばない場合は、著名な<a href="http://ja.wikipedia.org/wiki/%E4%BA%BA%E5%B7%A5%E5%A4%9A%E8%83%BD%E6%80%A7%E5%B9%B9%E7%B4%B0%E8%83%9E" rel="nofollow">iPS細胞</a>を作るために必要な4因子（Oct3/4・Sox2・Klf4・c-Myc）がどの組織で発現しているか、またデータを切り替えて検索してみましょう。</li></ul>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li>【余談】
<a href="http://biogps.org/iphone/" rel="nofollow">BioGPSのiPhoneアプリ</a>が無料で公開されていますので、「あの遺伝子はどの組織で発現してるのかな？」とふと調べたいときにお手持ちのiPhoneで遺伝子発現を調べられます。</li></ul>

<h3 id="content_1_3"><a id="h21a5220" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#h21a5220" title="h21a5220"><span class="sanchor">_</span></a> <a href="http://refex.dbcls.jp/" rel="nofollow"><span style="font-size:20px;display:inline-block;line-height:130%;text-indent:0px">RefEx</span></a>  </h3>
<p><span style="color:green">ヒト、マウス、ラットの4つの異なる実験手法によって得られた40種類の正常組織における遺伝子発現リファレンスデータセット</span></p>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li><a href="http://refex.dbcls.jp/" rel="nofollow">RefEx </a>（Reference Expression dataset）は、ライフサイエンス統合データベースセンター（DBCLS）が提供する、4つの異なる実験手法（EST、GeneChip、CAGE、RNA-seq）によって得られた40種類の正常組織における遺伝子発現量を並列に表現することで、手法間の比較とともに各遺伝子の発現量を直感的に比較することが可能な、リファレンス(参照)データセットです。</li>
<li>キーワード・遺伝子名検索では逐次的に検索語候補が提示される</li>
<li>『転写因子』や『Gタンパク質共役受容体』などのようなあるカテゴリーに属した遺伝子群についてまとめて検索可能</li>
<li>『組織特異的遺伝子』をワンタッチで検索</li></ul>

<h3 id="content_1_4"><a id="d71c8bae" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#d71c8bae" title="d71c8bae">_</a> 【実習2】RefEx を使って、組織特異的遺伝子を検索する  </h3>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li>1. <a href="http://refex.dbcls.jp/" rel="nofollow">http://refex.dbcls.jp/</a>を開きます。</li>
<li>2. 画面中央の「組織特異的に発現する遺伝子を見る」の臓器アイコンにカーソルを合わせると、更に詳細な部位のアイコンが出るので、調べたい臓器（例は肝臓）をクリックします。</li>
<li>3. 一覧表示画面では、左のバーから「絞り込み検索」や「ソート項目」の切り替えができます。</li>
<li>4. 「Download」アイコンをクリックすると検索結果のタブ区切りテキストがダウンロードされます。</li>
<li>5. 各遺伝子の青字の部分（例 <a href="http://refex.dbcls.jp/gene_info.php?lang=ja&amp;db=human&amp;geneID=2243&amp;refseq=NM_000508&amp;unigene=Hs.351593&amp;probe=205649_s_at" rel="nofollow">fibrinogen alpha chain</a>）をクリックすると詳細情報を閲覧できます。</li>
<li>6. 「ヒートマップ on Bodyparts3D」では、表示する部位の切り替え（全身・体幹部・頭部）ができます。「皮膚・骨格筋を表示」もしくは「アニメーション表示」にチェックを入れるとどのように表示されるでしょうか。</li>
<li>7. 「組織40分類別データ」では、バーの上にマウスオーバーすると測定部位と発現値が表示されます。</li>
<li>8. 「Download」をクリックすると、表示中の遺伝子の組織40分類別の発現データがタブ区切り形式でダウンロードできます。</li>
<li>9. 「Probe set ID」のリンク先をクリックすると、どういう情報が参照できるでしょうか。</li>
<li>10. オーソログ対応遺伝子について、ヒトとマウスで比較してみましょう。どのような違いがあるでしょうか。</li>
<li>11. 自分の研究テーマに関連する、また興味のある遺伝子について検索してみましょう。</li></ul>

<h3 id="content_1_5"><a id="x426b06b" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#x426b06b" title="x426b06b"><span class="sanchor">_</span></a> <a href="http://david.abcc.ncifcrf.gov/" rel="nofollow"><span style="font-size:20px;display:inline-block;line-height:130%;text-indent:0px">DAVID: The Database for Annotation, Visualization and Integrated Discovery</span></a>  </h3>
<p><span style="color:green">マイクロアレイデータの生物学的な解釈</span></p>
<p><a href="http://david.abcc.ncifcrf.gov/" rel="nofollow">http://david.abcc.ncifcrf.gov/</a></p>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li>マイクロアレイ実験の一般的な目的は、実験条件によって得られたある遺伝子群の発現が生物学的にどういう意味を持つかを考えることです。

![](microarray.analysis.005.png)

</li>
<li>今回は、その方法の一つとして、マイクロアレイの結果に<a href="http://www.google.co.jp/url?sa=t&amp;source=web&amp;cd=4&amp;ved=0CEEQFjAD&amp;url=http%3A%2F%2Fja.wikipedia.org%2Fwiki%2F%25E9%2581%25BA%25E4%25BC%259D%25E5%25AD%2590%25E3%2582%25AA%25E3%2583%25B3%25E3%2583%2588%25E3%2583%25AD%25E3%2582%25B8%25E3%2583%25BC&amp;ei=ve9QTd6XMtG6cbeW1KUH&amp;usg=AFQjCNF8U-O4ktlMGoR9DNC0wKltmbjtmw" rel="nofollow">Gene Ontology</a>の用語を付与することで、生物学的な解釈を行います。</li>
<li><a href="http://togotv.dbcls.jp/20120927.html#p01" rel="nofollow">【復習用】DAVIDを使ってマイクロアレイデータを解析する 2012</a> <a href="http://lifesciencedb.jp/image/small_video_icon.png" rel="nofollow"><img src="http://lifesciencedb.jp/image/small_video_icon.png" alt="http://lifesciencedb.jp/image/small_video_icon.png" /></a></li></ul>

<h3 id="content_1_6"><a id="wd2c65be" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#wd2c65be" title="wd2c65be">_</a> マイクロアレイデータの準備  </h3>
<p>サンプルデータとして、<a href="http://www.ncbi.nlm.nih.gov/geo/" rel="nofollow">NCBI GEO</a>より取得した公共の遺伝子発現データを用います。このデータは、ある実験の前後の2群間で有意に発現減少した遺伝子群のリストです。</p>

[110208_IDlist.txt](110208_IDlist.txt)

<p>（右クリックして「新しいタブで開く」もしくは「名前を付けてリンク先を保存」してください。）
<br class="spacer" />
このデータは、どのような実験から得られたデータなのか、どのように解釈できるのかをDAVIDを使って考察してみましょう！</p>

<h3 id="content_1_7"><a id="t120060f" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#t120060f" title="t120060f">_</a> 【実習3】DAVIDを用いて、発現データの結果を生物学的に解釈する  </h3>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li>1. 上部メニューの「Start Analysis」をクリックします。</li>
<li>2. 画面左側バーで、probe IDリストをコピペ or ファイルを指定します。</li>
<li>3. リストのIDの種類タイプを選択します。 … 今回は、「AFFY_ID」と「Gene List」</li>
<li>4. Submit List をクリックするとリストが読み込まれます。</li>
<li>5. アップロードしたリストは、左側バーの「List Manager」で「Uploaded List_1」として保存されています。削除やrenameもできます。</li>
<li>6. 解析を続けます。真ん中の「Functional Annotation Tool」をクリックします。</li>
<li>7. 「Gene Ontology」をクリックすると、Gene Ontologyを用いた解析の細かいメニューが表示されます。</li>
<li>8. 今回は、GOTERM_BP_FAT (BP=Biological Process)に注目します。その右の「Chart」をクリックすると結果がポップアップされます。</li>
<li>9. P-value を2回クリックしてp-valueが小さい（統計的に有意である）順にしてみましょう … p-value小さい順は、一度やればしばらく覚えているので、次からはしばらくは必要ないです</li>


#### 結果


![](david_go_bp.png)



<li>[応用編] Pathways &gt; KEGG_PATHWAY や Tissue Expression &gt; UP_TISSUE なども見てみましょう。生物学的にどういうことが言えるでしょうか。
<a name="plugin_fold_anchor2"></a>

#### サンプルデータの答え

<div class="plugin_fold_body"><p>Arabidopsis thaliana (シロイヌナズナ)の植物細胞と細胞壁分解酵素を用いて取り除いた植物細胞（<a href="http://ja.wikipedia.org/wiki/%E3%83%97%E3%83%AD%E3%83%88%E3%83%97%E3%83%A9%E3%82%B9%E3%83%88" rel="nofollow">プロトプラスト</a>）との比較（＝植物細胞の<a href="http://ja.wikipedia.org/wiki/%E3%82%AB%E3%83%AB%E3%82%B9_%28%E6%A4%8D%E7%89%A9%29" rel="nofollow">脱分化</a>前・後）</p>
</div></li></ul>
<hr class="full_hr" />

<h3 id="content_1_8"><a id="z337008a" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#z337008a" title="z337008a"><span class="sanchor">_</span></a> <a href="http://www.ncbi.nlm.nih.gov/geo/" rel="nofollow"><span style="font-size:20px;display:inline-block;line-height:130%;text-indent:0px">NCBI Gene Expression Omnibus (GEO)</span></a>  </h3>
<p><span style="color:green">世界最大の遺伝子発現（<a href="http://ja.wikipedia.org/wiki/DNA%E3%83%9E%E3%82%A4%E3%82%AF%E3%83%AD%E3%82%A2%E3%83%AC%E3%82%A4" rel="nofollow">マイクロアレイ</a>）データベース（レポジトリ）</span></p>

<h4 id="content_1_9"><a id="lca52056" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#lca52056" title="lca52056">_</a> <a href="http://www.ncbi.nlm.nih.gov/geo/" rel="nofollow">GEO</a>のエントリについて  </h4>
<pre>    GEO ID 番号の最初の3文字が
    GPL:  プラットフォーム（マイクロアレイ等の型番）
    GSM: サンプル（1枚のマイクロアレイから出たデータ）
    GSE:  シリーズ（1つの実験で出たデータを集めたもの。通常複数の GSM からなる）
    GDS:  データセット（NCBIで比較可能なデータを集めて再編成したもの。GEO上で簡単な解析が可能）</pre>
<p><br class="spacer" /><br class="spacer" /></p>

<h3 id="content_1_10"><a id="p112cdc5" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#p112cdc5" title="p112cdc5">_</a> 【実習4】データセットブラウザ(Dataset browser)を利用して、GEOに登録されているマイクロアレイデータを解析する  </h3>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li><a href="http://togotv.dbcls.jp/20120128.html#p01" rel="nofollow">【復習用1】NCBI GEOの使い方3～データセットブラウザの使い方1～ 2012</a> <a href="http://lifesciencedb.jp/image/small_video_icon.png" rel="nofollow"><img src="http://lifesciencedb.jp/image/small_video_icon.png" alt="http://lifesciencedb.jp/image/small_video_icon.png" /></a></li>
<li><a href="http://togotv.dbcls.jp/20120227.html#p01" rel="nofollow">【復習用2】NCBI GEOの使い方4～データセットブラウザの使い方2～ 2012</a> <a href="http://lifesciencedb.jp/image/small_video_icon.png" rel="nofollow"><img src="http://lifesciencedb.jp/image/small_video_icon.png" alt="http://lifesciencedb.jp/image/small_video_icon.png" /></a></li>
<li>1. <a href="http://www.ncbi.nlm.nih.gov/geo/" rel="nofollow">http://www.ncbi.nlm.nih.gov/geo/</a>を開きます。</li>
<li>2. 今回は例として「dioxin」というキーワードを検索してみましょう。「Datasets」に入力終了後、「GO」をクリックします。</li>
<li>3. GEOに登録されている様々な実験条件で行なわれたマイクロアレイ実験における発現データが表示されます。</li>
<li>4. 今回は乳がん細胞にダイオキシンをふりかけた実験「Dioxin effect on breast cancer cell line (HG-U133A)」を例に説明します（6番目？）。</li>
<li>5.  タイトルをクリックすると、解析用の「データセットブラウザ」が開きます。</li>
<li>6. 「Expression profiles」をクリックすると、この実験データセットにおける個々の遺伝子発現状況を検索できるページに飛びます。</li>
<li>7. 検索窓に表示されているアクセッション番号の後に続けて遺伝子名を追加（今回は例として <a href="http://www.google.co.jp/search?q=Oct4" rel="nofollow">Oct4</a> ）すると、この実験データセット内におけるその遺伝子の発現データが検索できます。</li>
<li>8. 「データセットブラウザ」の「Data Analysis Tools」では詳細なデータ解析が可能です。</li>
<li>9. 「Find gene name or symbol:」のところに自分の興味ある遺伝子名を入れてみましょう。</li>
<li>10. 「Find genes that are up/down for this condition(s):」の「GO」をクリックするとどのような遺伝子がヒットするでしょうか。</li>
<li>11. 「Compare 2 sets of samples」では2群間で発現に差のある遺伝子を（統計学的に）検索できます。step1で発現量の違いを検出する方法を設定します。step.2で比較する2群の設定をします。step.3の「Query Group A vs. B」をクリックすると、検索が始まります。</li>
<li>12. 「Cluster heatmaps」では、マイクロアレイデータ解析でよく用いられる<a href="http://MotDB.DBCLS.jp/?%5B%5Bhttp%3A%2F%2Fimages.google.co.jp%2Fimages%3Fq%3D%A5%D2%A1%BC%A5%C8%A5%DE%A5%C3%A5%D7%5D%5D" title="http://images.google.co.jp/images?q=ヒートマップ" rel="nofollow">ヒートマップ</a>でのデータ表示が行なえます。分類方法としてHierarchical、Partitional (K-means/K-medians)、By location on chromosomeの3種類が選べますが、それぞれどのようにデータが分類されるか試してみましょう。</li>
<li>13. ヒートマップ上をクリックすると領域選択が開始されます。リサイズや移動で範囲を決定した後、Stack up をクリックすると選択した範囲が拡大されます。</li>
<li>14. サンプルの内容とIDの対応は、元のページに戻って、Sample Subsets から確認できます。</li>
<li>15. さらに範囲選択して、Plot values をクリックすると、各遺伝子のサンプルごとの発現の様子がプロットで確認できます。</li>
<li>16. 範囲選択して、View in Entrez をクリックすると、選択範囲内のデータを棒グラフで見られます。</li>
<li>17. 範囲選択して、Download をクリックすると、選択範囲内のデータがテキスト形式でダウンロードできます。</li>
<li>18.  「Experiment design and value distribution」では実験データにおける発現の分布を参照できます。これにより、各サンプルのデータが互いに比較可能か（実験上のミスがないか）チェックすることができます。</li></ul>

<h3 id="content_1_11"><a id="of4939d3" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#of4939d3" title="of4939d3">_</a> 【実習4.5】R/Bioconductorのインストール  </h3>
<ul class="list2" style="padding-left:32px;margin-left:32px"><li><a href="http://www.r-project.org/" rel="nofollow">R</a>/<a href="http://www.bioconductor.org/" rel="nofollow">Bioconductor</a>
<ul class="list3" style="padding-left:16px;margin-left:16px"><li>東京大学門田先生による詳細な<a href="http://www.iu.a.u-tokyo.ac.jp/~kadota/r.html" rel="nofollow">利用法解説</a></li>
<li><a href="http://togotv.dbcls.jp/20090313.html" rel="nofollow">統合TV1</a>、<a href="http://togotv.dbcls.jp/20090319.html" rel="nofollow">統合TV2</a>、<a href="http://togotv.dbcls.jp/20090618.html" rel="nofollow">統合TV3</a>、<a href="http://togotv.dbcls.jp/20091219.html" rel="nofollow">統合TV4</a></li></ul></li></ul>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li>統合TV：<a href="http://togotv.dbcls.jp/20090313.html#p01" rel="nofollow">統計解析ソフト「R」の使い方 ～導入編～（winxp）</a></li>
<li>統合TV：<a href="http://togotv.dbcls.jp/20090618.html#p01" rel="nofollow">統計解析ソフト「R」の使い方 ～導入編～（macosx）</a>
<br class="spacer" /><br class="spacer" /></li></ul>
<p>1. <a href="http://www.r-project.org/" rel="nofollow">R</a> のサイトに行きます（「R」もしくは「R statistics」）<br class="spacer" />
2. download R のリンクをクリック<br class="spacer" />
3. ダウンロード元を聞かれるので、「Japan」の「Hyogo University」か「University of Tsukuba」のサイトをクリック（ミラー：<a href="http://dbcls.rois.ac.jp/~kawano/AJACS/" rel="nofollow">http://dbcls.rois.ac.jp/~kawano/AJACS/</a>）<br class="spacer" />
4. インストールするコンピュータのOSを選択（windows）<br class="spacer" />
5. 「base」をクリック<br class="spacer" />
6. 一番上にある「Download R 2.11.1 for Windows」をクリック<br class="spacer" />
7. ダウンロードが終わったらインストール<br class="spacer" />
　1. 言語は日本語でOKのはずですが、インストールの途中で文字化けした場合、一度インストールを中止し、言語をEnglishにしてやり直してください<br class="spacer" />
　2. 「Startup Option」のところで「Yes (customized startup)」を選んでください（コンポーネント選択の次の画面）<br class="spacer" />
　3. 最初の二つはそのままでOK<br class="spacer" />
　4. 「Internet Access」のところで、プロキシ接続が必要な場合（企業や学校からつなぐ場合に必要となることがあります）は「Internet2」を選択します<br class="spacer" />
　5. あとはそのままで全部OK<br class="spacer" />
8. R を起動します<br class="spacer" />
9. Bioconductor の一括インストール　＜注：講習会ではこれは実行しないでください＞<br class="spacer" />
　1.</p>
<pre>source(&quot;http://bioconductor.org/biocLite.R&quot;) </pre>
<p>　と打ち込んでリターン<br class="spacer" />
　2.</p>
<pre>bioclite() </pre>
<p>　と打ち込んでリターン<br class="spacer" />
　3. でインストールが始まりますが、かなり時間がかかるので今回は省略します<br class="spacer" />
10. Bioconductor パッケージの個別インストール<br class="spacer" />
　1. R 上部のメニューから「Packages」→「Select repositories」を選択します<br class="spacer" />
　2. 「BioC software」を選んで OK<br class="spacer" />
　3. R 上部のメニューから「Packages」→「Install package(s)」を選択します<br class="spacer" />
　4. 「affy」を選択して OK<br class="spacer" />
　5. R 上部のメニューから「Packages」→「Select repositories」を選択します<br class="spacer" />
　6. 「BioC annotation」を選んで OK<br class="spacer" />
　7. R 上部のメニューから「Packages」→「Install package(s)」を選択します<br class="spacer" />
　8. 「hgu133acdf」を選択して OK<br class="spacer" />
<br class="spacer" /><br class="spacer" /><br class="spacer" /><br class="spacer" /><br class="spacer" /></p>

<h4 id="content_1_12"><a id="k1932fab" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#k1932fab" title="k1932fab">_</a> GEOから生データを入手し、自分で（Rを使って）バックグラウンド補正・正規化する  </h4>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li>統合TV：<a href="http://togotv.dbcls.jp/20090319.html#p01" rel="nofollow">統計解析ソフト「R」の使い方 ～正規化編～</a>
<br class="spacer" /><br class="spacer" /></li></ul>
<p>1. 実験シリーズから生データをダウンロードします<br class="spacer" />
2. さきほどのGDS2744のページから、このデータセットの元になった実験シリーズ「GSE7765」のページに行きます<br class="spacer" />
3. 一番下からダウンロードできますが、ファイルサイズが大きいので <a href="http://dbcls.rois.ac.jp/~kawano/AJACS/" rel="nofollow">http://dbcls.rois.ac.jp/~kawano/AJACS/</a> からダウンロードしましょう（GSE7765.zip）<br class="spacer" />
4. 解凍します<br class="spacer" />
5. Rでデータのあるフォルダを指定します。「File」→「Change dir」から先ほど解凍したフォルダを指定します<br class="spacer" />
6.</p>
<pre>library(affy) </pre>
<p>と入力（コピペ）します。正規化用パッケージを呼び出しています<br class="spacer" />
7.</p>
<pre>write.exprs(justRMA(), file=&quot;RMA_expression.txt&quot;)</pre>
<p>と入力（コピペ）します。RMAという方法で正規化し、ファイルに保存しています<br class="spacer" />
8.</p>
<pre>write.exprs(mas5(ReadAffy()), file=&quot;MAS5_expression.txt&quot;)</pre>
<p>と入力（コピペ）します。MAS5という方法で正規化し、ファイルに保存しています<br class="spacer" />
9.</p>
<pre>write.exprs(mas5calls(ReadAffy()), file=&quot;MAS5calls_expression.txt&quot;)</pre>
<p>と入力（コピペ）します。MAS5で正規化し、その遺伝子が発現しているか（Present = P）発現していないか（Absent = A）を判定して、ファイルに保存しています<br class="spacer" />
<br class="spacer" /></p>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li><a href="http://motdb.dbcls.jp/?AJACS21%2Fwada" rel="nofollow">R/Bioconductorを使った遺伝子発現解析～導入と解析例～</a></li></ul>

<h3 id="content_1_13"><a id="u531c825" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#u531c825" title="u531c825">_</a> 【実習5】GEOのデータをEXCELで解析してみる  </h3>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li>参考図書：<a href="http://www.amazon.co.jp/%E3%83%9E%E3%82%A4%E3%82%AF%E3%83%AD%E3%82%A2%E3%83%AC%E3%82%A4%E3%83%87%E3%83%BC%E3%82%BF%E7%B5%B1%E8%A8%88%E8%A7%A3%E6%9E%90%E3%83%97%E3%83%AD%E3%83%88%E3%82%B3%E3%83%BC%E3%83%AB%E2%80%95Excel%E3%82%92%E4%B8%AD%E5%BF%83%E3%81%A8%E3%81%97%E3%81%9F%E3%83%87%E3%83%BC%E3%82%BF%E3%81%AE%E6%A8%99%E6%BA%96%E5%8C%96%E3%81%8B%E3%82%89%E6%9C%89%E6%84%8F%E5%B7%AE%E8%A7%A3%E6%9E%90%E3%80%81%E3%82%AF%E3%83%A9%E3%82%B9%E3%82%BF%E3%83%AA%E3%83%B3%E3%82%B0%E3%80%81%E3%83%8D%E3%83%83%E3%83%88%E3%83%AF%E3%83%BC%E3%82%AF%E8%A7%A3%E6%9E%90%E6%B3%95%E3%81%AE%E3%81%99%E3%81%B9%E3%81%A6-%E5%AE%9F%E9%A8%93%E5%8C%BB%E5%AD%A6%E5%88%A5%E5%86%8A-23-%E8%97%A4%E6%B8%95-%E8%88%AA/dp/4758101736/ref=sr_1_1?ie=UTF8&amp;s=books&amp;qid=1278382179&amp;sr=8-1" rel="nofollow">マイクロアレイデータ統計解析プロトコール</a>（羊土社）<br class="spacer" /><br class="spacer" /></li></ul>
<p>※注意：EXCELのバージョンによっては操作が異なる場合があります。</p>
<p>1. 先ほど使用した「GDS2744」のページから、バックグラウンド補正・正規化後のデータをダウンロードします。右側のクラスター図の下の「Download」にある「DataSet SOFT file」をクリックすればダウンロードできますが、みんなでアクセスすると迷惑なので、<a href="http://dbcls.rois.ac.jp/~kawano/AJACS/" rel="nofollow">こちら</a>からダウンロードしましょう(GDS2744.soft、右クリックから「対象をファイルに保存」)。<br class="spacer" />
2. EXCELを起動して、「ファイルを開く」から「ファイルの種類」を「すべてのファイル」にします<br class="spacer" />
3. 先ほどダウンロードした「GDS2744.soft」ファイルを指定します<br class="spacer" />
4. このファイルは「タブ区切りファイル」なので、データ形式指定のところでタブ区切りを指定します<br class="spacer" />
　1. 「カンマやタブなどの区切り文字によってフィールドごとに区切られたデータ」を指定して「次へ」<br class="spacer" />
　2. 区切り文字に「タブ」を指定して次へ<br class="spacer" />
　3. 完了<br class="spacer" />
　4. 45行目から、データが6個のカラムに別れていることを確認する<br class="spacer" />
　5. 43行目までは不要なので削除してしまいましょう。22217行目から下も、コントロールデータ（ポジコン・ネガコン）なので削除してしまいましょう<br class="spacer" />
5. まず、2種類のサンプルの倍数変化（Fold Change）をみて、遺伝子発現の増減を検出します。<br class="spacer" />
　1. 2行目のJ列を選択して、「数式」から「挿入」を選択して「統計」から「AVERAGE」を選択し、C2セルからE2セルまでを範囲指定します<br class="spacer" />
　2. 同様にK列に、F2セルからH2セルまでの平均値を計算します<br class="spacer" />
　3. L列に倍数変化（K2/J2）を計算します。ただし、そのまま計算すると発現が増加の場合と減少で数値が非対称になってしまうので、底が2の対数をとります。「挿入」→「数学/三角」の「LOG」を選択して、数値に「K2/J2」、底に「2」を入力します（=LOG(K2/J2,2)）<br class="spacer" />
　4. J2~L2を選択して一番下まで移動し、「シフトボタン」を押しながらj22216~L22216を選択する<br class="spacer" />
　5. 「ホーム」→「フィル」→「下方向にコピー」で、全データに計算式を適用<br class="spacer" />
　6. 全データを選択し（シートの左上の角をクリックするか、Controlキー＋A）、「データ」→「並べ替え」→「並べ替えのユーザ設定」を選択する<br class="spacer" />
　7. まず、「先頭行をデータの見出しとして使用する」にチェックを入れてから、最優先されるキーを「(列L)」にする。順序に「最大から最小」を指定して、OK<br class="spacer" />
　8. dioxinを添加したときに発現が増加する順に並び替えられました（3行目など上位に来ている多くはノイズの可能性が高いことに注意）。下から見ると、発現が減少した順に見ることができます<br class="spacer" />
6. 次に、t検定によるp値を求めます<br class="spacer" />
　1.  M2セルを選択し、「数式」→「挿入」→「統計」から「T.TEST」を選びます。<br class="spacer" />
　2. 配列1にC2～E2を、配列2にF2～H2を指定します。尾部には「2」を指定（両側検定）、検定の種類には「3」を指定します（等分散性を仮定しない）　（=T.TEST(C2:E2,F2:H2,2,3）<br class="spacer" />
　3. 一番下まで移動して、M22216セルをシフトキーを押しながらクリックします<br class="spacer" />
　4. 「ホーム」→「フィル」→「下方向にコピー」<br class="spacer" />
7. FCが1以上（2倍以上発現量増加）かつp値が0.01以下のプローブを検索します<br class="spacer" />
　1. N2セルに「数式」→「挿入」→「論理」→「AND」関数を使って論理式1に「L2&gt;1」、論理式2に「M2&lt;0.01」を入れる。「フィル」下までコピーする（TRUEが条件を満たしたプローブ）<br class="spacer" />
　2. 「データ」→「並べ替え」で最優先されるキーに「列N」、順序に「最大から最小」を指定して、次に優先されるキーに「列L」、順序に「最大から最小」を指定してデータを並び替える（10行目までが条件を満たしたプローブ）<br class="spacer" />
<br class="spacer" /><br class="spacer" /><br class="spacer" /><br class="spacer" /><br class="spacer" /></p>

<h3 id="content_1_14"><a id="r4b74645" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#r4b74645" title="r4b74645">_</a> 【実習6】GEO2Rを利用して、GEOに登録されているマイクロアレイデータを解析する  </h3>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li><a href="http://togotv.dbcls.jp/20120524.html#p01" rel="nofollow">【復習用】NCBI GEOの使い方5～GEO2Rを使う～</a> <a href="http://lifesciencedb.jp/image/small_video_icon.png" rel="nofollow"><img src="http://lifesciencedb.jp/image/small_video_icon.png" alt="http://lifesciencedb.jp/image/small_video_icon.png" /></a></li>
<li>1. <a href="http://www.ncbi.nlm.nih.gov/geo/" rel="nofollow">http://www.ncbi.nlm.nih.gov/geo/</a>を開きます。</li>
<li>2. 画面中央下の「<a href="http://www.ncbi.nlm.nih.gov/geo/browse/?view=series" rel="nofollow">Series</a>」をクリックします。</li>
<li>3. 検索機能を使って興味のある実験データセットを探すことができます。</li>
<li>4. 今回は喫煙による遺伝子発現の変化に関するデータについて調べたいというモチベーションを例にするので、「cigarette smoke」と入力し、検索します。</li>
<li>5. <a href="http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE17913" rel="nofollow">GSE17913 - Effects of Cigarette Smoke on the Human Oral Mucosal Transcriptome</a> という喫煙による口腔粘膜の遺伝子発現を調べたデータセットが見つかったので、「<a href="http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE17913" rel="nofollow">GSE17913</a>」をクリックします。</li>
<li>6. 今回のテーマであるGEO2Rへのリンクはページ下部にあるので、リンクをクリックし<a href="http://www.ncbi.nlm.nih.gov/geo/geo2r/?acc=GSE17913" rel="nofollow">GEO2Rのページに移動</a>します。</li>
<li>7. このデータセットに含まれるサンプルの一覧が表示されます。列見出しをクリックすると各項目でソートできます。「Title」をクリックすると、今回のデータセットが、喫煙者・非喫煙者のそれぞれ男性・女性の頬粘膜(buccal mucosa)から得られたサンプルであることがわかります。</li>
<li>8. 比較したいグループをそれぞれ設定します。「Define groups」をクリックして、それぞれのグループ名を入力します。今回は、非喫煙者の女性(never_smoker_F)と、喫煙者の女性(smoker_F)のサンプルをそれぞれグループ化します。</li></ul>
<p><span style="color:red">（※GEO2Rの各ジョブの実行は時間がかかるので要注意。講習では<a href="http://togotv.dbcls.jp/20120524.html#p01" rel="nofollow">復習用統合TV</a>の実行結果を見ながら進めるので、実行しないでください。）</span></p>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li>9. グループに入れたいサンプルをクリックやドラッグで選択してからグループ名をクリックすると、サンプルがグループに登録されます。</li>
<li>10. 次に、「Samples」をクリックした後、「Value distribution」タブをクリックし、「View」をクリックすると各サンプルの発現分布を調べることができます。</li>
<li>11. 発現分布が箱ひげ図で示されます。データセットブラウザと異なり、GEO2R では投稿された生のデータを用いて解析されます。</li>
<li>12. &quot;Export&quot; をクリックすると、箱ひげ図で与えられている値をまとめたタブ区切りテキストが表示され、これらを保存できます。</li>
<li>13. GEO2R タブに戻り、&quot;Top 250&quot; をクリックすると、選択したグループ間で各遺伝子の発現量に差があるかどうかの t 検定の結果、P 値が小さい順に 250 件表示されます。&quot;P.Value&quot; は元の P 値、&quot;adj.P.Val&quot; は多重検定の補正をかけた後の P 値です。有意性の評価は adj.P.Val に基づいています。
&quot;t&quot; は普通の t の標準偏差を全遺伝子の標準偏差を用いて調整したもの (moderated-t) です。普通の t より精度が上がっていますが、普通の t 分布に従うものとして扱えます。 &quot;B&quot; は2つのグループで発現量が異なっている対数オッズ値です。exp(B)/(1+exp(B)) の値が、発現量が異なっている確率で
す。&quot;logFC&quot; は、発現量の差が何倍であるかを2底の対数にしたものです。つまり値が 2 なら 4 倍の差を示しています。ここでの解析では発現量が対数で与えられている必要がありますが、元のデータでは対数になっていないことがあります。そのような場合デフォルトでは自動検出し、対数変換して計算してくれます。その上でこのような表示がされます。</li>
<li>14. 行をクリックすると、その行の遺伝子の各サンプルでの発現量グラフが見られます。</li>
<li>15. 今回喫煙者女性・非喫煙者女性間で最も差が大きいとされた遺伝子であるシトクロム P450 (異物代謝に関わる遺伝子)は、喫煙者群で有意に発現増加したことがわかります。</li>
<li>16. &quot;Sample values&quot; をクリックすると、発現量の値が一覧できます。</li>
<li>17. &quot;Select columns&quot; をクリックすると、表示するカラムを変更できます。 &quot;logFC&quot; を消し &quot;GO.Function&quot; を追加してみましょう。</li>
<li>18. &quot;Save all results&quot; をクリックすると、結果をテキストで表示・保存できます。</li>
<li>19. Options タブをクリックすると、いくつかの設定を変更できます。右の項目は多重検定の補正法の選択です。デフォルトでは Benjamini &amp; Hochberg の方法が使われていますが、これを Bonferroni の方法に変更してみます。中央はデータの対数をとるかどうかの選択です。デフォルトでは先程説明したとおり自動検出です。左の項目はプラットフォームの注釈の選択です。&quot;NCBI generated&quot; がある場合はそれの方が信頼できます。</li>
<li>20. Options に変更を加えたら、GEO2R タブに戻って &quot;Recalculate&quot; をクリックします。 変更を反映した計算結果が表示され、多重検定の補正法を変更したため、adj.P.Val が変わっていることがわかります。</li>
<li>21. Profile graph の項目では、プローブ ID を元に、個々の遺伝子の発現状況を調べることができます。</li>
<li>22. 「View data for (platform ID)」をpクリックするとプラットフォームの情報が表示されるので、目的の遺伝子のプローブ ID を、ブラウザの検索機能 (Ctrl+F)を用いて調べます。今回は例としてNFE2L2（酸化ストレスによって活性化する転写因子）を検索してみましょう。</li>
<li>23. 一番左がプローブIDなので、これをコピーし、さきほどの&quot;Enter ID&quot; の窓にプローブ ID をペーストし、&quot;Set&quot; をクリックすると。発現量のグラフが表示されます。（なおこの操作では、何の計算も実行されないので、検定の結果の P 値を調べることはできません。）</li>
<li>24. R script タブをクリックするとこれまでに実際に実行された R のスクリプトを見ることができます。これを参考に、手元の R でパラメータを調整するなどして更なる解析を行うことができます。</li>
<li>R の使い方については、下記の統合TV のコンテンツ「統計解析ソフト「R」の使い方」シリーズをご覧ください。</li>
<li><a href="http://togotv.dbcls.jp/20090618.html#p01" rel="nofollow">統計解析ソフト「R」の使い方 ～導入編～</a></li>
<li><a href="http://togotv.dbcls.jp/20091219.html#p01" rel="nofollow">統計解析ソフト「R」の使い方 ～ヒートマップ編～</a></li>
<li><a href="http://togotv.dbcls.jp/20111107.html#p01" rel="nofollow">統計解析ソフト「R」での立廻り</a></li></ul>

<h3 id="content_1_15"><a id="a83d5bfe" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#a83d5bfe" title="a83d5bfe">_</a> 【実習7】GEOを使って、自分の興味のある遺伝子の（ある実験条件下における）発現状況を調べる  </h3>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li><a href="http://togotv.dbcls.jp/20111020.html#p01" rel="nofollow">【復習用】NCBI GEOの使い方2～遺伝子プロファイルの検索・処理済みデータの取得～ 2011</a> <a href="http://lifesciencedb.jp/image/small_video_icon.png" rel="nofollow"><img src="http://lifesciencedb.jp/image/small_video_icon.png" alt="http://lifesciencedb.jp/image/small_video_icon.png" /></a></li>
<li>1. <a href="http://www.ncbi.nlm.nih.gov/geo/" rel="nofollow">http://www.ncbi.nlm.nih.gov/geo/</a>を開きます。</li>
<li>2.「Gene profiles」に自分の検索したい遺伝子名を入力します。</li>
<li>3. 今回は例として「<a href="http://www.google.co.jp/search?hl=ja&amp;q=Nanog%E9%81%BA%E4%BC%9D%E5%AD%90" rel="nofollow">nanog</a>」という遺伝子を検索してみましょう。入力終了後、「GO」をクリックします。</li>
<li>4. GEOに登録されている様々な実験条件で行なわれたマイクロアレイ実験における「nanog」遺伝子の発現データが表示されます。</li>
<li>5. 検索結果の右端にある画像をクリックすると、<a href="http://www.ncbi.nlm.nih.gov/geo/gds/profileGraph.cgi?&amp;dataset=DEAryz&amp;dataset=yyyzzz$&amp;gmin=5173.000000&amp;gmax=11680.000000&amp;absc=&amp;gds=2294&amp;idref=161072_at&amp;annot=Nanog" rel="nofollow">発現データの詳細をみる</a>ことができます。</li>
<li>6. <a href="http://www.ncbi.nlm.nih.gov/sites/GDSbrowser?acc=GDS2294" rel="nofollow">このサンプル（GDS2294）</a>では、nanogはどういう細胞のどういう実験条件で発現が増減しているか調べてみましょう。</li>
<li>7. ページ下部の「samples」に列挙された<a href="http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSM130365" rel="nofollow">リンク</a>をクリックすると、そのサンプル（一枚のマイクロアレイ）の詳細を閲覧できます。</li>
<li>8. <a href="http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSM130365" rel="nofollow">リンク先のページ</a>の中ほどにある<a href="http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE5583" rel="nofollow">「series」のリンク</a>をクリックすると、この実験全体の詳細情報が見られます。</li>
<li>9. <a href="http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE5583" rel="nofollow">この実験全体の詳細情報ページ</a>の下部にある<a href="ftp://ftp.ncbi.nih.gov/pub/geo/DATA/SeriesMatrix/GSE5583/" rel="nofollow">「Series Matrix File(s)」</a>をクリックすると、この実験の正規化補正済みのマイクロアレイデータをダウンロードすることができます。</li></ul>

<h3 id="content_1_16"><a id="ze44dc22" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#ze44dc22" title="ze44dc22">_</a> 【実習8】GEOを使って、自分の興味のあるマイクロアレイ実験データセットを検索&amp;生データをダウンロードする  </h3>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li><a href="http://togotv.dbcls.jp/20110711.html#p01" rel="nofollow">【復習用】NCBI GEOの使い方1～マイクロアレイデータの検索・取得～ 2011</a> <a href="http://lifesciencedb.jp/image/small_video_icon.png" rel="nofollow"><img src="http://lifesciencedb.jp/image/small_video_icon.png" alt="http://lifesciencedb.jp/image/small_video_icon.png" /></a></li>
<li>1. <a href="http://www.ncbi.nlm.nih.gov/geo/" rel="nofollow">http://www.ncbi.nlm.nih.gov/geo/</a>を開きます。</li>
<li>2. 画面中央の「Platforms」をクリックします。</li>
<li>3. <a href="http://www.informatics.jax.org/javawi2/servlet/WIFetch?page=imageSummaryByMrk&amp;key=25000&amp;imageType=8" rel="nofollow">Platform(マイクロアレイの種類)の一覧画面が現れる</a>ので、上部の「FIND PLATFORM」をクリックします。</li>
<li>4. <a href="http://www.ncbi.nlm.nih.gov/geo/query/browse.cgi?mode=findplatform" rel="nofollow">platformの検索画面</a>が現れるので、「Company name」に「Affymetrix」、「organism」に「Homo sapiens」を選択し、「FIND PLATFORM」をクリックします。</li>
<li>5. <a href="http://www.ncbi.nlm.nih.gov/geo/query/browse.cgi?mode=foundplatform" rel="nofollow">Affymetrixのヒトのマイクロアレイの検索結果</a>が表示されるので、中程にある「Affymetrix GeneChip Human Genome U133 Plus 2.0 Array」の左端にある<a href="http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GPL570" rel="nofollow">「GPL570」というID</a>をクリックします。</li>
<li>6. <a href="http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GPL570" rel="nofollow">表示された画面</a>の真ん中あたりにある「series」下の「More...」をクリックすると、登録されているデータセットを閲覧できます。</li>
<li>7. ブラウザの検索ボタンなどを使って「reprogramming」という単語を検索するとどういうデータがヒットするでしょうか？</li>
<li>8. ヒットしたデータの左端にあるIDをクリックすると、<a href="http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE9832" rel="nofollow">そのデータセットの詳細情報</a>が閲覧できます</li>
<li>9. ページ下部の「Download family」の中にある「Series Matrix File(s)」をクリックすると正規化済みのデータのダウンロードリンクが表示されます。</li>
<li>10. ページ最下部の「Supplementary file」にあるリンクから生データをダウンロードすることができます。</li>
<li>11. 自分の研究テーマに近い、また興味のあるマイクロアレイデータが利用可能か検索してみましょう。</li></ul>

<h3 id="content_1_17"><a id="b6353d6e" href="http://MotDB.DBCLS.jp/?AJACS36%2Fge#b6353d6e" title="b6353d6e"><span class="sanchor">_</span></a> 【参考1】<a href="http://lifesciencedb.jp/geo/" rel="nofollow">遺伝子発現バンク(GEO)目次、通称「GEO目次」</a>  </h3>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li><a href="http://togotv.dbcls.jp/20080623.html#p01" rel="nofollow">使い方参考動画 遺伝子発現バンク(GEO)目次を使い倒す－その壱</a> <a href="http://lifesciencedb.jp/image/small_video_icon.png" rel="nofollow"><img src="http://lifesciencedb.jp/image/small_video_icon.png" alt="http://lifesciencedb.jp/image/small_video_icon.png" /></a></li>
<li>NCBI GEO を日本語のインターフェイスで快適に使い、データの全容を俯瞰するための仕組みです。数多く登録されている遺伝子発現データの大まかな傾向をつかむのに役に立つことでしょう。</li>
<li>検索結果のRSS配信機能があるので、これを活用して、遺伝子発現データの新規登録の有無をチェックできます（便利！）。</li></ul>
