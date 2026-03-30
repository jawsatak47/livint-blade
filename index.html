import { useState, useCallback } from "react";

const STYLES = `
@import url('https://fonts.googleapis.com/css2?family=Cinzel+Decorative:wght@400;700;900&family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400;1,500;1,600&family=Courier+Prime:ital,wght@0,400;0,700;1,400&display=swap');

*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

:root {
  --bg: #09080600;
  --ink: #0C0A07;
  --surface: #131008;
  --card: #161210;
  --border: #271F15;
  --border2: #3D3025;
  --red: #C01C14;
  --red2: #8A1310;
  --gold: #C4973E;
  --gold2: #9A7430;
  --purple: #6A4E9A;
  --green: #3A7250;
  --text: #E5D8C5;
  --text2: #C4B49C;
  --text3: #8A7A68;
  --text4: #5A4E40;
  --text5: #342A20;
}

html, body { height: 100%; background: var(--ink); }

.grain {
  position: fixed; inset: 0; pointer-events: none; z-index: 9000;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='400'%3E%3Cfilter id='g'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.8' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='400' height='400' filter='url(%23g)' opacity='0.045'/%3E%3C/svg%3E");
  mix-blend-mode: overlay;
}

.wrap {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 32px 24px;
  max-width: 680px;
  margin: 0 auto;
}

/* ──────────────── HOME ──────────────── */
.home { text-align: center; width: 100%; animation: fadeUp 1s ease both; }

.home-emblem {
  font-size: 44px;
  color: var(--red);
  margin-bottom: 32px;
  filter: drop-shadow(0 0 12px rgba(192,28,20,0.4));
  animation: breathe 4s ease-in-out infinite;
}
@keyframes breathe { 0%,100%{opacity:0.8;filter:drop-shadow(0 0 8px rgba(192,28,20,0.3))} 50%{opacity:1;filter:drop-shadow(0 0 20px rgba(192,28,20,0.6))} }

.home-title {
  font-family: 'Cinzel Decorative', serif;
  font-size: clamp(26px, 7vw, 54px);
  font-weight: 700;
  letter-spacing: 0.1em;
  color: var(--text);
  line-height: 1.1;
  text-shadow: 0 0 40px rgba(196,151,62,0.15);
}

.home-line {
  display: flex;
  align-items: center;
  gap: 16px;
  margin: 20px auto;
  width: fit-content;
}
.home-rule { width: 80px; height: 1px; background: linear-gradient(to right, transparent, var(--red)); }
.home-rule.r { background: linear-gradient(to left, transparent, var(--red)); }
.home-diamond { width: 5px; height: 5px; background: var(--red); transform: rotate(45deg); }

.home-sub {
  font-family: 'Courier Prime', monospace;
  font-size: 10px;
  letter-spacing: 0.45em;
  text-transform: uppercase;
  color: var(--text4);
  margin-bottom: 52px;
}

.home-enter {
  font-family: 'Courier Prime', monospace;
  font-size: 11px;
  letter-spacing: 0.35em;
  text-transform: uppercase;
  color: var(--red);
  background: transparent;
  border: 1px solid var(--red);
  padding: 14px 40px;
  cursor: pointer;
  transition: all 0.25s;
  position: relative;
  overflow: hidden;
}
.home-enter::before {
  content: '';
  position: absolute;
  inset: 0;
  background: var(--red);
  transform: scaleX(0);
  transform-origin: left;
  transition: transform 0.25s;
}
.home-enter:hover::before { transform: scaleX(1); }
.home-enter:hover { color: var(--ink); }
.home-enter span { position: relative; z-index: 1; }

.home-meta {
  font-family: 'Courier Prime', monospace;
  font-size: 9px;
  letter-spacing: 0.25em;
  color: var(--text5);
  margin-top: 28px;
  text-transform: uppercase;
}

/* ──────────────── QUERY ──────────────── */
.query { width: 100%; animation: fadeUp 0.5s ease both; }

.section-label {
  font-family: 'Courier Prime', monospace;
  font-size: 8px;
  letter-spacing: 0.45em;
  text-transform: uppercase;
  color: var(--text4);
  margin-bottom: 10px;
}

.masters-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 6px;
  margin-bottom: 8px;
}

.master-card {
  border: 1px solid var(--border);
  padding: 12px 14px;
  cursor: pointer;
  transition: all 0.2s;
  background: var(--card);
  position: relative;
  overflow: hidden;
}
.master-card::after {
  content: '';
  position: absolute;
  left: 0; top: 0; bottom: 0;
  width: 2px;
  background: var(--accent, var(--red));
  transform: scaleY(0);
  transition: transform 0.2s;
}
.master-card.active::after,
.master-card:hover::after { transform: scaleY(1); }
.master-card.active { border-color: var(--accent, var(--red)); background: #181410; }
.master-card:hover:not(.active) { border-color: var(--border2); }

.mc-sym {
  font-size: 20px;
  margin-bottom: 8px;
  color: var(--accent, var(--red));
  line-height: 1;
}
.mc-name {
  font-family: 'Cormorant Garamond', serif;
  font-size: 13px;
  font-weight: 600;
  color: var(--text);
  line-height: 1.2;
  margin-bottom: 3px;
}
.mc-role {
  font-family: 'Courier Prime', monospace;
  font-size: 8px;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  color: var(--accent, var(--red));
  margin-bottom: 4px;
}
.mc-sub {
  font-family: 'Courier Prime', monospace;
  font-size: 8px;
  letter-spacing: 0.1em;
  color: var(--text4);
}

.pressures {
  display: flex;
  gap: 6px;
  margin-bottom: 6px;
}
.pressure-btn {
  flex: 1;
  font-family: 'Courier Prime', monospace;
  font-size: 9px;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  border: 1px solid var(--border);
  color: var(--text4);
  background: var(--card);
  padding: 9px 4px;
  cursor: pointer;
  transition: all 0.2s;
}
.pressure-btn.active {
  border-color: var(--gold);
  color: var(--gold);
  background: #181510;
}
.pressure-btn:hover:not(.active) { border-color: var(--border2); color: var(--text3); }

.toggles { display: flex; gap: 6px; margin-bottom: 20px; }
.toggle-btn {
  font-family: 'Courier Prime', monospace;
  font-size: 9px;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  border: 1px solid var(--border);
  color: var(--text4);
  background: transparent;
  padding: 8px 14px;
  cursor: pointer;
  transition: all 0.2s;
  display: flex;
  align-items: center;
  gap: 6px;
}
.toggle-btn.on { border-color: var(--red); color: var(--red); }
.toggle-dot {
  width: 5px; height: 5px;
  border: 1px solid currentColor;
  border-radius: 50%;
  transition: background 0.2s;
}
.toggle-btn.on .toggle-dot { background: var(--red); }

.question-area {
  position: relative;
  margin-bottom: 14px;
}
.question-area textarea {
  width: 100%;
  background: var(--surface);
  border: 1px solid var(--border);
  border-top: 2px solid var(--red2);
  color: var(--text);
  font-family: 'Cormorant Garamond', serif;
  font-size: 19px;
  font-style: italic;
  font-weight: 300;
  padding: 18px 20px;
  resize: none;
  outline: none;
  min-height: 110px;
  transition: border-color 0.2s;
  line-height: 1.65;
  letter-spacing: 0.01em;
}
.question-area textarea:focus { border-color: var(--border2); }
.question-area textarea::placeholder { color: var(--text5); font-style: italic; }

.query-footer {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.footer-left { font-family: 'Courier Prime', monospace; font-size: 9px; letter-spacing: 0.2em; color: var(--text4); }
.footer-left.err { color: var(--red); }
.footer-btns { display: flex; gap: 8px; }

.btn {
  font-family: 'Courier Prime', monospace;
  font-size: 10px;
  letter-spacing: 0.25em;
  text-transform: uppercase;
  border: 1px solid var(--red);
  color: var(--red);
  background: transparent;
  padding: 11px 28px;
  cursor: pointer;
  transition: all 0.2s;
  position: relative;
  overflow: hidden;
}
.btn::before {
  content: '';
  position: absolute; inset: 0;
  background: var(--red);
  transform: scaleX(0);
  transform-origin: right;
  transition: transform 0.2s;
}
.btn:hover:not(:disabled)::before { transform: scaleX(1); }
.btn:hover:not(:disabled) { color: var(--ink); }
.btn:disabled { opacity: 0.3; cursor: not-allowed; }
.btn span { position: relative; z-index: 1; }

.btn-ghost {
  border-color: var(--border2);
  color: var(--text4);
}
.btn-ghost::before { background: var(--border2); }
.btn-ghost:hover:not(:disabled) { color: var(--text); }

/* ──────────────── LOADING ──────────────── */
.loading { text-align: center; animation: fadeUp 0.4s ease both; }
.load-sym {
  font-size: 52px;
  color: var(--red);
  animation: spin-pulse 3s ease-in-out infinite;
  display: block;
  margin-bottom: 28px;
  filter: drop-shadow(0 0 16px rgba(192,28,20,0.5));
}
@keyframes spin-pulse {
  0% { opacity: 0.3; transform: scale(0.9); }
  50% { opacity: 1; transform: scale(1.05); }
  100% { opacity: 0.3; transform: scale(0.9); }
}
.load-bars {
  display: flex;
  gap: 6px;
  justify-content: center;
  margin-bottom: 20px;
}
.load-bar {
  width: 2px;
  height: 24px;
  background: var(--red2);
  animation: bar-pulse 1.4s ease-in-out infinite;
}
.load-bar:nth-child(2) { animation-delay: 0.2s; }
.load-bar:nth-child(3) { animation-delay: 0.4s; }
.load-bar:nth-child(4) { animation-delay: 0.6s; }
.load-bar:nth-child(5) { animation-delay: 0.8s; }
@keyframes bar-pulse { 0%,100%{height:8px;opacity:0.2} 50%{height:28px;opacity:1} }
.load-text {
  font-family: 'Courier Prime', monospace;
  font-size: 9px;
  letter-spacing: 0.4em;
  text-transform: uppercase;
  color: var(--text4);
}

/* ──────────────── RESPONSE ──────────────── */
.resp { width: 100%; animation: fadeUp 0.5s ease both; }

.resp-question {
  font-family: 'Cormorant Garamond', serif;
  font-size: 14px;
  font-style: italic;
  color: var(--text4);
  text-align: center;
  margin-bottom: 36px;
  padding-bottom: 28px;
  border-bottom: 1px solid var(--border);
  line-height: 1.6;
}

.resp-master-header {
  text-align: center;
  margin-bottom: 28px;
}
.resp-master-sym {
  font-size: 28px;
  display: block;
  margin-bottom: 8px;
}
.resp-master-name {
  font-family: 'Cinzel Decorative', serif;
  font-size: clamp(11px, 2vw, 14px);
  letter-spacing: 0.12em;
  color: var(--text);
}
.resp-master-title {
  font-family: 'Courier Prime', monospace;
  font-size: 9px;
  letter-spacing: 0.3em;
  text-transform: uppercase;
  margin-top: 4px;
}

.resp-sections { margin-bottom: 40px; }

.rsec {
  margin-bottom: 32px;
  animation: fadeUp 0.5s ease both;
}
.rsec:nth-child(1) { animation-delay: 0.05s; }
.rsec:nth-child(2) { animation-delay: 0.15s; }
.rsec:nth-child(3) { animation-delay: 0.25s; }
.rsec:nth-child(4) { animation-delay: 0.35s; }
.rsec:nth-child(5) { animation-delay: 0.45s; }

.rsec-label {
  font-family: 'Courier Prime', monospace;
  font-size: 8px;
  letter-spacing: 0.5em;
  text-transform: uppercase;
  color: var(--gold);
  margin-bottom: 10px;
  opacity: 0.8;
}
.rsec-rule { width: 32px; height: 1px; background: var(--border2); margin-bottom: 12px; }

.strike {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(19px, 3.5vw, 24px);
  font-weight: 500;
  line-height: 1.5;
  color: var(--text);
  border-left: 2px solid var(--accent-r, var(--red));
  padding-left: 18px;
  letter-spacing: 0.01em;
}
.way {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(15px, 2.5vw, 17px);
  line-height: 1.8;
  color: var(--text2);
  font-weight: 300;
}
.image {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(14px, 2.5vw, 16px);
  font-style: italic;
  line-height: 1.8;
  color: var(--text3);
  font-weight: 300;
}
.form-list { list-style: none; }
.form-item {
  font-family: 'Courier Prime', monospace;
  font-size: 12px;
  color: var(--text2);
  margin-bottom: 10px;
  padding-left: 22px;
  position: relative;
  line-height: 1.6;
  letter-spacing: 0.02em;
}
.form-item::before {
  content: "—";
  position: absolute;
  left: 0;
  color: var(--accent-r, var(--red));
}
.void {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(16px, 3vw, 20px);
  font-style: italic;
  font-weight: 600;
  color: var(--gold);
  line-height: 1.6;
  letter-spacing: 0.01em;
}

/* TRIAD */
.triad-section {
  margin-bottom: 52px;
  padding-bottom: 48px;
  border-bottom: 1px solid var(--border);
  animation: fadeUp 0.5s ease both;
}
.triad-section:last-child { border-bottom: none; }
.triad-section:nth-child(1) { animation-delay: 0.05s; }
.triad-section:nth-child(2) { animation-delay: 0.2s; }
.triad-section:nth-child(3) { animation-delay: 0.35s; }

.resp-footer {
  display: flex;
  gap: 10px;
  padding-top: 32px;
  border-top: 1px solid var(--border);
}

@keyframes fadeUp {
  from { opacity: 0; transform: translateY(14px); }
  to { opacity: 1; transform: translateY(0); }
}
`;

const MASTERS = {
  musashi: {
    name: "Miyamoto Musashi",
    role: "The Strategist",
    sub: "Position · Timing · Execution",
    sym: "⚔",
    accent: "#C01C14",
    cssAccent: "var(--red)",
    persona: `You are Miyamoto Musashi — the greatest swordsman who ever lived. Voice: sharp, efficient, tactical, cold. You see through hesitation to the essential move. You believe strategy is revealed through movement, not deliberation. You are not cruel, but utterly uncompromising. Waste no words.`
  },
  tsunetomo: {
    name: "Yamamoto Tsunetomo",
    role: "The Resolute",
    sub: "Decisiveness · Death · Commitment",
    sym: "☽",
    accent: "#6A4E9A",
    cssAccent: "var(--purple)",
    persona: `You are Yamamoto Tsunetomo, author of the Hagakure. Voice: intense, unwavering, death-aware. You teach that the way of the samurai is found in death — to live already dead is to have no fear, no hesitation, only action. You demand totality. Half-measures are an insult to the path.`
  },
  shoju: {
    name: "Shoju Rojin",
    role: "The Clear",
    sub: "Awareness · Dissolution · Presence",
    sym: "◯",
    accent: "#3A7250",
    cssAccent: "var(--green)",
    persona: `You are Shoju Rojin, the old Zen master. Voice: calm, paradoxical, minimal. You dissolve the constructed self. Your words land like stones in still water — they do not push; they reveal. You are not concerned with solutions. You expose what was always already there, waiting beneath the noise of identity.`
  },
  balanced: {
    name: "The Council",
    role: "All Three Masters",
    sub: "Strategy · Resolve · Clarity",
    sym: "△",
    accent: "#C4973E",
    cssAccent: "var(--gold)",
    persona: `You are the unified voice of three masters: Miyamoto Musashi (strategy, action, positioning), Yamamoto Tsunetomo (decisiveness, death-awareness, total commitment), and Shoju Rojin (Zen clarity, ego dissolution, presence). Do not separate their voices — weave them into one singular truth. Each perspective deepens the others.`
  }
};

const PRESSURES = {
  still: { name: "Still Water", instruction: "Tone: calm and grounding. Clear without force. Speak as still water reflects the sky." },
  steel: { name: "Forged Steel", instruction: "Tone: firm and corrective. Direct but not cruel. Speak as steel holds its edge." },
  war: { name: "War Mode", instruction: "Tone: absolute brutal honesty. Zero comfort. Zero softening. No cushioning of any kind. Speak as if this is the last teaching before the end." }
};

const buildSysPrompt = (masterKey, pressure, history, creator) => {
  const m = MASTERS[masterKey];
  const p = PRESSURES[pressure];
  const histCtx = history.length
    ? `\n\nThe seeker has previously asked: ${history.slice(-3).map(h => `"${h}"`).join("; ")}. If you detect a pattern of avoidance, repetition, or circling — name it directly and without mercy.`
    : "";
  const cCtx = creator
    ? "\n\nApply your wisdom specifically and practically to the creative life: making art, finishing work, artistic discipline, creative identity, earning income from craft, the fear of putting work out."
    : "";

  return `${m.persona}

${p.instruction}${histCtx}${cCtx}

Return ONLY valid JSON with no markdown formatting, no backticks, no preamble — just the JSON object:
{"strike":"1-2 sentences. A single cutting truth. Direct. No cushion.","way":"3-5 sentences. Deep perspective from this master. Controlled — no rambling.","image":"2-4 sentences. A short story, analogy, or visual scene that sticks in the mind.","form":["Executable action step 1","Executable action step 2","Executable action step 3"],"void":"One question only. Must interrupt autopilot thinking. Make it land."}`;
};

const buildTriadSysPrompt = (pressure, history, creator) => {
  const p = PRESSURES[pressure];
  const histCtx = history.length
    ? `\nPrevious questions from this seeker: ${history.slice(-2).map(h => `"${h}"`).join(", ")}. Name patterns if present.`
    : "";
  const cCtx = creator ? "\nApply all wisdom to creative work and the artistic life." : "";

  return `You are three distinct Japanese masters of wisdom answering the same question from their own perspective:

MUSASHI (The Strategist): sharp, tactical, efficient — sees through hesitation to the essential move.
TSUNETOMO (The Resolute): intense, death-aware, demanding — live as if already dead, no hesitation.
SHOJU ROJIN (The Clear): calm, paradoxical, Zen — dissolves ego, reveals what was always there.

${p.instruction}${histCtx}${cCtx}

Return ONLY valid JSON with no markdown, no backticks:
{"musashi":{"strike":"...","way":"...","image":"...","form":["...","...","..."],"void":"..."},"tsunetomo":{"strike":"...","way":"...","image":"...","form":["...","...","..."],"void":"..."},"shoju":{"strike":"...","way":"...","image":"...","form":["...","...","..."],"void":"..."}}`;
};

const callAPI = async (system, question) => {
  const res = await fetch("https://api.anthropic.com/v1/messages", {
    method: "POST",
    headers: { "Content-Type": "application/json" },
    body: JSON.stringify({
      model: "claude-sonnet-4-20250514",
      max_tokens: 1000,
      system,
      messages: [{ role: "user", content: question }]
    })
  });
  const d = await res.json();
  const txt = d.content.map(b => b.text || "").join("").replace(/```json|```/g, "").trim();
  return JSON.parse(txt);
};

const ResponseBlock = ({ data, masterKey, animBase = 0 }) => {
  const m = MASTERS[masterKey];
  const accent = m?.accent || "#C4973E";

  return (
    <div>
      <div className="resp-master-header" style={{ color: accent }}>
        <span className="resp-master-sym">{m?.sym}</span>
        <div className="resp-master-name" style={{ color: "#E5D8C5" }}>{m?.name}</div>
        <div className="resp-master-title" style={{ color: accent }}>{m?.role}</div>
      </div>

      <div className="resp-sections">
        <div className="rsec" style={{ animationDelay: `${animBase + 0.05}s` }}>
          <div className="rsec-label">⬥ Strike</div>
          <div className="rsec-rule" />
          <div className="strike" style={{ "--accent-r": accent }}>{data.strike}</div>
        </div>

        <div className="rsec" style={{ animationDelay: `${animBase + 0.15}s` }}>
          <div className="rsec-label">⬥ Way</div>
          <div className="rsec-rule" />
          <div className="way">{data.way}</div>
        </div>

        <div className="rsec" style={{ animationDelay: `${animBase + 0.25}s` }}>
          <div className="rsec-label">⬥ Image</div>
          <div className="rsec-rule" />
          <div className="image">{data.image}</div>
        </div>

        <div className="rsec" style={{ animationDelay: `${animBase + 0.35}s` }}>
          <div className="rsec-label">⬥ Form</div>
          <div className="rsec-rule" />
          <ul className="form-list">
            {(data.form || []).map((step, i) => (
              <li key={i} className="form-item" style={{ "--accent-r": accent }}>{step}</li>
            ))}
          </ul>
        </div>

        <div className="rsec" style={{ animationDelay: `${animBase + 0.45}s` }}>
          <div className="rsec-label">⬥ Void</div>
          <div className="rsec-rule" />
          <div className="void">{data.void}</div>
        </div>
      </div>
    </div>
  );
};

const DAILY_LIMIT = 5;

export default function LivingBlade() {
  const [screen, setScreen] = useState("home");
  const [master, setMaster] = useState("balanced");
  const [pressure, setPressure] = useState("steel");
  const [triad, setTriad] = useState(false);
  const [creator, setCreator] = useState(false);
  const [question, setQuestion] = useState("");
  const [response, setResponse] = useState(null);
  const [history, setHistory] = useState([]);
  const [used, setUsed] = useState(0);
  const [err, setErr] = useState("");
  const [loading, setLoading] = useState(false);

  const remaining = DAILY_LIMIT - used;

  const ask = useCallback(async () => {
    if (!question.trim() || remaining <= 0) return;
    setLoading(true);
    setErr("");
    setScreen("loading");

    try {
      let resp;
      if (triad) {
        const data = await callAPI(buildTriadSysPrompt(pressure, history, creator), question);
        resp = { type: "triad", data, q: question };
      } else {
        const data = await callAPI(buildSysPrompt(master, pressure, history, creator), question);
        resp = { type: "single", master, data, q: question };
      }
      setHistory(h => [...h, question]);
      setUsed(u => u + 1);
      setResponse(resp);
      setScreen("response");
    } catch (e) {
      setErr("The masters are silent. " + (e.message || "Try again."));
      setScreen("query");
    } finally {
      setLoading(false);
    }
  }, [question, remaining, triad, master, pressure, history, creator]);

  return (
    <>
      <style>{STYLES}</style>
      <div className="grain" />
      <div className="wrap">

        {/* ── HOME ── */}
        {screen === "home" && (
          <div className="home">
            <div className="home-emblem">⚔</div>
            <div className="home-title">Living Blade</div>
            <div className="home-line">
              <div className="home-rule" />
              <div className="home-diamond" />
              <div className="home-rule r" />
            </div>
            <div className="home-sub">Wisdom Engine</div>
            <button className="home-enter" onClick={() => setScreen("query")}>
              <span>Enter</span>
            </button>
            <div className="home-meta">{remaining} of {DAILY_LIMIT} questions remain this session</div>
          </div>
        )}

        {/* ── QUERY ── */}
        {screen === "query" && (
          <div className="query">
            <div style={{ marginBottom: 28 }}>
              <div className="section-label" style={{ marginBottom: 10 }}>Choose Your Master</div>
              <div className="masters-grid">
                {Object.entries(MASTERS).map(([k, v]) => (
                  <div
                    key={k}
                    className={`master-card ${master === k ? "active" : ""}`}
                    style={{ "--accent": v.accent }}
                    onClick={() => setMaster(k)}
                  >
                    <div className="mc-sym">{v.sym}</div>
                    <div className="mc-name">{v.name}</div>
                    <div className="mc-role">{v.role}</div>
                    <div className="mc-sub">{v.sub}</div>
                  </div>
                ))}
              </div>
            </div>

            <div style={{ marginBottom: 20 }}>
              <div className="section-label" style={{ marginBottom: 8 }}>Intensity</div>
              <div className="pressures">
                {Object.entries(PRESSURES).map(([k, v]) => (
                  <button
                    key={k}
                    className={`pressure-btn ${pressure === k ? "active" : ""}`}
                    onClick={() => setPressure(k)}
                  >
                    {v.name}
                  </button>
                ))}
              </div>
            </div>

            <div style={{ marginBottom: 20 }}>
              <div className="section-label" style={{ marginBottom: 8 }}>Mode</div>
              <div className="toggles">
                <button className={`toggle-btn ${triad ? "on" : ""}`} onClick={() => setTriad(t => !t)}>
                  <span className="toggle-dot" /> Triad View
                </button>
                <button className={`toggle-btn ${creator ? "on" : ""}`} onClick={() => setCreator(c => !c)}>
                  <span className="toggle-dot" /> Creator Path
                </button>
              </div>
            </div>

            <div className="question-area">
              <textarea
                value={question}
                onChange={e => setQuestion(e.target.value)}
                onKeyDown={e => { if (e.key === "Enter" && (e.metaKey || e.ctrlKey)) ask(); }}
                placeholder="What is before you?"
                rows={5}
              />
            </div>

            <div className="query-footer">
              <div className={`footer-left ${err ? "err" : ""}`}>
                {err || `${remaining} question${remaining !== 1 ? "s" : ""} remain`}
              </div>
              <div className="footer-btns">
                <button className="btn btn-ghost" onClick={() => setScreen("home")}>
                  <span>↩</span>
                </button>
                <button
                  className="btn"
                  onClick={ask}
                  disabled={!question.trim() || remaining <= 0}
                >
                  <span>{remaining <= 0 ? "Return Tomorrow" : "Speak →"}</span>
                </button>
              </div>
            </div>
          </div>
        )}

        {/* ── LOADING ── */}
        {screen === "loading" && (
          <div className="loading">
            <span className="load-sym">⚔</span>
            <div className="load-bars">
              {[0,1,2,3,4].map(i => (
                <div key={i} className="load-bar" style={{ animationDelay: `${i * 0.2}s` }} />
              ))}
            </div>
            <div className="load-text">The masters speak</div>
          </div>
        )}

        {/* ── RESPONSE ── */}
        {screen === "response" && response && (
          <div className="resp">
            <div className="resp-question">"{response.q}"</div>

            {response.type === "single" && (
              <ResponseBlock data={response.data} masterKey={response.master} />
            )}

            {response.type === "triad" && (
              <>
                {["musashi", "tsunetomo", "shoju"].map((k, i) => (
                  <div key={k} className="triad-section">
                    <ResponseBlock data={response.data[k]} masterKey={k} animBase={i * 0.15} />
                  </div>
                ))}
              </>
            )}

            <div className="resp-footer">
              <button className="btn btn-ghost" onClick={() => setScreen("home")}>
                <span>↩ Home</span>
              </button>
              <button className="btn" onClick={() => { setQuestion(""); setScreen("query"); }}>
                <span>Ask Again →</span>
              </button>
            </div>
          </div>
        )}

      </div>
    </>
  );
}
