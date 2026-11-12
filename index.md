---
layout: default
title: 首页
---

<!-- Hero Section -->
<section class="hero-box">
  <div class="hero-badge-row">
    <span class="hero-badge">💼 数字游民</span>
    <span class="hero-badge">🚗 极客自驾</span>
    <span class="hero-badge">⚡️ AI Agent & 自动化</span>
  </div>
  <h1 class="hero-title">你好，我是 HFly 👋</h1>
  <p class="hero-lead">
    专注于 <strong>AI 自动化、知识工程与轻量开发</strong>。<br>
    用代码构建趁手的生产力工具，用方向盘与镜头在路上丈量真实的物理世界。
  </p>
  <div class="hero-actions">
    <a href="#articles" class="btn-primary">📝 阅读最新文章</a>
    <a href="#projects" class="btn-secondary">🚀 精选开源项目</a>
    <a href="https://github.com/hfly2019" target="_blank" rel="noopener" class="btn-secondary">🐙 GitHub @hfly2019</a>
  </div>
</section>

<!-- Featured Projects Section -->
<section id="projects">
  <div class="section-head">
    <h2 class="section-title">🚀 精选开源与工具</h2>
    <span class="section-sub">Code & Tools</span>
  </div>

  <div class="project-grid">
    <div class="project-card">
      <div class="project-top">
        <h3 class="project-name">Hotlink Downloader Enhanced</h3>
        <span class="project-tag">Obsidian 插件</span>
      </div>
      <p class="project-desc">
        增强版 Obsidian 外链图片本地化下载插件，深度适配自定义附件存放路径与网络重试，解决笔记图床失效痛点。
      </p>
      <div class="project-meta">
        <span>⭐ 3 Stars · TypeScript</span>
        <a href="https://github.com/hfly2019/hotlink-image-downloader-enhanced" target="_blank" rel="noopener" class="project-link">
          查看仓库 →
        </a>
      </div>
    </div>

    <div class="project-card">
      <div class="project-top">
        <h3 class="project-name">CN Math Taxonomy</h3>
        <span class="project-tag">知识图谱 / 教育</span>
      </div>
      <p class="project-desc">
        初中数学知识图谱 + 前置诊断系统：完整对齐国家课程标准、人教版七–九年级 333 个核心知识点与自适应诊断。
      </p>
      <div class="project-meta">
        <span>Open Data · Python</span>
        <a href="https://github.com/hfly2019/cn-math-taxonomy" target="_blank" rel="noopener" class="project-link">
          查看仓库 →
        </a>
      </div>
    </div>

    <div class="project-card">
      <div class="project-top">
        <h3 class="project-name">Memos AI Sync+</h3>
        <span class="project-tag">AI 同步 / 笔记</span>
      </div>
      <p class="project-desc">
        Obsidian Memos AI Sync 强化分支：针对移动端界面交互进行深度重构，扩展 NVIDIA Cloud / 本地大模型智能双向同步。
      </p>
      <div class="project-meta">
        <span>Obsidian Plugin · AI</span>
        <a href="https://github.com/hfly2019/obsidian-memos-ai-sync-plus" target="_blank" rel="noopener" class="project-link">
          查看仓库 →
        </a>
      </div>
    </div>

    <div class="project-card">
      <div class="project-top">
        <h3 class="project-name">Shadowrocket Rules</h3>
        <span class="project-tag">网络规则集</span>
      </div>
      <p class="project-desc">
        个人精选 Shadowrocket 分流策略、独立模块与规则自动化维护脚本，追求极致纯净与高速直连体验。
      </p>
      <div class="project-meta">
        <span>Personal · Config</span>
        <a href="https://github.com/hfly2019/shadowrocket-rules" target="_blank" rel="noopener" class="project-link">
          查看仓库 →
        </a>
      </div>
    </div>
  </div>
</section>

<!-- Latest Articles Section -->
<section id="articles">
  <div class="section-head">
    <h2 class="section-title">📝 最新文章</h2>
    <span class="section-sub">Writing & Notes</span>
  </div>

  <div class="post-list">
    {% for post in site.posts %}
      <a href="{{ post.url }}" class="post-card">
        <div class="post-card-header">
          <span class="post-card-date">📅 {{ post.date | date: "%Y年%m月%d日" }}</span>
          {% if post.tags %}
            <span class="tag-badge">#{{ post.tags | first }}</span>
          {% endif %}
        </div>
        <h3 class="post-card-title">{{ post.title }}</h3>
        {% if post.description %}
          <p class="post-card-desc">{{ post.description }}</p>
        {% endif %}
      </a>
    {% endfor %}
  </div>
</section>

<!-- About Section -->
<section id="about">
  <div class="section-head">
    <h2 class="section-title">🧭 关于与生活方式</h2>
    <span class="section-sub">About & Lifestyle</span>
  </div>

  <div class="about-box">
    <p style="margin-top: 0; font-size: 1.05rem; line-height: 1.7;">
      信奉“Context not Control”的 AI 协作哲学与 MECE 原则。生活与折腾主要分布在以下三个切面：
    </p>

    <div class="about-features">
      <div class="about-item">
        <div class="about-item-title">⚡️ AI Agent & 自动化</div>
        <p class="about-item-desc">
          探索 Hermes Agent 与多端通信集成；基于 Mac mini M4 本地推理与端侧自动化，重复超过 3 次的流程必写代码自动化。
        </p>
      </div>

      <div class="about-item">
        <div class="about-item-title">📚 第二大脑 (Obsidian)</div>
        <p class="about-item-desc">
          基于双链、Canvas 与分层记忆模型搭建的个人知识库。持续记录技术剪藏、哲学思考与日常反思。
        </p>
      </div>

      <div class="about-item">
        <div class="about-item-title">🚗 自驾探索与摄影</div>
        <p class="about-item-desc">
          热爱周末逃离与长途公路穿越。驾驶 Tesla Model Y 寻访山川与未知风景，在自然中保持敏锐感受。
        </p>
      </div>
    </div>
  </div>
</section>
