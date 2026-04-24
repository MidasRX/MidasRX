```aura width=900 height=300
<div style={{ position: 'relative', display: 'flex', width: '100%', height: '100%', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif', background: '#08080d' }}>
  <style>{`
    @keyframes orb-a { 0%, 100% { transform: translate(0, 0); opacity: 0.6; } 50% { transform: translate(28px, -22px); opacity: 0.95; } }
    @keyframes orb-b { 0%, 100% { transform: translate(0, 0); opacity: 0.5; } 50% { transform: translate(-22px, 18px); opacity: 0.8; } }
    @keyframes ring-blink { 0%, 100% { opacity: 0.06; } 50% { opacity: 0.22; } }
    @keyframes shine { 0% { transform: translateX(-200px); } 100% { transform: translateX(900px); } }
    #b-o1 { animation: orb-a 9s ease-in-out infinite; }
    #b-o2 { animation: orb-b 11s ease-in-out infinite 1s; }
    #b-o3 { animation: orb-a 8s ease-in-out infinite 2s; }
    #b-r1 { animation: ring-blink 7s ease-in-out infinite; }
    #b-r2 { animation: ring-blink 9s ease-in-out infinite 1.5s; }
    #b-shine { animation: shine 6s linear infinite; }
  `}</style>

  <img src="./img/banner.png" style={{ position: 'absolute', top: 0, left: 0, width: '100%', height: '100%', objectFit: 'cover', opacity: 0.45 }} />

  <svg width="900" height="300" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="bg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(108,195,255,0.55)" />
        <stop offset="100%" stopColor="rgba(108,195,255,0)" />
      </radialGradient>
      <radialGradient id="bg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(230,100,180,0.5)" />
        <stop offset="100%" stopColor="rgba(230,100,180,0)" />
      </radialGradient>
      <radialGradient id="bg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(195,155,255,0.4)" />
        <stop offset="100%" stopColor="rgba(195,155,255,0)" />
      </radialGradient>
      <linearGradient id="b-shine-grad" x1="0" x2="1" y1="0" y2="0">
        <stop offset="0%" stopColor="rgba(255,255,255,0)" />
        <stop offset="50%" stopColor="rgba(255,255,255,0.08)" />
        <stop offset="100%" stopColor="rgba(255,255,255,0)" />
      </linearGradient>
    </defs>
    <ellipse id="b-o1" cx="120" cy="260" rx="280" ry="200" fill="url(#bg1)" />
    <ellipse id="b-o2" cx="780" cy="60"  rx="240" ry="190" fill="url(#bg2)" />
    <ellipse id="b-o3" cx="700" cy="280" rx="220" ry="160" fill="url(#bg3)" />
    <circle id="b-r1" cx="450" cy="150" r="90"  fill="none" stroke="rgba(255,255,255,0.9)" strokeWidth="0.7" />
    <circle id="b-r2" cx="450" cy="150" r="160" fill="none" stroke="rgba(255,255,255,0.9)" strokeWidth="0.7" />
    <rect id="b-shine" x="0" y="0" width="180" height="300" fill="url(#b-shine-grad)" />
  </svg>

  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', zIndex: 10 }}>
    <span style={{ fontSize: 14, color: 'rgba(255,255,255,0.45)', letterSpacing: 6, textTransform: 'uppercase', fontWeight: 300 }}>welcome to my profile</span>
    <span style={{ fontSize: 64, fontWeight: 700, color: '#ffffff', letterSpacing: -2, lineHeight: 1, marginTop: 14 }}>Maxime Police</span>
    <span style={{ fontSize: 14, color: 'rgba(255,255,255,0.55)', marginTop: 14, letterSpacing: 3, textTransform: 'uppercase', fontWeight: 300 }}>systems · low-level · windows</span>
    <div style={{ display: 'flex', gap: 8, marginTop: 22 }}>
      <span style={{ padding: '6px 16px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.7)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(255,255,255,0.1)', letterSpacing: 1 }}>C++</span>
      <span style={{ padding: '6px 16px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.7)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(255,255,255,0.1)', letterSpacing: 1 }}>Rust</span>
      <span style={{ padding: '6px 16px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.7)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(255,255,255,0.1)', letterSpacing: 1 }}>C#</span>
      <span style={{ padding: '6px 16px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.7)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(255,255,255,0.1)', letterSpacing: 1 }}>Windows Internals</span>
    </div>
  </div>
</div>
```

```aura width=900 height=240
<div style={{ display: 'flex', flexDirection: 'row', gap: 16, width: '100%', height: '100%', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes a-orb-l { 0%, 100% { transform: translate(0,0); opacity: 0.65; } 50% { transform: translate(20px,-14px); opacity: 0.9; } }
    @keyframes a-orb-r { 0%, 100% { transform: translate(0,0); opacity: 0.55; } 50% { transform: translate(-16px,12px); opacity: 0.85; } }
    @keyframes a-ring { 0%, 100% { opacity: 0.07; } 50% { opacity: 0.22; } }
    @keyframes cursor-blink { 0%, 49% { opacity: 1; } 50%, 99% { opacity: 0; } 100% { opacity: 1; } }
    #ab-o1 { animation: a-orb-l 8s ease-in-out infinite; }
    #ab-o2 { animation: a-orb-r 10s ease-in-out infinite 1s; }
    #ab-o3 { animation: a-orb-l 7s ease-in-out infinite 2s; }
    #ab-r1 { animation: a-ring 7s ease-in-out infinite; }
    #ab-r2 { animation: a-ring 7s ease-in-out infinite 2s; }
    #ab-cursor { animation: cursor-blink 1.1s step-end infinite; }
  `}</style>

  <div style={{ position: 'relative', display: 'flex', flex: 1, height: '100%', background: '#08080d', borderRadius: 16, overflow: 'hidden' }}>
    <svg width="100%" height="240" style={{ position: 'absolute', top: 0, left: 0 }}>
      <defs>
        <radialGradient id="abg1" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(108,195,255,0.55)" />
          <stop offset="100%" stopColor="rgba(108,195,255,0)" />
        </radialGradient>
        <radialGradient id="abg2" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(230,100,180,0.45)" />
          <stop offset="100%" stopColor="rgba(230,100,180,0)" />
        </radialGradient>
        <radialGradient id="abg3" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(195,155,255,0.35)" />
          <stop offset="100%" stopColor="rgba(195,155,255,0)" />
        </radialGradient>
      </defs>
      <ellipse id="ab-o1" cx="60"  cy="200" rx="160" ry="130" fill="url(#abg1)" />
      <ellipse id="ab-o2" cx="380" cy="40"  rx="140" ry="110" fill="url(#abg2)" />
      <ellipse id="ab-o3" cx="320" cy="220" rx="120" ry="100" fill="url(#abg3)" />
      <circle id="ab-r1" cx="200" cy="120" r="48"  fill="none" stroke="rgba(255,255,255,0.9)" strokeWidth="0.7" />
      <circle id="ab-r2" cx="200" cy="120" r="80"  fill="none" stroke="rgba(255,255,255,0.9)" strokeWidth="0.7" />
    </svg>
    <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'center', padding: '0 32px', zIndex: 10 }}>
      <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.4)', letterSpacing: 4, textTransform: 'uppercase', marginBottom: 12 }}>about</span>
      <span style={{ fontSize: 24, fontWeight: 600, color: '#ffffff', lineHeight: 1.3 }}>Low-level developer.</span>
      <span style={{ fontSize: 24, fontWeight: 600, color: '#ffffff', lineHeight: 1.3 }}>Windows whisperer.</span>
      <div style={{ display: 'flex', alignItems: 'center', marginTop: 16 }}>
        <span style={{ fontSize: 13, color: 'rgba(255,255,255,0.5)', fontFamily: 'monospace' }}>{'> currently shipping at Zerdium'}</span>
        <span id="ab-cursor" style={{ fontSize: 13, color: 'rgba(255,255,255,0.7)', fontFamily: 'monospace', marginLeft: 1 }}>_</span>
      </div>
    </div>
  </div>

  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: 260, flexShrink: 0, background: '#08080d', borderRadius: 16, overflow: 'hidden' }}>
    <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.35)', letterSpacing: 4, textTransform: 'uppercase' }}>currently at</span>
    <img src="./img/zerdium logo.png" style={{ width: 160, height: 80, objectFit: 'contain', marginTop: 12 }} />
    <span style={{ fontSize: 18, fontWeight: 700, color: '#ffffff', marginTop: 10 }}>Zerdium</span>
    <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.4)', marginTop: 4, letterSpacing: 1 }}>previously · Nova Sentinel</span>
  </div>
</div>
```

```aura width=900 height=220
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#08080d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes s-orb { 0%, 100% { transform: translate(0,0); opacity: 0.45; } 50% { transform: translate(18px,-14px); opacity: 0.7; } }
    @keyframes s-orb-b { 0%, 100% { transform: translate(0,0); opacity: 0.4; } 50% { transform: translate(-14px,10px); opacity: 0.65; } }
    #st-o1 { animation: s-orb 10s ease-in-out infinite; }
    #st-o2 { animation: s-orb-b 12s ease-in-out infinite 1s; }
    #st-o3 { animation: s-orb 9s ease-in-out infinite 2.5s; }
    #st-o4 { animation: s-orb-b 11s ease-in-out infinite 0.5s; }
  `}</style>
  <svg width="900" height="220" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="stg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(108,195,255,0.4)" />
        <stop offset="100%" stopColor="rgba(108,195,255,0)" />
      </radialGradient>
      <radialGradient id="stg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(230,100,180,0.35)" />
        <stop offset="100%" stopColor="rgba(230,100,180,0)" />
      </radialGradient>
      <radialGradient id="stg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(80,160,220,0.3)" />
        <stop offset="100%" stopColor="rgba(80,160,220,0)" />
      </radialGradient>
      <radialGradient id="stg4" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(195,155,255,0.3)" />
        <stop offset="100%" stopColor="rgba(195,155,255,0)" />
      </radialGradient>
    </defs>
    <ellipse id="st-o1" cx="80"  cy="180" rx="180" ry="140" fill="url(#stg1)" />
    <ellipse id="st-o2" cx="820" cy="50"  rx="170" ry="130" fill="url(#stg2)" />
    <ellipse id="st-o3" cx="720" cy="190" rx="160" ry="120" fill="url(#stg3)" />
    <ellipse id="st-o4" cx="180" cy="40"  rx="150" ry="110" fill="url(#stg4)" />
  </svg>
  <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.35)', letterSpacing: 5, textTransform: 'uppercase', marginBottom: 18, zIndex: 10 }}>my stack</span>
  <div style={{ display: 'flex', flexWrap: 'wrap', gap: 10, justifyContent: 'center', zIndex: 10, maxWidth: 780 }}>
    {['C++', 'Rust', 'C#', 'C', 'Python', 'HTML', 'CSS', 'Windows Mastering'].map((tech, i) => (
      <span key={i} style={{ padding: '8px 20px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.75)', borderRadius: 100, fontSize: 13, border: '1px solid rgba(255,255,255,0.1)', letterSpacing: 0.5 }}>{tech}</span>
    ))}
  </div>
</div>
```

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=MidasRX&show_icons=true&theme=tokyonight&hide_border=true&bg_color=08080d&title_color=6cc3ff&icon_color=e664b4&text_color=ffffff" alt="GitHub Stats" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=MidasRX&layout=compact&theme=tokyonight&hide_border=true&bg_color=08080d&title_color=6cc3ff&text_color=ffffff&langs_count=8" alt="Top Languages" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=MidasRX&theme=tokyonight&hide_border=true&background=08080d&ring=6cc3ff&fire=e664b4&currStreakLabel=ffffff" alt="GitHub Streak" />
</p>

```aura width=900 height=180
<div style={{ position: 'relative', display: 'flex', width: '100%', height: '100%', background: '#08080d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes joke-orb { 0%, 100% { transform: translate(0,0); opacity: 0.5; } 50% { transform: translate(20px,-12px); opacity: 0.8; } }
    @keyframes chick-bob { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-6px); } }
    @keyframes pop { 0% { opacity: 0; transform: scale(0.9); } 100% { opacity: 1; transform: scale(1); } }
    #j-o1 { animation: joke-orb 9s ease-in-out infinite; }
    #j-o2 { animation: joke-orb 11s ease-in-out infinite 1.5s; }
    #chick { animation: chick-bob 1.6s ease-in-out infinite; transform-origin: center; }
    #punch { animation: pop 1s ease-out 1.2s both; }
  `}</style>
  <svg width="900" height="180" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="jg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(255,195,110,0.4)" />
        <stop offset="100%" stopColor="rgba(255,195,110,0)" />
      </radialGradient>
      <radialGradient id="jg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(108,195,255,0.35)" />
        <stop offset="100%" stopColor="rgba(108,195,255,0)" />
      </radialGradient>
    </defs>
    <ellipse id="j-o1" cx="120" cy="160" rx="180" ry="130" fill="url(#jg1)" />
    <ellipse id="j-o2" cx="780" cy="30"  rx="170" ry="130" fill="url(#jg2)" />
  </svg>
  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'center', padding: '0 40px', zIndex: 10, width: '100%' }}>
    <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.4)', letterSpacing: 5, textTransform: 'uppercase', marginBottom: 8 }}>daily joke</span>
    <div style={{ display: 'flex', alignItems: 'center', gap: 14 }}>
      <span id="chick" style={{ fontSize: 44 }}>🐔</span>
      <div style={{ display: 'flex', flexDirection: 'column' }}>
        <span style={{ fontSize: 20, fontWeight: 600, color: '#ffffff', lineHeight: 1.3 }}>Why did the chicken cross the road?</span>
        <span id="punch" style={{ fontSize: 16, color: 'rgba(255,255,255,0.7)', marginTop: 6, fontStyle: 'italic' }}>To get to the other `;`</span>
      </div>
    </div>
  </div>
</div>
```

## 📬 Get In Touch

<p align="center">
  <a href="https://t.me/NagiOnTop">
    <img src="./img/telegram-logo-0-2.webp" alt="Telegram" width="64" height="64" />
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://discord.com/users/maximepolice">
    <img src="./img/canva-discord-logo-MAGzZ0yqbBM.webp" alt="Discord" width="64" height="64" />
  </a>
</p>

<p align="center">
  <b>Telegram</b> · <code>@NagiOnTop</code> &nbsp;·&nbsp; <b>Discord</b> · <code>maximepolice</code>
</p>

```aura width=160 height=44 link="https://t.me/NagiOnTop" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/telegram/26A5E4"
  text="@NagiOnTop"
  backgroundColor="#0a2939"
  width={160}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#eeeeee' },
    { offset: '60%', color: '#26A5E4' },
    { offset: '80%', color: '#111111' },
    { offset: '100%', color: '#555555' },
  ]}
/>
```

```aura width=170 height=44 link="https://discord.com/users/maximepolice" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/discord/5865F2"
  text="maximepolice"
  backgroundColor="#1a1b3a"
  width={170}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#eeeeee' },
    { offset: '60%', color: '#5865F2' },
    { offset: '80%', color: '#111111' },
    { offset: '100%', color: '#555555' },
  ]}
/>
```

```aura width=140 height=44 link="https://github.com/MidasRX" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/github/ffffff"
  text="GitHub"
  backgroundColor="#141414"
  width={140}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#eeeeee' },
    { offset: '60%', color: '#ffffff' },
    { offset: '80%', color: '#111111' },
    { offset: '100%', color: '#555555' },
  ]}
/>
```

<p align="center">
  <sub>Crafted with <a href="https://github.com/collectioneur/readme-aura">readme-aura</a> · React/JSX → SVG</sub>
</p>
