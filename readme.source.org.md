```aura width=900 height=310
<div style={{ position: 'relative', display: 'flex', width: '100%', height: '100%', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif', background: '#07070c' }}>
  <style>{`
    @keyframes corp-orb-a { 0%, 100% { transform: translate(0, 0); opacity: 0.55; } 50% { transform: translate(30px, -20px); opacity: 0.85; } }
    @keyframes corp-orb-b { 0%, 100% { transform: translate(0, 0); opacity: 0.45; } 50% { transform: translate(-24px, 16px); opacity: 0.72; } }
    @keyframes corp-ring { 0%, 100% { opacity: 0.05; } 50% { opacity: 0.16; } }
    @keyframes corp-ring-b { 0%, 100% { opacity: 0.03; } 50% { opacity: 0.10; } }
    @keyframes corp-shine { 0% { transform: translateX(-220px); } 100% { transform: translateX(920px); } }
    #co1 { animation: corp-orb-a 10s ease-in-out infinite; }
    #co2 { animation: corp-orb-b 13s ease-in-out infinite 1.2s; }
    #co3 { animation: corp-orb-a 9s ease-in-out infinite 2.5s; }
    #co4 { animation: corp-orb-b 11s ease-in-out infinite 0.6s; }
    #cr1 { animation: corp-ring 9s ease-in-out infinite; }
    #cr2 { animation: corp-ring 11s ease-in-out infinite 2.2s; }
    #cr3 { animation: corp-ring-b 13s ease-in-out infinite 4s; }
    #cshine { animation: corp-shine 8s linear infinite; }
  `}</style>
  <svg width="900" height="310" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="cg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(212,175,55,0.52)" />
        <stop offset="100%" stopColor="rgba(212,175,55,0)" />
      </radialGradient>
      <radialGradient id="cg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(184,134,11,0.44)" />
        <stop offset="100%" stopColor="rgba(184,134,11,0)" />
      </radialGradient>
      <radialGradient id="cg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(245,220,140,0.28)" />
        <stop offset="100%" stopColor="rgba(245,220,140,0)" />
      </radialGradient>
      <radialGradient id="cg4" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(212,175,55,0.22)" />
        <stop offset="100%" stopColor="rgba(212,175,55,0)" />
      </radialGradient>
      <linearGradient id="cshine-g" x1="0" x2="1" y1="0" y2="0">
        <stop offset="0%" stopColor="rgba(212,175,55,0)" />
        <stop offset="50%" stopColor="rgba(212,175,55,0.055)" />
        <stop offset="100%" stopColor="rgba(212,175,55,0)" />
      </linearGradient>
    </defs>
    <ellipse id="co1" cx="90"  cy="270" rx="290" ry="210" fill="url(#cg1)" />
    <ellipse id="co2" cx="820" cy="55"  rx="260" ry="200" fill="url(#cg2)" />
    <ellipse id="co3" cx="720" cy="285" rx="230" ry="170" fill="url(#cg3)" />
    <ellipse id="co4" cx="210" cy="45"  rx="210" ry="160" fill="url(#cg4)" />
    <circle id="cr1" cx="450" cy="155" r="90"  fill="none" stroke="rgba(212,175,55,0.9)" strokeWidth="0.6" />
    <circle id="cr2" cx="450" cy="155" r="155" fill="none" stroke="rgba(212,175,55,0.9)" strokeWidth="0.5" />
    <circle id="cr3" cx="450" cy="155" r="220" fill="none" stroke="rgba(212,175,55,0.9)" strokeWidth="0.4" />
    <rect id="cshine" x="0" y="0" width="200" height="310" fill="url(#cshine-g)" />
  </svg>
  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', zIndex: 10 }}>
    <img src="./img/zerdium logo.png" width={86} height={86} style={{ objectFit: 'contain', marginBottom: 14 }} />
    <span style={{ fontSize: 10, color: 'rgba(212,175,55,0.55)', letterSpacing: 7, textTransform: 'uppercase', fontWeight: 300 }}>official organization</span>
    <span style={{ fontSize: 64, fontWeight: 800, color: '#ffffff', letterSpacing: -2, lineHeight: 1, marginTop: 10 }}>ZERDIUM</span>
    <span style={{ fontSize: 12, color: 'rgba(212,175,55,0.85)', letterSpacing: 9, textTransform: 'uppercase', fontWeight: 300, marginTop: 10 }}>Corporation</span>
    <div style={{ display: 'flex', gap: 10, marginTop: 24 }}>
      <span style={{ padding: '5px 15px', background: 'rgba(212,175,55,0.07)', color: 'rgba(212,175,55,0.85)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(212,175,55,0.22)', letterSpacing: 0.8 }}>🇫🇷 Owner · France</span>
      <span style={{ padding: '5px 15px', background: 'rgba(212,175,55,0.07)', color: 'rgba(212,175,55,0.85)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(212,175,55,0.22)', letterSpacing: 0.8 }}>🇷🇺 Registered · Russia</span>
      <span style={{ padding: '5px 15px', background: 'rgba(212,175,55,0.07)', color: 'rgba(212,175,55,0.85)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(212,175,55,0.22)', letterSpacing: 0.8 }}>🔒 Proprietary</span>
      <span style={{ padding: '5px 15px', background: 'rgba(212,175,55,0.07)', color: 'rgba(212,175,55,0.85)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(212,175,55,0.22)', letterSpacing: 0.8 }}>💼 Private Funding</span>
    </div>
  </div>
</div>
```

```aura width=900 height=230
<div style={{ display: 'flex', flexDirection: 'row', gap: 16, width: '100%', height: '100%', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes ab2-orb-l { 0%, 100% { transform: translate(0,0); opacity: 0.6; } 50% { transform: translate(22px,-16px); opacity: 0.88; } }
    @keyframes ab2-orb-r { 0%, 100% { transform: translate(0,0); opacity: 0.5; } 50% { transform: translate(-18px,14px); opacity: 0.75; } }
    @keyframes ab2-ring { 0%, 100% { opacity: 0.06; } 50% { opacity: 0.18; } }
    @keyframes ab2-cursor { 0%, 49% { opacity: 1; } 50%, 99% { opacity: 0; } 100% { opacity: 1; } }
    #ab2-o1 { animation: ab2-orb-l 9s ease-in-out infinite; }
    #ab2-o2 { animation: ab2-orb-r 11s ease-in-out infinite 1.1s; }
    #ab2-o3 { animation: ab2-orb-l 8s ease-in-out infinite 2.3s; }
    #ab2-r1 { animation: ab2-ring 8s ease-in-out infinite; }
    #ab2-r2 { animation: ab2-ring 8s ease-in-out infinite 2.4s; }
    #ab2-cur { animation: ab2-cursor 1.1s step-end infinite; }
  `}</style>

  <div style={{ position: 'relative', display: 'flex', flex: 1, height: '100%', background: '#07070c', borderRadius: 16, overflow: 'hidden' }}>
    <svg width="100%" height="230" style={{ position: 'absolute', top: 0, left: 0 }}>
      <defs>
        <radialGradient id="ab2g1" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(212,175,55,0.48)" />
          <stop offset="100%" stopColor="rgba(212,175,55,0)" />
        </radialGradient>
        <radialGradient id="ab2g2" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(184,134,11,0.38)" />
          <stop offset="100%" stopColor="rgba(184,134,11,0)" />
        </radialGradient>
        <radialGradient id="ab2g3" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(245,220,140,0.28)" />
          <stop offset="100%" stopColor="rgba(245,220,140,0)" />
        </radialGradient>
      </defs>
      <ellipse id="ab2-o1" cx="50"  cy="195" rx="170" ry="140" fill="url(#ab2g1)" />
      <ellipse id="ab2-o2" cx="410" cy="38"  rx="150" ry="120" fill="url(#ab2g2)" />
      <ellipse id="ab2-o3" cx="340" cy="215" rx="130" ry="105" fill="url(#ab2g3)" />
      <circle id="ab2-r1" cx="210" cy="115" r="50"  fill="none" stroke="rgba(212,175,55,0.9)" strokeWidth="0.6" />
      <circle id="ab2-r2" cx="210" cy="115" r="85"  fill="none" stroke="rgba(212,175,55,0.9)" strokeWidth="0.5" />
    </svg>
    <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'center', padding: '0 36px', zIndex: 10 }}>
      <span style={{ fontSize: 10, color: 'rgba(212,175,55,0.5)', letterSpacing: 4, textTransform: 'uppercase', marginBottom: 14 }}>about</span>
      <span style={{ fontSize: 22, fontWeight: 700, color: '#ffffff', lineHeight: 1.35 }}>Private software corporation.</span>
      <span style={{ fontSize: 22, fontWeight: 700, color: '#ffffff', lineHeight: 1.35 }}>Proprietary by design.</span>
      <span style={{ fontSize: 13, color: 'rgba(255,255,255,0.45)', marginTop: 14, lineHeight: 1.6, maxWidth: 380 }}>ZerdiumCorp builds internal tooling, systems software, and proprietary infrastructure. All research, source code, and products remain exclusively owned by the corporation.</span>
      <div style={{ display: 'flex', alignItems: 'center', marginTop: 16 }}>
        <span style={{ fontSize: 12, color: 'rgba(212,175,55,0.55)', fontFamily: 'monospace' }}>{'> closed · internal · not open for investment'}</span>
        <span id="ab2-cur" style={{ fontSize: 12, color: 'rgba(212,175,55,0.7)', fontFamily: 'monospace', marginLeft: 1 }}>_</span>
      </div>
    </div>
  </div>

  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'center', gap: 0, width: 262, flexShrink: 0, background: '#07070c', borderRadius: 16, overflow: 'hidden', padding: '0 22px' }}>
    <svg width="262" height="230" style={{ position: 'absolute', top: 0, left: 0 }}>
      <defs>
        <radialGradient id="fact-g" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(212,175,55,0.18)" />
          <stop offset="100%" stopColor="rgba(212,175,55,0)" />
        </radialGradient>
      </defs>
      <ellipse cx="131" cy="115" rx="140" ry="120" fill="url(#fact-g)" />
    </svg>
    <span style={{ fontSize: 10, color: 'rgba(212,175,55,0.5)', letterSpacing: 4, textTransform: 'uppercase', marginBottom: 16, zIndex: 10 }}>corporate profile</span>
    {[
      { label: 'Jurisdiction', value: 'Russian Federation' },
      { label: 'Leadership', value: 'France (owner)' },
      { label: 'Funding', value: 'Private income only' },
      { label: 'Investment', value: 'Not available' },
      { label: 'License', value: 'All rights reserved' },
    ].map((item, i) => (
      <div key={i} style={{ display: 'flex', flexDirection: 'column', marginBottom: 13, zIndex: 10 }}>
        <span style={{ fontSize: 10, color: 'rgba(212,175,55,0.45)', letterSpacing: 2, textTransform: 'uppercase' }}>{item.label}</span>
        <span style={{ fontSize: 13, color: 'rgba(255,255,255,0.82)', fontWeight: 500, marginTop: 2 }}>{item.value}</span>
      </div>
    ))}
  </div>
</div>
```

```aura width=900 height=200
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#07070c', borderRadius: 16, overflow: 'hidden', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes svc-orb-a { 0%, 100% { transform: translate(0,0); opacity: 0.45; } 50% { transform: translate(22px,-16px); opacity: 0.72; } }
    @keyframes svc-orb-b { 0%, 100% { transform: translate(0,0); opacity: 0.38; } 50% { transform: translate(-18px,12px); opacity: 0.6; } }
    @keyframes svc-chip { 0% { opacity: 0; transform: translateY(10px); } 100% { opacity: 1; transform: translateY(0); } }
    #sv1 { animation: svc-orb-a 11s ease-in-out infinite; }
    #sv2 { animation: svc-orb-b 13s ease-in-out infinite 1.5s; }
    #sv3 { animation: svc-orb-a 10s ease-in-out infinite 3s; }
    #sv4 { animation: svc-orb-b 12s ease-in-out infinite 0.8s; }
  `}</style>
  <svg width="900" height="200" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="svg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(212,175,55,0.38)" />
        <stop offset="100%" stopColor="rgba(212,175,55,0)" />
      </radialGradient>
      <radialGradient id="svg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(184,134,11,0.3)" />
        <stop offset="100%" stopColor="rgba(184,134,11,0)" />
      </radialGradient>
      <radialGradient id="svg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(245,220,140,0.2)" />
        <stop offset="100%" stopColor="rgba(245,220,140,0)" />
      </radialGradient>
      <radialGradient id="svg4" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(212,175,55,0.16)" />
        <stop offset="100%" stopColor="rgba(212,175,55,0)" />
      </radialGradient>
    </defs>
    <ellipse id="sv1" cx="80"  cy="170" rx="190" ry="130" fill="url(#svg1)" />
    <ellipse id="sv2" cx="830" cy="40"  rx="175" ry="130" fill="url(#svg2)" />
    <ellipse id="sv3" cx="700" cy="175" rx="160" ry="120" fill="url(#svg3)" />
    <ellipse id="sv4" cx="200" cy="35"  rx="160" ry="115" fill="url(#svg4)" />
  </svg>
  <span style={{ fontSize: 10, color: 'rgba(212,175,55,0.5)', letterSpacing: 4, textTransform: 'uppercase', marginBottom: 24, zIndex: 10 }}>services</span>
  <div style={{ display: 'flex', gap: 16, zIndex: 10 }}>
    {[
      { icon: '🎯', label: 'Cheat', desc: 'Game cheats & exploits', color: 'rgba(212,175,55,0.85)' },
      { icon: '🖥', label: 'Remote Access Tools', desc: 'Private · Internal use only', color: 'rgba(108,195,255,0.85)' },
      { icon: '🌐', label: 'Website', desc: 'Web development & hosting', color: 'rgba(163,230,53,0.85)' },
      { icon: '🎮', label: 'Game', desc: 'Game development', color: 'rgba(195,155,255,0.85)' },
    ].map((svc, i) => (
      <div key={i} style={{ display: 'flex', flexDirection: 'column', alignItems: 'center', gap: 8, padding: '18px 28px', background: 'rgba(255,255,255,0.025)', border: '1px solid rgba(212,175,55,0.12)', borderRadius: 14, minWidth: 170 }}>
        <span style={{ fontSize: 28 }}>{svc.icon}</span>
        <span style={{ fontSize: 13, fontWeight: 700, color: svc.color, textAlign: 'center' }}>{svc.label}</span>
        <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.35)', textAlign: 'center', letterSpacing: 0.5 }}>{svc.desc}</span>
      </div>
    ))}
  </div>
</div>
```

```aura width=900 height=290
<div style={{ display: 'flex', flexDirection: 'row', gap: 16, width: '100%', height: '100%', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes team-orb-a { 0%, 100% { transform: translate(0,0); opacity: 0.5; } 50% { transform: translate(20px,-14px); opacity: 0.78; } }
    @keyframes team-orb-b { 0%, 100% { transform: translate(0,0); opacity: 0.42; } 50% { transform: translate(-16px,12px); opacity: 0.65; } }
    @keyframes team-ring { 0%, 100% { opacity: 0.05; } 50% { opacity: 0.16; } }
    #to1 { animation: team-orb-a 10s ease-in-out infinite; }
    #to2 { animation: team-orb-b 12s ease-in-out infinite 1.3s; }
    #to3 { animation: team-orb-a 9s ease-in-out infinite 2.6s; }
    #tr1 { animation: team-ring 9s ease-in-out infinite; }
    #tr2 { animation: team-ring 9s ease-in-out infinite 3s; }
  `}</style>

  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'center', flex: 1, height: '100%', background: '#07070c', borderRadius: 16, overflow: 'hidden', padding: '0 32px' }}>
    <svg width="100%" height="290" style={{ position: 'absolute', top: 0, left: 0 }}>
      <defs>
        <radialGradient id="tg1" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(212,175,55,0.45)" />
          <stop offset="100%" stopColor="rgba(212,175,55,0)" />
        </radialGradient>
        <radialGradient id="tg2" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(184,134,11,0.35)" />
          <stop offset="100%" stopColor="rgba(184,134,11,0)" />
        </radialGradient>
        <radialGradient id="tg3" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(245,220,140,0.22)" />
          <stop offset="100%" stopColor="rgba(245,220,140,0)" />
        </radialGradient>
      </defs>
      <ellipse id="to1" cx="50"  cy="250" rx="180" ry="150" fill="url(#tg1)" />
      <ellipse id="to2" cx="480" cy="38"  rx="160" ry="130" fill="url(#tg2)" />
      <ellipse id="to3" cx="390" cy="260" rx="140" ry="110" fill="url(#tg3)" />
      <circle id="tr1" cx="230" cy="145" r="55"  fill="none" stroke="rgba(212,175,55,0.9)" strokeWidth="0.55" />
      <circle id="tr2" cx="230" cy="145" r="92"  fill="none" stroke="rgba(212,175,55,0.9)" strokeWidth="0.45" />
    </svg>
    <div style={{ position: 'relative', zIndex: 10 }}>
      <span style={{ fontSize: 10, color: 'rgba(212,175,55,0.5)', letterSpacing: 4, textTransform: 'uppercase' }}>ownership history</span>
      <div style={{ display: 'flex', flexDirection: 'column', gap: 14, marginTop: 18 }}>
        <div style={{ display: 'flex', alignItems: 'center', gap: 14 }}>
          <div style={{ width: 36, height: 36, borderRadius: '50%', background: 'rgba(212,175,55,0.12)', border: '1px solid rgba(212,175,55,0.4)', display: 'flex', alignItems: 'center', justifyContent: 'center', fontSize: 14, flexShrink: 0 }}>👑</div>
          <div style={{ display: 'flex', flexDirection: 'column' }}>
            <span style={{ fontSize: 15, fontWeight: 700, color: '#ffffff' }}>MidasR (Nagi)</span>
            <span style={{ fontSize: 11, color: 'rgba(212,175,55,0.75)', letterSpacing: 1 }}>Current Owner · github.com/MidasRX</span>
          </div>
          <span style={{ marginLeft: 'auto', padding: '3px 10px', background: 'rgba(212,175,55,0.1)', color: 'rgba(212,175,55,0.9)', borderRadius: 100, fontSize: 10, border: '1px solid rgba(212,175,55,0.25)', letterSpacing: 1 }}>ACTIVE</span>
        </div>
        <div style={{ height: '1px', background: 'rgba(212,175,55,0.08)' }} />
        <div style={{ display: 'flex', alignItems: 'center', gap: 14 }}>
          <div style={{ width: 36, height: 36, borderRadius: '50%', background: 'rgba(255,255,255,0.04)', border: '1px solid rgba(255,255,255,0.12)', display: 'flex', alignItems: 'center', justifyContent: 'center', fontSize: 14, flexShrink: 0 }}>🏛</div>
          <div style={{ display: 'flex', flexDirection: 'column' }}>
            <span style={{ fontSize: 15, fontWeight: 600, color: 'rgba(255,255,255,0.6)' }}>Totowi</span>
            <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.3)', letterSpacing: 1 }}>Former Owner</span>
          </div>
          <span style={{ marginLeft: 'auto', padding: '3px 10px', background: 'rgba(255,255,255,0.04)', color: 'rgba(255,255,255,0.3)', borderRadius: 100, fontSize: 10, border: '1px solid rgba(255,255,255,0.08)', letterSpacing: 1 }}>FORMER</span>
        </div>
      </div>
    </div>
  </div>

  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'center', width: 420, flexShrink: 0, background: '#07070c', borderRadius: 16, overflow: 'hidden', padding: '0 28px' }}>
    <svg width="420" height="290" style={{ position: 'absolute', top: 0, left: 0 }}>
      <defs>
        <radialGradient id="devg" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(212,175,55,0.14)" />
          <stop offset="100%" stopColor="rgba(212,175,55,0)" />
        </radialGradient>
      </defs>
      <ellipse cx="210" cy="145" rx="230" ry="160" fill="url(#devg)" />
    </svg>
    <span style={{ fontSize: 10, color: 'rgba(212,175,55,0.5)', letterSpacing: 4, textTransform: 'uppercase', marginBottom: 18, zIndex: 10 }}>developers</span>
    <div style={{ display: 'flex', flexDirection: 'column', gap: 12, zIndex: 10 }}>
      {[
        { name: 'dilka', role: 'Junior C# Developer · Junior C++/C Developer', status: 'active', color: '#6cc3ff' },
        { name: 'phoenix', role: 'C/C++ Developer', status: 'active', color: '#a3e635' },
        { name: 'Midnight', role: 'C/C++ Developer', status: 'retired', color: 'rgba(255,255,255,0.3)' },
      ].map((dev, i) => (
        <div key={i} style={{ display: 'flex', alignItems: 'center', gap: 12 }}>
          <div style={{ width: 8, height: 8, borderRadius: '50%', background: dev.status === 'active' ? '#22c55e' : '#6b7280', flexShrink: 0 }} />
          <div style={{ display: 'flex', flexDirection: 'column', flex: 1 }}>
            <span style={{ fontSize: 13, fontWeight: 600, color: dev.color }}>{dev.name}</span>
            <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.38)', marginTop: 1 }}>{dev.role}</span>
          </div>
          {dev.status === 'retired' && (
            <span style={{ padding: '2px 8px', background: 'rgba(107,114,128,0.15)', color: 'rgba(255,255,255,0.3)', borderRadius: 100, fontSize: 9, border: '1px solid rgba(107,114,128,0.2)', letterSpacing: 1, textTransform: 'uppercase' }}>Fired / Retired</span>
          )}
        </div>
      ))}
    </div>
  </div>
</div>
```

```aura width=900 height=130
<div style={{ position: 'relative', display: 'flex', flexDirection: 'row', gap: 16, alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#07070c', borderRadius: 16, overflow: 'hidden', fontFamily: 'Inter, sans-serif', padding: '0 36px' }}>
  <style>{`
    @keyframes fin-orb { 0%, 100% { transform: translate(0,0); opacity: 0.45; } 50% { transform: translate(18px,-12px); opacity: 0.68; } }
    @keyframes fin-orb-b { 0%, 100% { transform: translate(0,0); opacity: 0.38; } 50% { transform: translate(-14px,10px); opacity: 0.58; } }
    #fo1 { animation: fin-orb 11s ease-in-out infinite; }
    #fo2 { animation: fin-orb-b 13s ease-in-out infinite 1.4s; }
    #fo3 { animation: fin-orb 9s ease-in-out infinite 2.8s; }
  `}</style>
  <svg width="900" height="130" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="fg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(212,175,55,0.38)" />
        <stop offset="100%" stopColor="rgba(212,175,55,0)" />
      </radialGradient>
      <radialGradient id="fg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(34,197,94,0.25)" />
        <stop offset="100%" stopColor="rgba(34,197,94,0)" />
      </radialGradient>
      <radialGradient id="fg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(212,175,55,0.18)" />
        <stop offset="100%" stopColor="rgba(212,175,55,0)" />
      </radialGradient>
    </defs>
    <ellipse id="fo1" cx="120"  cy="65" rx="180" ry="90" fill="url(#fg1)" />
    <ellipse id="fo2" cx="780"  cy="65" rx="170" ry="85" fill="url(#fg2)" />
    <ellipse id="fo3" cx="450"  cy="65" rx="200" ry="75" fill="url(#fg3)" />
  </svg>
  <span style={{ fontSize: 10, color: 'rgba(212,175,55,0.5)', letterSpacing: 4, textTransform: 'uppercase', position: 'relative', zIndex: 10, marginRight: 32 }}>financials</span>
  <div style={{ display: 'flex', gap: 32, zIndex: 10 }}>
    <div style={{ display: 'flex', flexDirection: 'column', alignItems: 'center' }}>
      <span style={{ fontSize: 34, fontWeight: 800, color: '#D4AF37', letterSpacing: -1 }}>80 €</span>
      <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.38)', letterSpacing: 2.5, textTransform: 'uppercase', marginTop: 4 }}>Current Funds</span>
    </div>
    <div style={{ width: '1px', height: 60, background: 'rgba(212,175,55,0.15)', alignSelf: 'center' }} />
    <div style={{ display: 'flex', flexDirection: 'column', alignItems: 'center' }}>
      <span style={{ fontSize: 34, fontWeight: 800, color: '#22c55e', letterSpacing: -1 }}>1 000 €</span>
      <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.38)', letterSpacing: 2.5, textTransform: 'uppercase', marginTop: 4 }}>Active Investment / Month</span>
    </div>
    <div style={{ width: '1px', height: 60, background: 'rgba(212,175,55,0.15)', alignSelf: 'center' }} />
    <div style={{ display: 'flex', flexDirection: 'column', alignItems: 'center' }}>
      <span style={{ fontSize: 34, fontWeight: 800, color: 'rgba(255,255,255,0.55)', letterSpacing: -1 }}>Private</span>
      <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.38)', letterSpacing: 2.5, textTransform: 'uppercase', marginTop: 4 }}>Funding Source</span>
    </div>
  </div>
</div>
```

```aura width=900 height=110
<div style={{ position: 'relative', display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#07070c', borderRadius: 16, overflow: 'hidden', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes leg-orb { 0%, 100% { transform: translate(0,0); opacity: 0.4; } 50% { transform: translate(20px,-12px); opacity: 0.65; } }
    @keyframes leg-orb-b { 0%, 100% { transform: translate(0,0); opacity: 0.35; } 50% { transform: translate(-16px,10px); opacity: 0.55; } }
    #lo1 { animation: leg-orb 11s ease-in-out infinite; }
    #lo2 { animation: leg-orb-b 13s ease-in-out infinite 1.5s; }
    #lo3 { animation: leg-orb 9s ease-in-out infinite 3s; }
  `}</style>
  <svg width="900" height="110" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="lg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(212,175,55,0.35)" />
        <stop offset="100%" stopColor="rgba(212,175,55,0)" />
      </radialGradient>
      <radialGradient id="lg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(184,134,11,0.28)" />
        <stop offset="100%" stopColor="rgba(184,134,11,0)" />
      </radialGradient>
      <radialGradient id="lg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(212,175,55,0.2)" />
        <stop offset="100%" stopColor="rgba(212,175,55,0)" />
      </radialGradient>
    </defs>
    <ellipse id="lo1" cx="80"  cy="55" rx="160" ry="90" fill="url(#lg1)" />
    <ellipse id="lo2" cx="830" cy="55" rx="150" ry="85" fill="url(#lg2)" />
    <ellipse id="lo3" cx="450" cy="55" rx="180" ry="70" fill="url(#lg3)" />
  </svg>
  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10, gap: 6 }}>
    <span style={{ fontSize: 11, color: 'rgba(212,175,55,0.7)', letterSpacing: 3, textTransform: 'uppercase', fontWeight: 600 }}>© ZerdiumCorp · All Rights Reserved</span>
    <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.35)', letterSpacing: 1 }}>All software, source code, and materials are proprietary and confidential. Unauthorized use, reproduction, or distribution is strictly prohibited.</span>
    <div style={{ display: 'flex', gap: 20, marginTop: 4 }}>
      <span style={{ fontSize: 10, color: 'rgba(212,175,55,0.4)', letterSpacing: 1.5, textTransform: 'uppercase' }}>Proprietary License</span>
      <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.15)' }}>·</span>
      <span style={{ fontSize: 10, color: 'rgba(212,175,55,0.4)', letterSpacing: 1.5, textTransform: 'uppercase' }}>No Investment</span>
      <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.15)' }}>·</span>
      <span style={{ fontSize: 10, color: 'rgba(212,175,55,0.4)', letterSpacing: 1.5, textTransform: 'uppercase' }}>Closed Source</span>
      <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.15)' }}>·</span>
      <span style={{ fontSize: 10, color: 'rgba(212,175,55,0.4)', letterSpacing: 1.5, textTransform: 'uppercase' }}>Private Funding</span>
    </div>
  </div>
</div>
```
