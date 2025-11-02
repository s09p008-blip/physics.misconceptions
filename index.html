<!doctype html>
<html lang="ja">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>高校物理 素朴概念ネットワーク</title>
  <meta name="description" content="高校物理の素朴概念データベース（GitHub Pages で公開するためのシンプルなHTML版）" />
  <!-- Tailwind CDN for styling (works for demo / GitHub Pages) -->
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gradient-to-br from-blue-50 to-indigo-100 min-h-screen">
  <div id="root" class="p-6"></div>

  <!-- React + ReactDOM (開発用) -->
  <script crossorigin src="https://unpkg.com/react@18/umd/react.development.js"></script>
  <script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
  <!-- Babel for in-browser JSX transpile (簡易デモ用) -->
  <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>

  <!-- アプリ本体（JSX） -->
  <script type="text/babel">
    // 簡易アイコンコンポーネント（元の lucide-react の代替）
    const Icon = ({children, className}) => (
      <span className={className} style={{display:'inline-block'}}>{children}</span>
    );
    const Search = props => <Icon {...props}>🔍</Icon>;
    const Book = props => <Icon {...props}>📚</Icon>;
    const Users = props => <Icon {...props}>👥</Icon>;
    const Plus = props => <Icon {...props}>➕</Icon>;
    const X = props => <Icon {...props}>✖️</Icon>;
    const Tag = props => <Icon {...props}>🏷️</Icon>;
    const BookOpen = props => <Icon {...props}>📖</Icon>;
    const User = props => <Icon {...props}>👤</Icon>;

    // ...existing code...
    const INITIAL_DATA = [
      { id: 1, misconception: "速度と速さは同じもの", field: "力学", keywords: ["速度"], citation: "Aguirre, J. M. (1988)", isUserAdded: false },
      { id: 2, misconception: "物体の加速度は必ず速度と同じ方向を向く", field: "力学", keywords: ["速度", "加速度"], citation: "Reif, F., & Allen, S. (1992)", isUserAdded: false },
      { id: 3, misconception: "負の符号は向きを表すことを理解せず、\"値が小さい\"と解釈する", field: "力学", keywords: ["速度"], citation: "Goldberg, F. M., & Anderson, J. H. (1989)", isUserAdded: false },
      { id: 4, misconception: "位置が一致する瞬間には速度も等しいと考える（\"同位置＝同速度\"）", field: "力学", keywords: ["速度"], citation: "Driver, R., et al. (1994)", isUserAdded: false },
      { id: 5, misconception: "等速運動でも「動いているから加速度がある」と考える", field: "力学", keywords: ["速度", "加速度"], citation: "Trowbridge, D. E., & McDermott, L. C. (1981)", isUserAdded: false },
      { id: 6, misconception: "v-tグラフの傾きを理解せず、グラフの高さで加速度を判断する", field: "力学", keywords: ["速度", "加速度"], citation: "McDermott, L. C., Rosenquist, M. L., & van Zee, E. H. (1987)", isUserAdded: false },
      { id: 7, misconception: "v-tグラフで2つの線が交わると\"衝突する\"と考える", field: "力学", keywords: ["速度"], citation: ". (1985)", isUserAdded: false },
      { id: 8, misconception: "真空中では物体は運動できない、または真空中では全ての物体が静止する", field: "力学", keywords: ["力"], citation: "Sjoberg, S., & Lie, S. (1981)", isUserAdded: false },
      { id: 9, misconception: "重力は地球の大気によるもの", field: "力学", keywords: ["重力"], citation: "Driver et al. (1994)", isUserAdded: false },
      { id: 10, misconception: "力＝速度と考え、「速く動いている＝大きな力が働いている」と捉える", field: "力学", keywords: ["力", "速度"], citation: "Viennot, L. (1979)", isUserAdded: false },
      { id: 11, misconception: "速度がゼロなら、その瞬間に力もゼロになる", field: "力学", keywords: ["力", "速度"], citation: "Driver et al. (1994)", isUserAdded: false },
      { id: 12, misconception: "物体に複数の力が働いている時、最も大きい力の方向に運動する", field: "力学", keywords: ["力"], citation: "Driver, R., et al. (1994)", isUserAdded: false },
      { id: 13, misconception: "投げたボールが空中にある時、手の力がまだボールに伝わり続けている", field: "力学", keywords: ["力"], citation: "McCloskey, M. (1983)", isUserAdded: false },
      { id: 14, misconception: "「作用反作用」を同一物体に働く2つの力だと誤解する", field: "力学", keywords: ["力"], citation: "Halloun, I. A., & Hestenes, D. (1985)", isUserAdded: false },
      { id: 15, misconception: "重い物の方が速く落ちる", field: "力学", keywords: ["重力"], citation: "Gunstone, R. F., & White, R. T. (1981)", isUserAdded: false },
      { id: 16, misconception: "等速直線運動では力が働いていない", field: "力学", keywords: ["力", "速度"], citation: "Viennot, L. (1979)", isUserAdded: false },
      { id: 17, misconception: "止まっている物体には力が働いていない", field: "力学", keywords: ["力"], citation: "Minstrell, J. (1982)", isUserAdded: false },
      { id: 18, misconception: "斜面上の静止物体には、垂直抗力しか働いていないと考える", field: "力学", keywords: ["力"], citation: "Brown, D. E. (1989)", isUserAdded: false },
      { id: 19, misconception: "摩擦力は常に運動と逆向きだけでなく、静止した物体には働かない", field: "力学", keywords: ["力"], citation: "Clough & Driver (1985)", isUserAdded: false },
      { id: 20, misconception: "空気抵抗が物体を減速させるのではなく、\"力が使い果たされる\"", field: "力学", keywords: ["力"], citation: "Biddulph, F., & Osborne, R. (1984)", isUserAdded: false },
      { id: 21, misconception: "摩擦や空気抵抗がエネルギーを\"消滅\"させる", field: "力学", keywords: ["エネルギー"], citation: "Engel Clough, E., & Driver, R. (1985)", isUserAdded: false },
      { id: 22, misconception: "エネルギーは使うと無くなる物質のようなもの", field: "力学", keywords: ["エネルギー"], citation: "Bryce, T. G., & MacMillan, K. (2009)", isUserAdded: false },
      { id: 23, misconception: "エネルギー保存則は「運動エネルギーは常に一定」を意味すると誤解", field: "力学", keywords: ["エネルギー"], citation: "Singh, C., & Rosengrant, D. (2003)", isUserAdded: false },
      { id: 24, misconception: "運動量と運動エネルギーを混同する", field: "力学", keywords: ["エネルギー", "運動量"], citation: "McCloskey, M. (1983)", isUserAdded: false },
      { id: 25, misconception: "衝突後、2つの物体の運動エネルギーは必ず等しくなる", field: "力学", keywords: ["エネルギー"], citation: "Singh, C., & Rosengrant, D. (2003)", isUserAdded: false },
      { id: 26, misconception: "熱と温度を同一視する", field: "熱", keywords: ["熱", "温度"], citation: "Erickson, G. L., & Tiberghien, A. (1985)", isUserAdded: false },
      { id: 27, misconception: "熱は物質であり、物体間を移動する", field: "熱", keywords: ["熱"], citation: "Engel Clough, E., & Driver, R. (1985)", isUserAdded: false },
      { id: 28, misconception: "金属は\"冷たい\"性質を持ち、木は\"暖かい\"性質を持つ", field: "熱", keywords: ["熱", "温度"], citation: "Driver, R., et al. (1994)", isUserAdded: false },
      { id: 29, misconception: "物質が状態変化すると分子の質量や大きさが変わる", field: "熱", keywords: ["熱"], citation: "Adadan, E., & Yavuzkaya, M. N. (2018)", isUserAdded: false },
      { id: 30, misconception: "沸騰中の水の温度は上昇し続ける", field: "熱", keywords: ["熱", "温度"], citation: "fgren, L. (2000)", isUserAdded: false },
      { id: 31, misconception: "蒸発は高温でのみ起こる現象", field: "熱", keywords: ["熱"], citation: "Lewis, E. L., & Linn, M. C. (1994)", isUserAdded: false },
      { id: 32, misconception: "音波は\"物質的な塊\"として空間を伝わる", field: "波・光", keywords: ["音", "波"], citation: "Caleon, I., & Subramaniam, R. (2010)", isUserAdded: false },
      { id: 33, misconception: "音は真空中も伝わる", field: "波・光", keywords: ["音", "波"], citation: "Caleon, I., & Subramaniam, R. (2010)", isUserAdded: false },
      { id: 34, misconception: "音の高さ（振動数）と音の大きさ（振幅）を混同する", field: "波・光", keywords: ["音", "波"], citation: "Caleon, I., & Subramaniam, R. (2010)", isUserAdded: false },
      { id: 35, misconception: "音は「物質的な塊」として伝わる", field: "波・光", keywords: ["音", "波"], citation: "Barman, C. R., Barman, N. S., & Miller, J. A. (1996)", isUserAdded: false },
      { id: 36, misconception: "エコーは音が\"反射\"ではなく\"跳ね返ってくる\"", field: "波・光", keywords: ["音", "波"], citation: "Caleon, I., & Subramaniam, R. (2010)", isUserAdded: false },
      { id: 37, misconception: "光は目から出て対象物を\"見る\"", field: "波・光", keywords: ["光"], citation: "Guesne, E. (1985)", isUserAdded: false },
      { id: 38, misconception: "暗闇では\"何も見えない\"のは、光がないから\"目が働かない\"", field: "波・光", keywords: ["光"], citation: "Guesne (1985)", isUserAdded: false },
      { id: 39, misconception: "影は光が\"遮られてできる黒い物質\"", field: "波・光", keywords: ["光"], citation: "Goldberg & McDermott (1987)", isUserAdded: false },
      { id: 40, misconception: "鏡の像は鏡の表面にある", field: "波・光", keywords: ["光"], citation: "Galili, I., & Hazan, A. (2000)", isUserAdded: false },
      { id: 41, misconception: "光の反射角は入射角より常に小さい", field: "波・光", keywords: ["光"], citation: "Galili, I., & Hazan, A. (2000)", isUserAdded: false },
      { id: 42, misconception: "波の伝播速度と媒質の振動速度を混同する", field: "波・光", keywords: ["波"], citation: "Zylbersztajn, A., & Watts, M. (1982)", isUserAdded: false },
      { id: 43, misconception: "屈折は光が\"曲がる\"現象", field: "波・光", keywords: ["光"], citation: "Galili, I., & Hazan, A. (2000)", isUserAdded: false },
      { id: 44, misconception: "レンズを通る光はすべて焦点を通る", field: "波・光", keywords: ["光"], citation: "Bryan, J. A., & Slough, S. W. (2009)", isUserAdded: false },
      { id: 45, misconception: "凸レンズの焦点距離より内側に物体を置くと像はできない", field: "波・光", keywords: ["光"], citation: "Goldberg, F. M., & McDermott, L. C. (1987)", isUserAdded: false },
      { id: 46, misconception: "地震波は地球内部を直進する", field: "波・光", keywords: ["波"], citation: "Libarkin, J. C., et al. (2015)", isUserAdded: false },
      { id: 47, misconception: "電磁波（光・電波）も音波と同じ\"振動\"の一種", field: "波・光", keywords: ["光", "波"], citation: "Neumann, K., & Hopf, M. (2012)", isUserAdded: false },
      { id: 48, misconception: "電池は\"一定の電流\"を供給する装置", field: "電磁気", keywords: ["電流", "回路"], citation: "Engelhardt, P. V., & Beichner, R. J. (2004)", isUserAdded: false },
      { id: 49, misconception: "電流は回路を回る間に\"消費\"される", field: "電磁気", keywords: ["電流", "回路"], citation: "Engelhardt, P. V., & Beichner, R. J. (2004)", isUserAdded: false },
      { id: 50, misconception: "電流は電池の両極から出て、電球で\"衝突\"して光る", field: "電磁気", keywords: ["電流", "回路"], citation: "Shipstone (1984)", isUserAdded: false },
      { id: 51, misconception: "並列回路では、各枝の電流は等しい", field: "電磁気", keywords: ["電流", "回路"], citation: "Moodley, K., & Gaigher, E. (2019)", isUserAdded: false },
      { id: 52, misconception: "電圧は\"電流の強さ\"を表す", field: "電磁気", keywords: ["電流", "電圧", "回路"], citation: "Engelhardt, P. V., & Beichner, R. J. (2004)", isUserAdded: false },
      { id: 53, misconception: "全ての金属が磁石に引き寄せられる", field: "電磁気", keywords: ["磁場"], citation: "Hickey, R., & Schibeci, R. A. (1999)", isUserAdded: false },
      { id: 54, misconception: "磁場は\"目に見えない糸\"のようなもの", field: "電磁気", keywords: ["磁場"], citation: "Driver, R., et al. (1994)", isUserAdded: false },
      { id: 55, misconception: "電流が流れると磁場が\"発生\"し、電流が止まると磁場は\"消滅\"する", field: "電磁気", keywords: ["電流", "磁場"], citation: "Stocklmayer (1994)", isUserAdded: false },
      { id: 56, misconception: "電磁誘導は磁石が\"電気を作り出す\"現象", field: "電磁気", keywords: ["磁場"], citation: "Saglam, M., & Millar, R. (2006)", isUserAdded: false },
      { id: 57, misconception: "コイルの巻数が多いほど誘導電流は必ず大きくなる", field: "電磁気", keywords: ["電流", "磁場"], citation: "Saglam, M., & Millar, R. (2006)", isUserAdded: false },
      { id: 58, misconception: "変圧器は\"電流を増やす\"装置", field: "電磁気", keywords: ["電流", "電圧"], citation: "Jelicic, K., et al. (2017)", isUserAdded: false },
      { id: 59, misconception: "放射線を浴びた物体は放射能を持つようになる", field: "放射線", keywords: ["放射線"], citation: "Millar & Gill (1996)", isUserAdded: false },
      { id: 60, misconception: "放射線はすべて人工的なもの", field: "放射線", keywords: ["放射線"], citation: "Millar, R., & Gill, J. S. (1996)", isUserAdded: false },
      { id: 61, misconception: "α線・β線・γ線は本質的に同じもの", field: "放射線", keywords: ["放射線"], citation: "Millar & Gill (1996)", isUserAdded: false }
    ];

    // PhysicsMisconceptionsNetwork コンポーネント（元ファイルを簡易的にブラウザで動かすために一部調整）
    const { useState, useEffect } = React;

    const PhysicsMisconceptionsNetwork = () => {
      const [data, setData] = useState([]);
      const [searchTerm, setSearchTerm] = useState('');
      const [selectedField, setSelectedField] = useState('全て');
      const [selectedItem, setSelectedItem] = useState(null);
      const [userNotes, setUserNotes] = useState({});
      const [showAddNote, setShowAddNote] = useState(false);
      const [newNote, setNewNote] = useState('');
      const [showAddForm, setShowAddForm] = useState(false);
      const [newMisconception, setNewMisconception] = useState({
        misconception: '',
        field: '力学',
        keywords: '',
        citation: '',
        contributorName: '',
        contributorSchool: ''
      });

      useEffect(() => {
        const savedData = localStorage.getItem('physicsMisconceptionsData');
        const savedNotes = localStorage.getItem('physicsMisconceptionsNotes');
        if (savedData) {
          setData(JSON.parse(savedData));
        } else {
          setData(INITIAL_DATA);
          localStorage.setItem('physicsMisconceptionsData', JSON.stringify(INITIAL_DATA));
        }
        if (savedNotes) setUserNotes(JSON.parse(savedNotes));
      }, []);

      const saveNote = (id) => {
        if (newNote.trim()) {
          const updated = {
            ...userNotes,
            [id]: [...(userNotes[id] || []), { 
              text: newNote, 
              date: new Date().toLocaleDateString('ja-JP'),
              time: new Date().toLocaleTimeString('ja-JP')
            }]
          };
          setUserNotes(updated);
          localStorage.setItem('physicsMisconceptionsNotes', JSON.stringify(updated));
          setNewNote('');
          setShowAddNote(false);
        }
      };

      const addNewMisconception = () => {
        if (newMisconception.misconception.trim() && newMisconception.contributorName.trim()) {
          const keywordsArray = newMisconception.keywords
            .split(/[,、\s]+/)
            .filter(k => k.trim())
            .map(k => k.trim());
          const maxId = Math.max(...data.map(item => item.id), 0);
          let contributorInfo = newMisconception.contributorName.trim();
          if (newMisconception.contributorSchool.trim()) {
            contributorInfo += ` (${newMisconception.contributorSchool.trim()})`;
          }
          const newItem = {
            id: maxId + 1,
            misconception: newMisconception.misconception.trim(),
            field: newMisconception.field,
            keywords: keywordsArray,
            citation: newMisconception.citation.trim() || '現場の先生からの報告',
            isUserAdded: true,
            contributor: contributorInfo,
            addedDate: new Date().toLocaleDateString('ja-JP')
          };
          const updatedData = [...data, newItem];
          setData(updatedData);
          localStorage.setItem('physicsMisconceptionsData', JSON.stringify(updatedData));
          setNewMisconception({
            misconception: '',
            field: '力学',
            keywords: '',
            citation: '',
            contributorName: '',
            contributorSchool: ''
          });
          setShowAddForm(false);
          alert('✅ 新しい素朴概念を追加しました！ご協力ありがとうございます！');
        } else {
          alert('⚠️ 素朴概念の説明とお名前は必須項目です');
        }
      };

      const resetData = () => {
        if (confirm('全てのデータを初期状態に戻しますか？（ユーザーが追加した素朴概念とメモが削除されます）')) {
          setData(INITIAL_DATA);
          setUserNotes({});
          localStorage.setItem('physicsMisconceptionsData', JSON.stringify(INITIAL_DATA));
          localStorage.removeItem('physicsMisconceptionsNotes');
          alert('✅ データをリセットしました');
        }
      };

      const filteredData = data.filter(item => {
        const matchesSearch = item.misconception.toLowerCase().includes(searchTerm.toLowerCase()) ||
                             item.keywords.some(k => k.includes(searchTerm));
        const matchesField = selectedField === '全て' || item.field === selectedField;
        return matchesSearch && matchesField;
      });

      const fields = ['全て', '力学', '熱', '波・光', '電磁気', '放射線'];
      const userAddedCount = data.filter(item => item.isUserAdded).length;

      return (
        <div className="min-h-screen p-6 max-w-7xl mx-auto">
          <header className="bg-white rounded-lg shadow-lg p-6 mb-6">
            <h1 className="text-4xl font-bold text-indigo-900 mb-2">高校物理 素朴概念ネットワーク</h1>
            <p className="text-gray-600 mb-4">生徒の理解を深めるための、全国の先生方で育てる実践的データベース</p>
            <div className="flex items-center gap-4 text-sm text-gray-500 flex-wrap">
              <div className="flex items-center gap-2"><Book className="w-4 h-4" />
                <span>論文ベース: {INITIAL_DATA.length}件</span>
              </div>
              <div className="flex items-center gap-2"><Users className="w-4 h-4" />
                <span>現場から追加: {userAddedCount}件</span>
              </div>
              <div className="flex items-center gap-2"><BookOpen className="w-4 h-4" />
                <span className="font-semibold">総計: {data.length}件</span>
              </div>
            </div>
          </header>

          <div className="bg-white rounded-lg shadow-lg p-6 mb-6">
            <div className="flex gap-4 mb-4">
              <div className="flex-1 relative">
                <Search className="absolute left-3 top-3 text-gray-400 w-5 h-5" />
                <input
                  type="text"
                  placeholder="キーワードで検索（例: 速度, エネルギー, 光）"
                  className="w-full pl-10 pr-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500 focus:border-transparent"
                  value={searchTerm}
                  onChange={(e) => setSearchTerm(e.target.value)}
                />
              </div>
              <button onClick={() => setShowAddForm(true)} className="flex items-center gap-2 px-6 py-2 bg-green-600 text-white rounded-lg hover:bg-green-700 font-medium transition-colors whitespace-nowrap">
                <Plus className="w-5 h-5" />
                新規追加
              </button>
            </div>

            <div className="flex gap-2 flex-wrap mb-4">
              {fields.map(field => (
                <button key={field} onClick={() => setSelectedField(field)} className={`px-4 py-2 rounded-lg font-medium transition-colors ${selectedField === field ? 'bg-indigo-600 text-white' : 'bg-gray-200 text-gray-700 hover:bg-gray-300'}`}>
                  {field}
                </button>
              ))}
            </div>

            <div className="flex justify-between items-center">
              <div className="text-sm text-gray-600">{filteredData.length}件の素朴概念が見つかりました</div>
              <button onClick={resetData} className="text-sm text-red-600 hover:text-red-800 underline">データをリセット</button>
            </div>
          </div>

          {/* 新規追加フォーム（簡易） */}
          {showAddForm && (
            <div className="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 z-50" onClick={() => setShowAddForm(false)}>
              <div className="bg-white rounded-lg max-w-2xl w-full max-h-[90vh] overflow-y-auto p-6" onClick={(e) => e.stopPropagation()}>
                <div className="flex justify-between items-center mb-4">
                  <h2 className="text-2xl font-bold text-indigo-900">新しい素朴概念を追加</h2>
                  <button onClick={() => setShowAddForm(false)} className="text-gray-500 hover:text-gray-700"><X className="w-6 h-6" /></button>
                </div>
                <div className="space-y-4">
                  <div className="bg-yellow-50 border-l-4 border-yellow-500 p-4 mb-4">
                    <div className="flex items-start">
                      <User className="w-5 h-5 text-yellow-600 mt-0.5 mr-2" />
                      <div>
                        <p className="text-sm font-medium text-yellow-800">貢献者情報</p>
                        <p className="text-xs text-yellow-700 mt-1">あなたの発見を全国の先生方と共有しましょう！お名前を記録させていただきます。</p>
                      </div>
                    </div>
                  </div>

                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">お名前（ニックネーム可）<span className="text-red-500">*</span></label>
                    <input type="text" value={newMisconception.contributorName} onChange={(e) => setNewMisconception({...newMisconception, contributorName: e.target.value})} className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500" placeholder="例: 田中 太郎 / タナカ先生 / たなか" />
                  </div>

                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">学校名・地域（オプション）</label>
                    <input type="text" value={newMisconception.contributorSchool} onChange={(e) => setNewMisconception({...newMisconception, contributorSchool: e.target.value})} className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500" placeholder="例: 〇〇高校 / 東京都 / 関東地方" />
                    <p className="text-xs text-gray-500 mt-1">任意項目です。プライバシーに配慮して記入してください</p>
                  </div>

                  <hr className="my-4" />

                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">分野 <span className="text-red-500">*</span></label>
                    <select value={newMisconception.field} onChange={(e) => setNewMisconception({...newMisconception, field: e.target.value})} className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500">
                      <option value="力学">力学</option>
                      <option value="熱">熱</option>
                      <option value="波・光">波・光</option>
                      <option value="電磁気">電磁気</option>
                      <option value="放射線">放射線</option>
                    </select>
                  </div>

                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">素朴概念の説明 <span className="text-red-500">*</span></label>
                    <textarea value={newMisconception.misconception} onChange={(e) => setNewMisconception({...newMisconception, misconception: e.target.value})} className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500" rows="4" placeholder="例: 電流は回路を回る間に消費される" />
                  </div>

                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">キーワード/ハッシュタグ（カンマ区切り）</label>
                    <div className="flex items-start gap-2">
                      <Tag className="w-5 h-5 text-gray-400 mt-2" />
                      <input type="text" value={newMisconception.keywords} onChange={(e) => setNewMisconception({...newMisconception, keywords: e.target.value})} className="flex-1 px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500" placeholder="例: 電流, 回路, 電圧" />
                    </div>
                    <p className="text-xs text-gray-500 mt-1">複数のキーワードはカンマ（,）で区切ってください</p>
                  </div>

                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">状況・出典（オプション）</label>
                    <input type="text" value={newMisconception.citation} onChange={(e) => setNewMisconception({...newMisconception, citation: e.target.value})} className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500" placeholder="例: 2年生の授業中に複数の生徒から" />
                  </div>

                  <div className="flex gap-3 pt-4">
                    <button onClick={addNewMisconception} disabled={!newMisconception.misconception.trim() || !newMisconception.contributorName.trim()} className="flex-1 px-6 py-3 bg-green-600 text-white rounded-lg hover:bg-green-700 font-medium disabled:bg-gray-300 disabled:cursor-not-allowed transition-colors">追加する</button>
                    <button onClick={() => setShowAddForm(false)} className="px-6 py-3 bg-gray-300 text-gray-700 rounded-lg hover:bg-gray-400 font-medium transition-colors">キャンセル</button>
                  </div>
                </div>
              </div>
            </div>
          )}

          <div className="grid md:grid-cols-2 lg:grid-cols-3 gap-4">
            {filteredData.map(item => (
              <div key={item.id} className="bg-white rounded-lg shadow-md p-4 hover:shadow-xl transition-shadow cursor-pointer relative" onClick={() => setSelectedItem(item)}>
                {item.isUserAdded && (
                  <div className="absolute top-2 right-2"><span className="bg-green-100 text-green-800 text-xs px-2 py-1 rounded-full font-medium">👤 追加</span></div>
                )}
                <div className="flex justify-between items-start mb-2">
                  <span className="text-xs font-bold text-indigo-600">No.{item.id}</span>
                  <span className={`text-xs px-2 py-1 rounded-full ${item.field === '力学' ? 'bg-blue-100 text-blue-800' : item.field === '熱' ? 'bg-red-100 text-red-800' : item.field === '波・光' ? 'bg-yellow-100 text-yellow-800' : item.field === '電磁気' ? 'bg-purple-100 text-purple-800' : 'bg-green-100 text-green-800'}`}
                    >
                    {item.field}
                  </span>
                </div>
                <p className="text-gray-800 font-medium mb-2 line-clamp-3">{item.misconception}</p>
                <div className="flex flex-wrap gap-1 mb-2">{item.keywords.map((keyword, idx) => (<span key={idx} className="text-xs bg-gray-100 text-gray-600 px-2 py-1 rounded">#{keyword}</span>))}</div>
                {item.contributor && (<div className="text-xs text-green-600 mt-2">📌 {item.contributor}</div>)}
                {userNotes[item.id] && userNotes[item.id].length > 0 && (<div className="text-xs text-gray-500 mt-1">💡 {userNotes[item.id].length}件のメモ</div>)}
              </div>
            ))}
          </div>

          {selectedItem && (
            <div className="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 z-50" onClick={() => setSelectedItem(null)}>
              <div className="bg-white rounded-lg max-w-2xl w-full max-h-[90vh] overflow-y-auto p-6" onClick={(e) => e.stopPropagation()}>
                <div className="flex justify-between items-start mb-4">
                  <div className="flex items-center gap-2"><h2 className="text-2xl font-bold text-indigo-900">No.{selectedItem.id}</h2>
                    {selectedItem.isUserAdded && (<span className="bg-green-100 text-green-800 text-sm px-3 py-1 rounded-full font-medium">👤 現場から追加</span>)}
                  </div>
                  <button onClick={() => setSelectedItem(null)} className="text-gray-500 hover:text-gray-700"><X className="w-6 h-6" /></button>
                </div>

                <div className="mb-4"><span className={`inline-block px-3 py-1 rounded-full text-sm font-medium ${selectedItem.field === '力学' ? 'bg-blue-100 text-blue-800' : selectedItem.field === '熱' ? 'bg-red-100 text-red-800' : selectedItem.field === '波・光' ? 'bg-yellow-100 text-yellow-800' : selectedItem.field === '電磁気' ? 'bg-purple-100 text-purple-800' : 'bg-green-100 text-green-800'}`}>{selectedItem.field}</span></div>

                <h3 className="text-xl font-semibold mb-4">{selectedItem.misconception}</h3>

                <div className="mb-4"><h4 className="font-semibold text-gray-700 mb-2">キーワード:</h4><div className="flex flex-wrap gap-2">{selectedItem.keywords.map((keyword, idx) => (<span key={idx} className="bg-gray-100 text-gray-700 px-3 py-1 rounded-full text-sm">#{keyword}</span>))}</div></div>

                <div className="mb-4"><h4 className="font-semibold text-gray-700 mb-2">出典:</h4><p className="text-sm text-gray-600">{selectedItem.citation}</p></div>

                {selectedItem.contributor && (<div className="mb-4 bg-green-50 p-3 rounded-lg border border-green-200"><div className="flex items-center gap-2 mb-1"><User className="w-4 h-4 text-green-600" /><h4 className="font-semibold text-green-800 text-sm">貢献者</h4></div><p className="text-sm text-green-700">{selectedItem.contributor}</p>{selectedItem.addedDate && (<p className="text-xs text-green-600 mt-1">追加日: {selectedItem.addedDate}</p>)}</div>)}

                <div className="border-t pt-4">
                  <div className="flex justify-between items-center mb-3"><h4 className="font-semibold text-gray-700">先生方のメモ:</h4><button onClick={() => setShowAddNote(!showAddNote)} className="flex items-center gap-1 text-sm text-indigo-600 hover:text-indigo-800"><Plus className="w-4 h-4" />メモを追加</button></div>

                  {showAddNote && (<div className="mb-4 p-3 bg-gray-50 rounded-lg"><textarea className="w-full p-2 border border-gray-300 rounded-lg mb-2 focus:ring-2 focus:ring-indigo-500" rows="3" placeholder="授業での気づき、対応方法などを記入してください..." value={newNote} onChange={(e) => setNewNote(e.target.value)} /><div className="flex gap-2"><button onClick={() => saveNote(selectedItem.id)} className="px-4 py-2 bg-indigo-600 text-white rounded-lg hover:bg-indigo-700">保存</button><button onClick={() => {setShowAddNote(false); setNewNote('');}} className="px-4 py-2 bg-gray-300 text-gray-700 rounded-lg hover:bg-gray-400">キャンセル</button></div></div>)}

                  <div className="space-y-2">{userNotes[selectedItem.id] && userNotes[selectedItem.id].length > 0 ? userNotes[selectedItem.id].map((note, idx) => (<div key={idx} className="p-3 bg-indigo-50 rounded-lg"><p className="text-sm text-gray-800">{note.text}</p><p className="text-xs text-gray-500 mt-1">{note.date} {note.time}</p></div>)) : (<p className="text-sm text-gray-500 italic">まだメモがありません</p>)}</div>
                </div>
              </div>
            </div>
          )}

          <footer className="mt-8 text-center text-sm text-gray-600"><p>このデータベースは論文「高校物理教育における素朴概念の体系的分類」（BESTプロジェクトに基づく）から作成されました</p><p className="mt-2">© 2025 物理教育研究 | データはブラウザに保存されます</p><p className="mt-1 text-xs text-gray-500">全国の先生方のご協力により、このデータベースは成長し続けています</p></footer>
        </div>
      );
    };

    const root = ReactDOM.createRoot(document.getElementById('root'));
    root.render(<PhysicsMisconceptionsNetwork />);
  </script>
</body>
</html>
