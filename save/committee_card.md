<section class="member-section">
<div class="member-card">
    <div class="member-photo">
      <img src="assets/images/USC.jpg" alt="USC" />
    </div>
    <div class="member-info">
      <h2 class="member-name">Zlatko Bodrožić</h2>
      <div class="member-meta">
        <p>University of Liverpool, UK (Lead Coordinator)</p>
        <a href="mailto:Z.Bodrozic@liverpool.ac.uk">Z.Bodrozic@liverpool.ac.uk</a>
        <p>Introduction</p>
      </div>
    </div>
  </div>

<div class="member-card">
    <div class="member-photo">
      <img src="assets/images/Pilar.jpg" alt="Pilar" />
    </div>
    <div class="member-info">
      <h2 class="member-name">Pilar Acosta</h2>
      <div class="member-meta">
        <p>Toulouse Business School, France</p>
        <a href="mailto:p.acosta@tbs-education.fr">p.acosta@tbs-education.fr</a>
        <p>Introduction</p>
      </div>
    </div>
  </div>

<div class="member-card">
    <div class="member-photo">
      <img src="assets/images/Paul.jpg" alt="Paul" />
    </div>
    <div class="member-info">
      <h2 class="member-name">Paul S. Adler</h2>
      <div class="member-meta">
        <p>University of Southern California, USA</p>
        <a href="mailto:padler@marshall.usc.edu">padler@marshall.usc.edu</a>
        <p>Introduction</p>
      </div>
    </div>
  </div>

<div class="member-card">
    <div class="member-photo">
      <img src="assets/images/michigan.jpg" alt="michigan" />
    </div>
    <div class="member-info">
      <h2 class="member-name">Gerald F. Davis</h2>
      <div class="member-meta">
        <p>University of Michigan, USA</p>
        <a href="mailto:gfdavis@umich.edu">gfdavis@umich.edu</a>
        <p>Introduction</p>
      </div>
    </div>
  </div>

<div class="member-card">
    <div class="member-photo">
      <img src="assets/images/cityu.jpg" alt="cityu" />
    </div>
    <div class="member-info">
      <h2 class="member-name">Alfred Tat-Kei Ho</h2>
      <div class="member-meta">
        <p>City University of Hong Kong, Institute of Global Governance and Innovation for a Shared Future, Hong Kong</p>
        <a href="mailto:ho.tkalfred@cityu.edu.hk">ho.tkalfred@cityu.edu.hk</a>
        <p>Introduction</p>
      </div>
    </div>
  </div>

<div class="member-card">
    <div class="member-photo">
      <img src="assets/images/cityu.jpg" alt="cityu" />
    </div>
    <div class="member-info">
      <h2 class="member-name">Nicole Ning Liu</h2>
      <div class="member-meta">
        <p>City University of Hong Kong, Department of Public and International Affairs, Hong Kong</p>
        <a href="mailto:ning.liu@cityu.edu.hk">ning.liu@cityu.edu.hk</a>
        <p>Introduction</p>
      </div>
    </div>
  </div>
</section>








<style>
.member-section,
.member-section * {
  box-sizing: border-box;
}

.member-section {
  width: 100%;
  max-width: none;              /* 不受原容器宽度限制 */
  margin: 0 auto;
  padding: 0;

  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr)); /* 一排3个 */
  gap: 24px;

  /* 只让成员区突破父容器，不影响页面其他区域 */
  position: relative;
  left: 50%;
  transform: translateX(-50%);
  width: min(1400px, 96vw);     /* 可按需要调大，例如 1500px */
}

.member-card {
  display: flex;
  flex-direction: column;       /* 单个卡片内部改为上下结构，更适合网格 */
  align-items: stretch;
  gap: 16px;
  width: 100%;
  margin: 0;
  background: #ffffff;
  border-radius: 18px;
  padding: 16px 18px;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.08);
  overflow: hidden;
  min-width: 0;
}

.member-photo {
  width: 100%;
  max-width: none;
  flex: none;
}

.member-photo img {
  display: block;
  width: 100%;
  height: auto;
  aspect-ratio: 4 / 3;          /* 网格卡片里横向比例更自然 */
  object-fit: cover;
  border-radius: 14px;
}

.member-info {
  flex: 1;
  min-width: 0;
}

.member-name {
  margin: 0 0 12px;
  font-size: 20px;
  font-weight: 700;
  line-height: 1.4;
  color: #1f2a44;
}

.member-meta p {
  margin: 0 0 10px;
  font-size: 16px;
  line-height: 1.8;
  color: #4a5568;
  word-break: break-word;
}

.member-meta a {
  display: inline-block;
  margin: 0 0 10px;
  color: #2563eb;
  text-decoration: none;
  word-break: break-word;
}

.member-meta a:hover {
  text-decoration: underline;
}

/* 平板：2列 */
@media (max-width: 1024px) {
  .member-section {
    grid-template-columns: repeat(2, minmax(0, 1fr));
    width: min(1000px, 94vw);
  }
}

/* 手机：1列 */
@media (max-width: 768px) {
  .member-section {
    grid-template-columns: 1fr;
    width: min(100%, 92vw);
    left: auto;
    transform: none;
  }

  .member-card {
    padding: 14px;
  }

  .member-name,
  .member-meta {
    text-align: center;
  }
}
</style>