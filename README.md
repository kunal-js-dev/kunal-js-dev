import React from "react";

const projects = [ { title: "🌿 Air Quality System", desc: "IoT Monitoring using Arduino (DHT11 + MQ135)", repo: "https://github.com/kunal-js-dev/air-quality-monitor", demo: "https://your-air-quality-demo.vercel.app" }, { title: "🤖 Nova AI", desc: "Voice + Automation Assistant", repo: "https://github.com/kunal-js-dev/nova-ai", demo: "https://your-nova-ai-demo.vercel.app" }, { title: "📚 LearnFlow Portal", desc: "Web learning platform built with TypeScript", repo: "https://github.com/kunal-js-dev/learnflow-portal", demo: "https://learnflow-portal.vercel.app" } ];

export default function Portfolio() { return ( <div className="min-h-screen bg-black text-cyan-400 font-mono p-6"> {/* HERO */} <div className="text-center mb-10"> <h1 className="text-4xl font-bold">⚡ KUNAL.JS</h1> <p className="text-lg mt-2">AI + IoT Developer • Smart Systems Builder</p> </div>

{/* PLAYER PROFILE */}
  <div className="border border-cyan-500 p-4 rounded-2xl mb-6">
    <h2 className="text-xl mb-2">🎮 PLAYER PROFILE</h2>
    <p>Name: Kunal JS</p>
    <p>Class: AI + IoT Developer</p>
    <p>Level: 07</p>
  </div>

  {/* SKILLS */}
  <div className="border border-cyan-500 p-4 rounded-2xl mb-6">
    <h2 className="text-xl mb-2">🌌 SKILL TREE</h2>
    <ul>
      <li>AI Systems ███████░░░</li>
      <li>IoT Dev ████████░░</li>
      <li>Web Dev ███████░░░</li>
    </ul>
  </div>

  {/* PROJECTS */}
  <div className="border border-cyan-500 p-4 rounded-2xl mb-6">
    <h2 className="text-xl mb-4">⚔️ PROJECT ARENA</h2>
    <div className="grid grid-cols-1 md:grid-cols-3 gap-4">
      {projects.map((p, i) => (
        <div key={i} className="border border-cyan-400 p-4 rounded-xl hover:shadow-[0_0_15px_cyan] transition">
          <h3 className="text-lg font-bold mb-2">{p.title}</h3>
          <p className="mb-3">{p.desc}</p>

          <div className="flex gap-3">
            <a
              href={p.repo}
              target="_blank"
              rel="noreferrer"
              className="px-3 py-1 border border-cyan-400 rounded hover:bg-cyan-400 hover:text-black"
            >
              🔗 Repo
            </a>

            <a
              href={p.demo}
              target="_blank"
              rel="noreferrer"
              className="px-3 py-1 border border-green-400 rounded hover:bg-green-400 hover:text-black"
            >
              🚀 Live
            </a>
          </div>
        </div>
      ))}
    </div>
  </div>

  {/* CONTACT */}
  <div className="text-center mt-10 space-y-3">
    <p>📧 kunalkunal2915@gmail.com</p>

    <div className="flex justify-center gap-4">
      <a
        href="https://www.linkedin.com/in/kunal-j-s-8b4227384"
        target="_blank"
        rel="noreferrer"
        className="px-4 py-2 border border-blue-400 rounded-xl backdrop-blur-md bg-white/5 hover:bg-blue-400 hover:text-black hover:shadow-[0_0_20px_#60a5fa] transition"
      >
        🔗 LinkedIn
      </a>

      <a
        href="mailto:kunalkunal2915@gmail.com"
        className="px-4 py-2 border border-cyan-400 rounded-xl backdrop-blur-md bg-white/5 hover:bg-cyan-400 hover:text-black hover:shadow-[0_0_20px_cyan] transition"
      >
        📧 Email
      </a>
    </div>
  </div>
</div>

); }