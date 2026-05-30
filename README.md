<div style={{
  display: 'flex',
  flexDirection: 'column',
  justifyContent: 'center',
  alignItems: 'flex-start',
  width: '100%',
  height: '100%',
  background: 'linear-gradient(135deg, #0a0a0f 0%, #0d0d1a 50%, #0a0f0a 100%)',
  padding: '48px 56px',
  position: 'relative',
  overflow: 'hidden',
}}>
  <style>{`
    @keyframes shimmer {
      0% { opacity: 0.3; transform: translateX(-10px); }
      50% { opacity: 0.7; }
      100% { opacity: 0.3; transform: translateX(10px); }
    }
    @keyframes fadeUp {
      0% { opacity: 0; transform: translateY(12px); }
      100% { opacity: 1; transform: translateY(0); }
    }
    #line1 { animation: fadeUp 0.6s ease forwards; }
    #line2 { animation: fadeUp 0.6s 0.15s ease both; }
    #accent { animation: shimmer 3s ease-in-out infinite; }
  `}</style>

  {/* Decorative orb top-right */}
  <div id="accent" style={{
    position: 'absolute',
    top: -60,
    right: -60,
    width: 220,
    height: 220,
    borderRadius: '50%',
    background: 'radial-gradient(circle, rgba(120,255,120,0.12) 0%, rgba(80,200,80,0.04) 60%, transparent 100%)',
  }} />

  {/* Thin accent line */}
  <div style={{
    width: 40,
    height: 2,
    background: 'rgba(160,255,160,0.6)',
    marginBottom: 24,
  }} />

  {/* Name */}
  <div id="line1" style={{
    fontSize: 52,
    fontWeight: 700,
    color: '#f0f0f0',
    letterSpacing: '-1.5px',
    lineHeight: 1.1,
    marginBottom: 12,
    fontFamily: 'Inter',
  }}>
    JESTIN JN
  </div>

  {/* Role line */}
  <div id="line2" style={{
    fontSize: 15,
    color: 'rgba(255,255,255,0.4)',
    letterSpacing: '3px',
    textTransform: 'uppercase',
    fontFamily: 'Inter',
    fontWeight: 400,
  }}>
    Civil Engineer · Designer · Writer
  </div>

  {/* Bottom tag */}
  <div style={{
    position: 'absolute',
    bottom: 32,
    right: 56,
    fontSize: 11,
    color: 'rgba(255,255,255,0.18)',
    letterSpacing: '2px',
    fontFamily: 'Inter',
  }}>
    CSIR-SERC · Chennai
  </div>
</div>
