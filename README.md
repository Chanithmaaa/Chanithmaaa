export default function SkillsSection() {
  const devTools = [
    "Python", "Java", "JavaScript", "Next.js", "React",
    "HTML5", "CSS3", "MySQL", "Vercel", "GitHub", "IntelliJ", "VS Code"
  ];

  const aiTools = [
    "Firebase", "Supabase", "Raspberry Pi", "TensorFlow", "OpenCV"
  ];

  const designTools = [
    "Photoshop", "Illustrator", "Premiere Pro", "After Effects", "Figma"
  ];

  return (
    <section className="min-h-screen bg-[#020817] text-white flex flex-col items-center justify-center px-6 py-20">
      <h2 className="text-4xl font-bold mb-10">Languages and Tools:</h2>

      <div className="text-center mb-10">
        <h3 className="text-2xl font-semibold mb-6">Development & Web</h3>
        <div className="flex flex-wrap justify-center gap-4 max-w-4xl">
          {devTools.map((tool) => (
            <div
              key={tool}
              className="px-5 py-3 rounded-2xl bg-slate-800 shadow-lg border border-slate-700 hover:scale-105 transition"
            >
              {tool}
            </div>
          ))}
        </div>
      </div>

      <div className="text-center mb-10">
        <h3 className="text-2xl font-semibold mb-6">IoT & AI Stack</h3>
        <div className="flex flex-wrap justify-center gap-4 max-w-3xl">
          {aiTools.map((tool) => (
            <div
              key={tool}
              className="px-5 py-3 rounded-2xl bg-slate-800 shadow-lg border border-slate-700 hover:scale-105 transition"
            >
              {tool}
            </div>
          ))}
        </div>
      </div>

      <div className="text-center">
        <h3 className="text-2xl font-semibold mb-6">Design & Editing</h3>
        <div className="flex flex-wrap justify-center gap-4 max-w-3xl">
          {designTools.map((tool) => (
            <div
              key={tool}
              className="px-5 py-3 rounded-2xl bg-slate-800 shadow-lg border border-slate-700 hover:scale-105 transition"
            >
              {tool}
            </div>
          ))}
        </div>
      </div>
    </section>
  );
}
