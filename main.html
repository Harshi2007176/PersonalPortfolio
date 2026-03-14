import { useState, useEffect, useRef } from "react";

const portfolioData = {
  name: "Harshini Bondila",
  title: "CS Student @ UT Dallas",
  subtitle: "Freshman · Builder · Curious Mind",
  bio: "Hey! I'm Harshini — a Computer Science freshman at the University of Texas at Dallas. I'm passionate about building things with code, always eager to learn, and constantly exploring what technology can do. When I'm not debugging, you'll find me at the gym or binge-watching a good series.",
  hobbies: ["Working out", "Watching movies & TV shows", "Exploring tech"],
  skills: [
    { name: "C / C++", level: 75, icon: "⚙️" },
    { name: "Java", level: 70, icon: "☕" },
    { name: "HTML / CSS", level: 80, icon: "🎨" },
  ],
  contact: {
    email: "Hbondila@gmail.com",
    github: "https://github.com/Harshi2007176",
  },
};

const GithubIcon = () => (
  <svg viewBox="0 0 24 24" width="22" height="22" fill="currentColor">
    <path d="M12 0C5.374 0 0 5.373 0 12c0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23A11.509 11.509 0 0112 5.803c1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576C20.566 21.797 24 17.3 24 12c0-6.627-5.373-12-12-12z"/>
  </svg>
);

const EmailIcon = () => (
  <svg viewBox="0 0 24 24" width="22" height="22" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round">
    <path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/>
    <polyline points="22,6 12,13 2,6"/>
  </svg>
);

function SkillBar({ skill, index }) {
  const [animated, setAnimated] = useState(false);
  const ref = useRef(null);

  useEffect(() => {
    const observer = new IntersectionObserver(
      ([entry]) => { if (entry.isIntersecting) setAnimated(true); },
      { threshold: 0.3 }
    );
    if (ref.current) observer.observe(ref.current);
    return () => observer.disconnect();
  }, []);

  return (
    <div ref={ref} style={{
      background: "white",
      borderRadius: "16px",
      padding: "24px 28px",
      boxShadow: "0 4px 24px rgba(59,130,246,0.07)",
      border: "1px solid #e0eaff",
      animationDelay: `${index * 0.12}s`,
      animation: "fadeUp 0.6s ease both",
    }}>
      <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", marginBottom: "12px" }}>
        <div style={{ display: "flex", alignItems: "center", gap: "10px" }}>
          <span style={{ fontSize: "22px" }}>{skill.icon}</span>
          <span style={{ fontFamily: "'DM Sans', sans-serif", fontWeight: 600, fontSize: "16px", color: "#1e293b" }}>{skill.name}</span>
        </div>
        <span style={{ fontFamily: "'DM Mono', monospace", fontSize: "14px", color: "#3b82f6", fontWeight: 600 }}>{skill.level}%</span>
      </div>
      <div style={{ background: "#e0eaff", borderRadius: "100px", height: "8px", overflow: "hidden" }}>
        <div style={{
          width: animated ? `${skill.level}%` : "0%",
          height: "100%",
          background: "linear-gradient(90deg, #60a5fa, #3b82f6)",
          borderRadius: "100px",
          transition: `width 1.1s cubic-bezier(0.4,0,0.2,1) ${index * 0.15}s`,
        }} />
      </div>
    </div>
  );
}

function Section({ id, children, style = {} }) {
  const ref = useRef(null);
  const [visible, setVisible] = useState(false);
  useEffect(() => {
    const observer = new IntersectionObserver(
      ([e]) => { if (e.isIntersecting) setVisible(true); },
      { threshold: 0.1 }
    );
    if (ref.current) observer.observe(ref.current);
    return () => observer.disconnect();
  }, []);

  return (
    <section id={id} ref={ref} style={{
      opacity: visible ? 1 : 0,
      transform: visible ? "translateY(0)" : "translateY(32px)",
      transition: "opacity 0.7s ease, transform 0.7s ease",
      ...style
    }}>
      {children}
    </section>
  );
}

export default function Portfolio() {
  const [activeNav, setActiveNav] = useState("home");
  const [menuOpen, setMenuOpen] = useState(false);

  const scrollTo = (id) => {
    document.getElementById(id)?.scrollIntoView({ behavior: "smooth" });
    setActiveNav(id);
    setMenuOpen(false);
  };

  useEffect(() => {
    const sections = ["home", "about", "skills", "contact"];
    const observer = new IntersectionObserver(
      (entries) => {
        entries.forEach(e => { if (e.isIntersecting) setActiveNav(e.target.id); });
      },
      { rootMargin: "-40% 0px -55% 0px" }
    );
    sections.forEach(id => {
      const el = document.getElementById(id);
      if (el) observer.observe(el);
    });
    return () => observer.disconnect();
  }, []);

  const navLinks = ["home", "about", "skills", "contact"];

  return (
    <div style={{ fontFamily: "'DM Sans', sans-serif", background: "#f8faff", minHeight: "100vh", color: "#1e293b" }}>
      <style>{`
        @import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@300;400;500;600;700&family=Fraunces:wght@700;900&family=DM+Mono:wght@400;500&display=swap');
        * { margin: 0; padding: 0; box-sizing: border-box; }
        html { scroll-behavior: smooth; }
        @keyframes fadeUp {
          from { opacity: 0; transform: translateY(24px); }
          to { opacity: 1; transform: translateY(0); }
        }
        @keyframes float {
          0%, 100% { transform: translateY(0px); }
          50% { transform: translateY(-10px); }
        }
        @keyframes gradientShift {
          0% { background-position: 0% 50%; }
          50% { background-position: 100% 50%; }
          100% { background-position: 0% 50%; }
        }
        @keyframes pulse {
          0%, 100% { opacity: 1; }
          50% { opacity: 0.5; }
        }
        .nav-link {
          text-decoration: none;
          font-family: 'DM Sans', sans-serif;
          font-size: 14px;
          font-weight: 500;
          color: #64748b;
          padding: 6px 14px;
          border-radius: 100px;
          transition: all 0.2s ease;
          cursor: pointer;
          border: none;
          background: none;
          letter-spacing: 0.5px;
          text-transform: capitalize;
        }
        .nav-link:hover { color: #3b82f6; background: #eff6ff; }
        .nav-link.active { color: #3b82f6; background: #eff6ff; font-weight: 600; }
        .btn-primary {
          background: linear-gradient(135deg, #3b82f6, #2563eb);
          color: white;
          border: none;
          padding: 14px 32px;
          border-radius: 100px;
          font-family: 'DM Sans', sans-serif;
          font-size: 15px;
          font-weight: 600;
          cursor: pointer;
          transition: all 0.25s ease;
          box-shadow: 0 4px 20px rgba(59,130,246,0.3);
          letter-spacing: 0.3px;
        }
        .btn-primary:hover { transform: translateY(-2px); box-shadow: 0 8px 28px rgba(59,130,246,0.4); background: linear-gradient(135deg, #2563eb, #1d4ed8); }
        .btn-outline {
          background: white;
          color: #3b82f6;
          border: 2px solid #3b82f6;
          padding: 12px 28px;
          border-radius: 100px;
          font-family: 'DM Sans', sans-serif;
          font-size: 15px;
          font-weight: 600;
          cursor: pointer;
          transition: all 0.25s ease;
          text-decoration: none;
          display: inline-block;
        }
        .btn-outline:hover { background: #eff6ff; transform: translateY(-2px); }
        .contact-card {
          background: white;
          border-radius: 18px;
          padding: 24px 28px;
          display: flex;
          align-items: center;
          gap: 16px;
          box-shadow: 0 4px 24px rgba(59,130,246,0.07);
          border: 1px solid #e0eaff;
          text-decoration: none;
          color: inherit;
          transition: all 0.25s ease;
        }
        .contact-card:hover { transform: translateY(-4px); box-shadow: 0 12px 36px rgba(59,130,246,0.14); border-color: #93c5fd; }
        .hobby-tag {
          background: #eff6ff;
          color: #3b82f6;
          border: 1px solid #bfdbfe;
          border-radius: 100px;
          padding: 6px 16px;
          font-size: 13px;
          font-weight: 500;
          display: inline-block;
        }
      `}</style>

      {/* NAV */}
      <nav style={{
        position: "fixed", top: 0, left: 0, right: 0, zIndex: 100,
        background: "rgba(248,250,255,0.9)",
        backdropFilter: "blur(16px)",
        borderBottom: "1px solid rgba(224,234,255,0.8)",
        padding: "0 24px",
        height: "64px",
        display: "flex", alignItems: "center", justifyContent: "space-between",
      }}>
        <span style={{ fontFamily: "'Fraunces', serif", fontWeight: 900, fontSize: "22px", color: "#1e293b", letterSpacing: "-0.5px" }}>
          HB<span style={{ color: "#3b82f6" }}>.</span>
        </span>
        <div style={{ display: "flex", gap: "4px" }}>
          {navLinks.map(link => (
            <button key={link} className={`nav-link ${activeNav === link ? "active" : ""}`} onClick={() => scrollTo(link)}>
              {link}
            </button>
          ))}
        </div>
      </nav>

      {/* HERO */}
      <section id="home" style={{
        minHeight: "100vh",
        display: "flex", alignItems: "center", justifyContent: "center",
        padding: "80px 24px 48px",
        position: "relative",
        overflow: "hidden",
      }}>
        {/* Background decoration */}
        <div style={{
          position: "absolute", top: "10%", right: "5%",
          width: "420px", height: "420px",
          background: "radial-gradient(circle, rgba(59,130,246,0.1) 0%, transparent 70%)",
          borderRadius: "50%",
          pointerEvents: "none",
        }} />
        <div style={{
          position: "absolute", bottom: "15%", left: "2%",
          width: "280px", height: "280px",
          background: "radial-gradient(circle, rgba(96,165,250,0.07) 0%, transparent 70%)",
          borderRadius: "50%",
          pointerEvents: "none",
        }} />

        <div style={{ maxWidth: "680px", textAlign: "center", animation: "fadeUp 0.8s ease both" }}>
          {/* Avatar */}
          <div style={{
            width: "100px", height: "100px",
            background: "linear-gradient(135deg, #60a5fa, #3b82f6, #2563eb)",
            borderRadius: "50%",
            margin: "0 auto 32px",
            display: "flex", alignItems: "center", justifyContent: "center",
            fontSize: "40px",
            boxShadow: "0 8px 32px rgba(59,130,246,0.3)",
            animation: "float 4s ease-in-out infinite",
          }}>
            👩‍💻
          </div>

          <div style={{
            display: "inline-flex", alignItems: "center", gap: "8px",
            background: "#eff6ff", border: "1px solid #bfdbfe",
            borderRadius: "100px", padding: "6px 16px",
            marginBottom: "20px",
            animation: "fadeUp 0.8s ease 0.1s both",
          }}>
            <span style={{ width: "8px", height: "8px", background: "#22c55e", borderRadius: "50%", animation: "pulse 2s infinite" }} />
            <span style={{ fontSize: "13px", fontWeight: 500, color: "#3b82f6" }}>CS Freshman @ UT Dallas</span>
          </div>

          <h1 style={{
            fontFamily: "'Fraunces', serif",
            fontWeight: 900,
            fontSize: "clamp(42px, 8vw, 72px)",
            lineHeight: 1.05,
            letterSpacing: "-2px",
            color: "#0f172a",
            marginBottom: "16px",
            animation: "fadeUp 0.8s ease 0.2s both",
          }}>
            Harshini<br />
            <span style={{ color: "#3b82f6" }}>Bondila</span>
          </h1>

          <p style={{
            fontSize: "18px", color: "#64748b", lineHeight: 1.7,
            marginBottom: "40px", fontWeight: 400,
            animation: "fadeUp 0.8s ease 0.3s both",
          }}>
            Passionate about writing clean code, solving problems,<br />and building things that matter.
          </p>

          <div style={{ display: "flex", gap: "14px", justifyContent: "center", flexWrap: "wrap", animation: "fadeUp 0.8s ease 0.4s both" }}>
            <button className="btn-primary" onClick={() => scrollTo("contact")}>Get in touch</button>
            <button className="btn-outline" onClick={() => scrollTo("about")}>About me</button>
          </div>
        </div>
      </section>

      {/* ABOUT */}
      <Section id="about" style={{ padding: "80px 24px", maxWidth: "860px", margin: "0 auto" }}>
        <div style={{ textAlign: "center", marginBottom: "48px" }}>
          <span style={{ fontSize: "13px", fontWeight: 600, color: "#3b82f6", letterSpacing: "2px", textTransform: "uppercase" }}>Who I am</span>
          <h2 style={{ fontFamily: "'Fraunces', serif", fontWeight: 900, fontSize: "clamp(32px, 5vw, 48px)", letterSpacing: "-1px", marginTop: "8px", color: "#0f172a" }}>
            About Me
          </h2>
        </div>

        <div style={{
          background: "white", borderRadius: "24px",
          padding: "clamp(28px, 5vw, 48px)",
          boxShadow: "0 4px 40px rgba(59,130,246,0.08)",
          border: "1px solid #e0eaff",
          display: "grid", gridTemplateColumns: "1fr 1fr", gap: "40px",
        }}>
          <div>
            <p style={{ fontSize: "16px", lineHeight: 1.85, color: "#475569", marginBottom: "24px" }}>
              {portfolioData.bio}
            </p>
            <div style={{ display: "flex", flexWrap: "wrap", gap: "8px" }}>
              {portfolioData.hobbies.map((h, i) => (
                <span key={i} className="hobby-tag">{h}</span>
              ))}
            </div>
          </div>
          <div style={{ display: "flex", flexDirection: "column", gap: "20px" }}>
            {[
              { icon: "🎓", label: "University", value: "UT Dallas" },
              { icon: "📚", label: "Major", value: "Computer Science" },
              { icon: "🌱", label: "Year", value: "Freshman (2024–2028)" },
              { icon: "📍", label: "Location", value: "Dallas, TX" },
            ].map((item, i) => (
              <div key={i} style={{ display: "flex", alignItems: "center", gap: "14px" }}>
                <div style={{
                  width: "44px", height: "44px", background: "#eff6ff",
                  borderRadius: "12px", display: "flex", alignItems: "center", justifyContent: "center",
                  fontSize: "20px", flexShrink: 0,
                }}>
                  {item.icon}
                </div>
                <div>
                  <div style={{ fontSize: "11px", fontWeight: 600, color: "#94a3b8", letterSpacing: "1px", textTransform: "uppercase" }}>{item.label}</div>
                  <div style={{ fontSize: "15px", fontWeight: 600, color: "#1e293b" }}>{item.value}</div>
                </div>
              </div>
            ))}
          </div>
        </div>
      </Section>

      {/* SKILLS */}
      <Section id="skills" style={{ padding: "80px 24px", maxWidth: "860px", margin: "0 auto" }}>
        <div style={{ textAlign: "center", marginBottom: "48px" }}>
          <span style={{ fontSize: "13px", fontWeight: 600, color: "#3b82f6", letterSpacing: "2px", textTransform: "uppercase" }}>What I know</span>
          <h2 style={{ fontFamily: "'Fraunces', serif", fontWeight: 900, fontSize: "clamp(32px, 5vw, 48px)", letterSpacing: "-1px", marginTop: "8px", color: "#0f172a" }}>
            Skills
          </h2>
          <p style={{ color: "#64748b", marginTop: "12px", fontSize: "16px" }}>Languages I've been learning and working with</p>
        </div>
        <div style={{ display: "flex", flexDirection: "column", gap: "16px" }}>
          {portfolioData.skills.map((skill, i) => (
            <SkillBar key={i} skill={skill} index={i} />
          ))}
        </div>

        {/* Learning banner */}
        <div style={{
          marginTop: "32px",
          background: "linear-gradient(135deg, #eff6ff, #dbeafe)",
          border: "1px solid #bfdbfe",
          borderRadius: "16px",
          padding: "24px 28px",
          display: "flex", alignItems: "center", gap: "16px",
        }}>
          <span style={{ fontSize: "28px" }}>🚀</span>
          <div>
            <div style={{ fontWeight: 700, color: "#1e40af", fontSize: "15px", marginBottom: "4px" }}>Always learning</div>
            <div style={{ color: "#3b82f6", fontSize: "14px" }}>Exploring data structures, algorithms, and more as a CS freshman — just getting started!</div>
          </div>
        </div>
      </Section>

      {/* CONTACT */}
      <Section id="contact" style={{ padding: "80px 24px 100px", maxWidth: "660px", margin: "0 auto" }}>
        <div style={{ textAlign: "center", marginBottom: "48px" }}>
          <span style={{ fontSize: "13px", fontWeight: 600, color: "#3b82f6", letterSpacing: "2px", textTransform: "uppercase" }}>Say hello</span>
          <h2 style={{ fontFamily: "'Fraunces', serif", fontWeight: 900, fontSize: "clamp(32px, 5vw, 48px)", letterSpacing: "-1px", marginTop: "8px", color: "#0f172a" }}>
            Contact
          </h2>
          <p style={{ color: "#64748b", marginTop: "12px", fontSize: "16px" }}>I'd love to connect — whether it's to collaborate, learn, or just chat!</p>
        </div>

        <div style={{ display: "flex", flexDirection: "column", gap: "16px" }}>
          <a className="contact-card" href={`mailto:${portfolioData.contact.email}`}>
            <div style={{ width: "48px", height: "48px", background: "#eff6ff", borderRadius: "14px", display: "flex", alignItems: "center", justifyContent: "center", color: "#3b82f6", flexShrink: 0 }}>
              <EmailIcon />
            </div>
            <div>
              <div style={{ fontSize: "12px", fontWeight: 600, color: "#94a3b8", letterSpacing: "1px", textTransform: "uppercase", marginBottom: "2px" }}>Email</div>
              <div style={{ fontWeight: 600, color: "#1e293b", fontSize: "15px" }}>{portfolioData.contact.email}</div>
            </div>
          </a>

          <a className="contact-card" href={portfolioData.contact.github} target="_blank" rel="noopener noreferrer">
            <div style={{ width: "48px", height: "48px", background: "#f1f5f9", borderRadius: "14px", display: "flex", alignItems: "center", justifyContent: "center", color: "#334155", flexShrink: 0 }}>
              <GithubIcon />
            </div>
            <div>
              <div style={{ fontSize: "12px", fontWeight: 600, color: "#94a3b8", letterSpacing: "1px", textTransform: "uppercase", marginBottom: "2px" }}>GitHub</div>
              <div style={{ fontWeight: 600, color: "#1e293b", fontSize: "15px" }}>github.com/Harshi2007176</div>
            </div>
          </a>
        </div>

        <p style={{ textAlign: "center", color: "#94a3b8", fontSize: "14px", marginTop: "40px" }}>
          Made with 💙 by Harshini Bondila
        </p>
      </Section>
    </div>
  );
}
