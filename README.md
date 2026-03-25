import { motion } from "framer-motion";

export default function HrithikPortfolio() {
  const projects = [
    {
      title: "Face Recognition Attendance System",
      description:
        "A Python-based computer vision system that detects faces and automates attendance tracking.",
      tech: ["Python", "OpenCV", "Computer Vision"],
      github: "#",
      demo: "#",
    },
    {
      title: "Stochastic Resonance Simulator",
      description:
        "A simulation project exploring stochastic resonance phenomena for signal processing experiments.",
      tech: ["Python", "Signal Processing"],
      github: "#",
      demo: "#",
    },
    {
      title: "Job Application Tracker",
      description:
        "A web application for tracking job applications and managing application status efficiently.",
      tech: ["JavaScript", "HTML", "CSS"],
      github: "#",
      demo: "#",
    },
    {
      title: "GitHub Issues Tracker",
      description:
        "A JavaScript project for organizing and tracking GitHub issues in a clean workflow.",
      tech: ["JavaScript", "GitHub API"],
      github: "#",
      demo: "#",
    },
  ];

  const skills = [
    "HTML",
    "CSS",
    "JavaScript",
    "React",
    "Python",
    "Git",
    "GitHub",
    "UI/UX",
  ];

  const fadeUp = {
    hidden: { opacity: 0, y: 24 },
    visible: (i = 0) => ({
      opacity: 1,
      y: 0,
      transition: { duration: 0.6, delay: i * 0.12 },
    }),
  };

  return (
    <div className="min-h-screen bg-slate-950 text-white">
      <motion.section
        initial="hidden"
        animate="visible"
        variants={fadeUp}
        className="relative overflow-hidden border-b border-white/10"
      >
        <div className="absolute inset-0 bg-gradient-to-br from-blue-600/20 via-cyan-400/10 to-transparent" />
        <motion.div
          animate={{ y: [0, -12, 0], x: [0, 8, 0] }}
          transition={{ duration: 8, repeat: Infinity, ease: "easeInOut" }}
          className="absolute -top-24 -right-24 h-72 w-72 rounded-full bg-blue-500/20 blur-3xl"
        />
        <motion.div
          animate={{ y: [0, 14, 0], x: [0, -10, 0] }}
          transition={{ duration: 9, repeat: Infinity, ease: "easeInOut" }}
          className="absolute -bottom-24 -left-24 h-72 w-72 rounded-full bg-cyan-500/20 blur-3xl"
        />

        <div className="relative mx-auto max-w-6xl px-6 py-24 md:px-10 lg:px-12">
          <div className="grid items-center gap-12 md:grid-cols-2">
            <div>
              <p className="mb-4 inline-flex rounded-full border border-blue-400/30 bg-blue-500/10 px-4 py-1 text-sm text-blue-200">
                Computer Science Student • Front-End Developer
              </p>
              <h1 className="text-4xl font-bold leading-tight md:text-6xl">
                Hi, I&apos;m <span className="text-blue-400">Hrithik Majumader</span>
              </h1>
              <p className="mt-6 max-w-xl text-lg text-slate-300">
                I build modern, responsive web experiences and explore AI-driven
                solutions with a strong interest in machine learning, computer
                vision, and user-focused design.
              </p>
              <div className="mt-8 flex flex-wrap gap-4">
                <a
                  href="#projects"
                  className="rounded-2xl bg-blue-500 px-6 py-3 font-medium text-white shadow-lg shadow-blue-500/20 transition hover:-translate-y-0.5"
                >
                  View Projects
                </a>
                <a
                  href="#contact"
                  className="rounded-2xl border border-white/15 px-6 py-3 font-medium text-slate-200 transition hover:bg-white/5"
                >
                  Contact Me
                </a>
              </div>
            </div>

            <div className="flex justify-center md:justify-end">
              <div className="w-full max-w-md rounded-[2rem] border border-white/10 bg-white/5 p-6 shadow-2xl backdrop-blur">
                <div className="rounded-[1.5rem] border border-white/10 bg-slate-900 p-6">
                  <div className="mb-6 flex items-center gap-4">
                    <motion.div
                    animate={{ scale: [1, 1.05, 1] }}
                    transition={{ duration: 3, repeat: Infinity, ease: "easeInOut" }}
                    className="flex h-16 w-16 items-center justify-center rounded-2xl bg-blue-500/20 text-2xl font-bold text-blue-300"
                  >
                      HM
                    </motion.div>
                    <div>
                      <h2 className="text-xl font-semibold">Hrithik Majumader</h2>
                      <p className="text-slate-400">Khulna, Bangladesh</p>
                    </div>
                  </div>

                  <div className="space-y-4 text-sm text-slate-300">
                    <div className="rounded-2xl bg-white/5 p-4">
                      <p className="text-slate-400">Current Focus</p>
                      <p className="mt-1 font-medium text-white">
                        React, JavaScript, UI/UX, AI/ML
                      </p>
                    </div>
                    <div className="rounded-2xl bg-white/5 p-4">
                      <p className="text-slate-400">Interests</p>
                      <p className="mt-1 font-medium text-white">
                        Web Development, Computer Vision, NLP, Cybersecurity
                      </p>
                    </div>
                    <div className="rounded-2xl bg-white/5 p-4">
                      <p className="text-slate-400">Goal</p>
                      <p className="mt-1 font-medium text-white">
                        Become a full-stack developer with AI expertise
                      </p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </motion.section>

      <motion.section
        initial="hidden"
        whileInView="visible"
        viewport={{ once: true, amount: 0.2 }}
        variants={fadeUp}
        className="mx-auto max-w-6xl px-6 py-20 md:px-10 lg:px-12"
        id="about"
      >
        <div className="grid gap-10 md:grid-cols-[1.2fr_0.8fr]">
          <div>
            <p className="text-sm uppercase tracking-[0.2em] text-blue-300">About Me</p>
            <h2 className="mt-3 text-3xl font-bold md:text-4xl">Building clean digital experiences with strong technical foundations.</h2>
            <p className="mt-6 text-slate-300 leading-8">
              I am a Computer Science student passionate about creating useful,
              polished, and user-friendly products. My work combines front-end
              development with curiosity for artificial intelligence and modern
              problem-solving. I enjoy turning ideas into practical projects and
              continuously improving my technical and design skills.
            </p>
          </div>

          <div className="grid gap-4">
            <div className="rounded-3xl border border-white/10 bg-white/5 p-6">
              <h3 className="text-lg font-semibold">Education</h3>
              <p className="mt-2 text-slate-300">Computer Science Student</p>
            </div>
            <div className="rounded-3xl border border-white/10 bg-white/5 p-6">
              <h3 className="text-lg font-semibold">Learning Now</h3>
              <p className="mt-2 text-slate-300">JavaScript, React, Web Development, UI/UX Design</p>
            </div>
            <div className="rounded-3xl border border-white/10 bg-white/5 p-6">
              <h3 className="text-lg font-semibold">Location</h3>
              <p className="mt-2 text-slate-300">Khulna, Bangladesh</p>
            </div>
          </div>
        </div>
      </motion.section>

      <motion.section
        initial="hidden"
        whileInView="visible"
        viewport={{ once: true, amount: 0.2 }}
        variants={fadeUp}
        className="border-y border-white/10 bg-white/[0.03]"
      >
        <div className="mx-auto max-w-6xl px-6 py-20 md:px-10 lg:px-12" id="skills">
          <p className="text-sm uppercase tracking-[0.2em] text-blue-300">Tech Stack</p>
          <h2 className="mt-3 text-3xl font-bold md:text-4xl">Skills & Tools</h2>
          <div className="mt-10 flex flex-wrap gap-4">
            {skills.map((skill, index) => (
              <motion.span
                custom={index}
                initial="hidden"
                whileInView="visible"
                viewport={{ once: true }}
                variants={fadeUp}
                key={skill}
                className="rounded-2xl border border-blue-400/20 bg-blue-500/10 px-5 py-3 text-sm font-medium text-blue-100"
              >
                {skill}
              </motion.span>
            ))}
          </div>
        </div>
      </motion.section>

      <motion.section
        initial="hidden"
        whileInView="visible"
        viewport={{ once: true, amount: 0.15 }}
        variants={fadeUp}
        className="mx-auto max-w-6xl px-6 py-20 md:px-10 lg:px-12"
        id="projects"
      >
        <p className="text-sm uppercase tracking-[0.2em] text-blue-300">Portfolio</p>
        <h2 className="mt-3 text-3xl font-bold md:text-4xl">Featured Projects</h2>
        <div className="mt-10 grid gap-6 md:grid-cols-2">
          {projects.map((project, index) => (
            <motion.div
              custom={index}
              initial="hidden"
              whileInView="visible"
              viewport={{ once: true, amount: 0.2 }}
              variants={fadeUp}
              key={project.title}
              className="rounded-[2rem] border border-white/10 bg-white/5 p-6 shadow-xl transition hover:-translate-y-2 hover:shadow-2xl"
            >
              <h3 className="text-2xl font-semibold">{project.title}</h3>
              <p className="mt-4 leading-7 text-slate-300">{project.description}</p>
              <div className="mt-5 flex flex-wrap gap-2">
                {project.tech.map((item) => (
                  <span
                    key={item}
                    className="rounded-full bg-slate-800 px-3 py-1 text-xs text-slate-200"
                  >
                    {item}
                  </span>
                ))}
              </div>
              <div className="mt-6 flex gap-3">
                <a
                  href={project.github}
                  className="rounded-xl border border-white/15 px-4 py-2 text-sm font-medium text-white transition hover:bg-white/5"
                >
                  GitHub
                </a>
                <a
                  href={project.demo}
                  className="rounded-xl bg-blue-500 px-4 py-2 text-sm font-medium text-white transition hover:opacity-90"
                >
                  Live Demo
                </a>
              </div>
            </motion.div>
          ))}
        </div>
      </motion.section>

      <motion.section
        initial="hidden"
        whileInView="visible"
        viewport={{ once: true, amount: 0.2 }}
        variants={fadeUp}
        className="border-t border-white/10 bg-white/[0.03]"
      >
        <div className="mx-auto grid max-w-6xl gap-8 px-6 py-20 md:grid-cols-2 md:px-10 lg:px-12">
          <div>
            <p className="text-sm uppercase tracking-[0.2em] text-blue-300">Why Me</p>
            <h2 className="mt-3 text-3xl font-bold md:text-4xl">Focused on growth, quality, and real-world impact.</h2>
          </div>
          <div className="grid gap-4">
            <div className="rounded-3xl border border-white/10 bg-white/5 p-5 text-slate-300">
              Strong interest in building responsive, user-friendly, and visually polished interfaces.
            </div>
            <div className="rounded-3xl border border-white/10 bg-white/5 p-5 text-slate-300">
              Curious mindset across AI, machine learning, computer vision, NLP, and cybersecurity.
            </div>
            <div className="rounded-3xl border border-white/10 bg-white/5 p-5 text-slate-300">
              Dedicated to continuous learning, project building, and improving problem-solving skills.
            </div>
          </div>
        </div>
      </motion.section>

      <motion.section
        initial="hidden"
        whileInView="visible"
        viewport={{ once: true, amount: 0.2 }}
        variants={fadeUp}
        className="mx-auto max-w-6xl px-6 py-20 md:px-10 lg:px-12"
        id="contact"
      >
        <div className="rounded-[2rem] border border-white/10 bg-gradient-to-br from-blue-500/10 to-cyan-500/10 p-8 md:p-12">
          <p className="text-sm uppercase tracking-[0.2em] text-blue-300">Contact</p>
          <h2 className="mt-3 text-3xl font-bold md:text-4xl">Let&apos;s connect and build something meaningful.</h2>
          <p className="mt-4 max-w-2xl text-slate-300">
            I am open to collaboration, project opportunities, and learning from
            other developers and creators.
          </p>
          <div className="mt-8 flex flex-wrap gap-4">
            <a
              href="https://www.linkedin.com/in/hrithikmajumader"
              className="rounded-2xl bg-white px-6 py-3 font-medium text-slate-900 transition hover:-translate-y-0.5"
            >
              LinkedIn
            </a>
            <a
              href="mailto:hrithikmajumader@163.com"
              className="rounded-2xl border border-white/15 px-6 py-3 font-medium text-white transition hover:bg-white/5"
            >
              Email Me
            </a>
          </div>
        </div>
      </motion.section>
    </div>
  );
}

