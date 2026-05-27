const questions = [
  { text: "旅行前、GoogleMapの保存が増えていく", axis: "P", reverse: false },
  { text: "当日予定変更はむしろ楽しい", axis: "P", reverse: true },
  { text: "旅程が埋まっていないと少し不安", axis: "P", reverse: false },
  { text: "現地で偶然見つけた店に入りたい", axis: "P", reverse: true },
  { text: "移動時間まで細かく考える", axis: "P", reverse: false },
  { text: "『とりあえず歩く』が好き", axis: "P", reverse: true },
  { text: "予約が取れていないと落ち着かない", axis: "P", reverse: false },
  { text: "旅行は予定通りに進まなくていい", axis: "P", reverse: true },

  { text: "朝から予定を詰め込みたい", axis: "A", reverse: false },
  { text: "旅行中もカフェ休憩はかなり重要", axis: "A", reverse: true },
  { text: "『せっかくだから』で予定が増える", axis: "A", reverse: false },
  { text: "宿でのんびりする時間が必要", axis: "A", reverse: true },
  { text: "1日に複数スポット回りたい", axis: "A", reverse: false },
  { text: "移動だけで疲れやすい", axis: "A", reverse: true },
  { text: "夜まで動き続けても平気", axis: "A", reverse: false },
  { text: "旅行先では余白時間を残したい", axis: "A", reverse: true },

  { text: "景色や空間の写真を撮りたくなる", axis: "V", reverse: false },
  { text: "有名スポットより現地の空気感が好き", axis: "V", reverse: true },
  { text: "旅行先の写真フォルダが大量になる", axis: "V", reverse: false },
  { text: "『映えるか』より『楽しいか』を優先", axis: "V", reverse: true },
  { text: "おしゃれなカフェやホテルに惹かれる", axis: "V", reverse: false },
  { text: "ローカルな食堂にワクワクする", axis: "V", reverse: true },
  { text: "旅行中、写真を撮るために立ち止まる", axis: "V", reverse: false },
  { text: "観光名所より街歩きが好き", axis: "V", reverse: true },

  { text: "旅行では宿にお金をかけたい", axis: "L", reverse: false },
  { text: "移動費はできるだけ抑えたい", axis: "L", reverse: true },
  { text: "『せっかくなら良い店』が口癖", axis: "L", reverse: false },
  { text: "コスパの良い穴場を探すのが好き", axis: "L", reverse: true },
  { text: "タクシー移動に抵抗が少ない", axis: "L", reverse: false },
  { text: "安く旅行を攻略するのが楽しい", axis: "L", reverse: true },
  { text: "旅先では多少贅沢したい", axis: "L", reverse: false },
  { text: "節約できると少し嬉しい", axis: "L", reverse: true },
];

const roleMap = {
  PAVL: "旅演出家",
  PAVS: "景色収集家",
  PAEL: "感性探訪家",
  PAES: "路地開拓士",
  PCVL: "余白貴族",
  PCVS: "カフェ漂流家",
  PCEL: "癒し滞在家",
  PCES: "静かな放浪家",
  FAVL: "夜更かし演出家",
  FAVS: "映え放浪家",
  FAEL: "自由探検家",
  FAES: "気まぐれ開拓士",
  FCVL: "月夜の漂流家",
  FCVS: "余白収集家",
  FCEL: "空気感旅行家",
  FCES: "風まかせ人"
};

const quiz = document.getElementById("quiz");

questions.forEach((q, index) => {
  const div = document.createElement("div");
  div.className = "question";

  div.innerHTML = `
    <p>${index + 1}. ${q.text}</p>
    <div class="options">
      ${[1,2,3,4,5].map(v => `
        <label>
          <input type="radio" name="q${index}" value="${v}">
          ${["かなりそう思う","ややそう思う","どちらでもない","あまり思わない","全く思わない"][v-1]}
        </label>
      `).join("")}
    </div>
  `;

  quiz.appendChild(div);
});

document.getElementById("submitBtn").addEventListener("click", () => {
  const scores = {
    P: 0,
    A: 0,
    V: 0,
    L: 0
  };

  for (let i = 0; i < questions.length; i++) {
    const checked = document.querySelector(`input[name="q${i}"]:checked`);

    if (!checked) {
      alert(`${i + 1}問目が未回答です`);
      return;
    }

    let value = Number(checked.value);
    const q = questions[i];

    if (q.reverse) {
      value = 6 - value;
    }

    scores[q.axis] += value;
  }

  const type =
    (scores.P >= 24 ? "P" : "F") +
    (scores.A >= 24 ? "A" : "C") +
    (scores.V >= 24 ? "V" : "E") +
    (scores.L >= 24 ? "L" : "S");

  const role = roleMap[type];

  const result = document.getElementById("result");
  result.classList.remove("hidden");

  result.innerHTML = `
    <div class="result-card">
      <h2>${type}</h2>
      <h1>${role}</h1>
      <p>あなたは「${role}」タイプです。</p>
      <p>旅先での価値観と行動スタイルから判定されています。</p>
    </div>
  `;

  window.scrollTo({
    top: document.body.scrollHeight,
    behavior: "smooth"
  });
});
