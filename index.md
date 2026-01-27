---
layout: default
---

<style>
  /* Responsive grid layout */
  .content-grid {
    display: grid;
    grid-template-columns: 1fr 3fr;
    gap: 2rem;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 1.5rem;
  }

  @media (max-width: 768px) {
    .content-grid {
      grid-template-columns: 1fr;
    }
  }

  /* Sidebar styling */
  .sidebar {
    position: sticky;
    top: 2rem;
    max-width: 300px;
  }

  .name-header {
    text-align: center;
    margin-bottom: 1rem;
    font-size: 1.8rem;
    font-weight: 600;
    color: #2c3e50;
  }

  .avatar-container {
    text-align: center;
    margin-bottom: 1.5rem;
  }

  .avatar {
    width: 100%;
    max-width: 250px;
    border-radius: 50%;
    border: 3px solid #eee;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    transition: transform 0.3s ease;
  }

  .avatar:hover {
    transform: scale(1.05);
  }

  .position {
    text-align: center;
    font-style: italic;
    color: #555;
    margin-bottom: 1.5rem;
    line-height: 1.4;
  }

  .github-link {
    display: block;
    text-align: center;
    margin-bottom: 1.5rem;
    color: #007bff;
    text-decoration: none;
    font-weight: 500;
  }

  .github-link:hover {
    text-decoration: underline;
  }

  /* Main content */
  .main-content {
    line-height: 1.6;
  }

  /* Timeline image container */
  .timeline-container {
    position: relative;
    margin: 1.5rem 0;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 4px 12px rgba(0,0,0,0.08);
  }

  .timeline-container a {
    display: block;
    width: 100%;
  }

  .timeline-container img {
    width: 100%;
    height: auto;
    display: block;
    transition: transform 0.3s ease;
  }

  .timeline-container a:hover img {
    transform: scale(1.03);
  }

  .timeline-caption {
    text-align: center;
    font-size: 0.9rem;
    color: #666;
    margin-top: 0.5rem;
    font-style: italic;
  }

  /* Custom list markers */
  .research-list {
    padding-left: 1.5rem;
    margin: 1rem 0;
  }

  .research-list li {
    margin-bottom: 0.7rem;
    position: relative;
  }

  .research-list li:before {
    content: "■";
    color: #007bff;
    font-weight: bold;
    position: absolute;
    left: -1.2rem;
    width: 1rem;
  }

  /* Profile links */
  .profile-links {
    display: flex;
    flex-wrap: wrap;
    gap: 0.8rem;
    margin: 1.5rem 0;
  }

  .profile-links a {
    padding: 0.4rem 0.8rem;
    background: #f8f9fa;
    border-radius: 4px;
    text-decoration: none;
    color: #007bff;
    transition: all 0.2s;
  }

  .profile-links a:hover {
    background: #e9ecef;
    transform: translateY(-2px);
  }

  .last-updated {
    text-align: center;
    margin-top: 2rem;
    padding-top: 1rem;
    border-top: 1px solid #eee;
    color: #666;
    font-size: 0.9rem;
  }

  /* Lightbox modal for timeline image */
  .lightbox-modal {
    display: none;
    position: fixed;
    z-index: 1000;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0,0,0,0.9);
    cursor: pointer;
  }

  .lightbox-modal.active {
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .lightbox-image {
    max-width: 90%;
    max-height: 90%;
    object-fit: contain;
    border: 3px solid white;
    box-shadow: 0 0 30px rgba(255,255,255,0.5);
  }

  .lightbox-close {
    position: absolute;
    top: 20px;
    right: 30px;
    color: white;
    font-size: 40px;
    font-weight: bold;
    cursor: pointer;
    user-select: none;
  }

  .lightbox-close:hover {
    color: #ccc;
  }
</style>

<div class="content-grid">
  <div class="sidebar">
    <h1 class="name-header">Ilya M. Afanasyev, Ph.D.</h1>
    <div class="avatar-container">
      <img src="avatar.jpg" alt="Ilya Afanasyev" class="avatar">
    </div>
    <p class="position">Expert at Chebyshev Research Center (Huawei) &<br>Adjunct Associate Professor</p>
    <a href="#" class="github-link">View My GitHub Profile</a>
    
    <div class="profile-links">
      <a href="https://scholar.google.ru/citations?user=Ogv_bdYAAAAJ" target="_blank">Google Scholar</a>
      <a href="https://www.researchgate.net/profile/Ilya-Afanasyev-3" target="_blank">ResearchGate</a>
      <a href="https://ru.linkedin.com/in/ilya-afanasyev-8783291a" target="_blank">LinkedIn</a>
      <a href="mailto:ilya.afanasyev@gmail.com">Email</a>
    </div>
  </div>

  <div class="main-content">
    <h1>About Me</h1>
    
    <p><strong>Ilya M. Afanasyev, Ph.D.</strong>, is an Expert at the <strong>Chebyshev Research Center (Huawei)</strong> and an Adjunct Associate Professor at <strong>Innopolis University</strong> and <strong>Saint Petersburg Electrotechnical University "LETI"</strong>. He earned his Ph.D. in Optical and Optoelectronical Devices from Vavilov State Optical Institute (2006).</p>
    
    <p>With over two decades of R&D experience, Dr. Afanasyev has worked in industry (Huawei, TGT, Giesecke & Devrient) and held academic positions at various institutions including the University of Trento, Innopolis University, KFU, ITMO, and SPbPU. He specializes in <strong>Autonomous Systems, Sensors, Computer Vision, and Mobile Robotics</strong>.</p>
    
    <p>He is a <strong>Marie Curie Fellow alumnus</strong>, holder of 2 patents, and author of 50+ publications indexed in Scopus/WoS.</p>

    <h2>📅 Experience Timeline</h2>
    
    <div class="timeline-container" onclick="openLightbox()">
      <img src="timeline.png" alt="Career Timeline (2000-2025)">
      <div class="timeline-caption">Visual overview of my academic and industrial career path (2000–2025). Click image to enlarge.</div>
    </div>

    <h2>🔬 Research Interests</h2>
    
    <ul class="research-list">
      <li><strong>Mobile Robotics:</strong> SLAM, Navigation, Path Planning</li>
      <li><strong>Computer Vision:</strong> Object Detection, Tracking, Camera Calibration</li>
      <li><strong>Sensors:</strong> Sensor Fusion, Optical Sensors, IMU</li>
      <li><strong>Intelligent Systems:</strong> UAV, Intelligent Transportation Systems (ITS)</li>
    </ul>

    <h2>📚 Selected Publications & Patents</h2>
    
    <p>Here are a few highlights. For the full list, please visit my <a href="https://scholar.google.ru/citations?user=Ogv_bdYAAAAJ" target="_blank">Google Scholar Profile</a>.</p>
    
    <p><strong>Most Cited (SLAM Benchmarking)</strong><br>
    1. <strong>Comparison of Various SLAM Systems for Mobile Robot in an Indoor Environment.</strong><br>
    M. Filipenko, I. Afanasyev.<br>
    <em>9th IEEE International Conference on Intelligent Systems (IS)</em>, 2018.<br>
    [Cited by ~250+] <a href="https://doi.org/10.1109/IS.2018.8710464" target="_blank">DOI</a></p>
    
    <p><strong>Lidar SLAM & Ground Truth Analysis</strong><br>
    2. <strong>Map Comparison of Lidar-based 2D SLAM Algorithms Using Precise Ground Truth.</strong><br>
    R. Yagfarov, M. Ivanou, I. Afanasyev.<br>
    <em>International Conference on Control, Automation, Robotics and Vision (ICARCV)</em>, Singapore, 2018.<br>
    [Cited by ~130+] <a href="https://doi.org/10.1109/ICARCV.2018.8581131" target="_blank">DOI</a></p>
    
    <p><strong>Top Journal (UAV Efficiency)</strong><br>
    3. <strong>Game Theory-based Parameter Tuning for Energy-efficient Path Planning on Modern UAVs.</strong><br>
    D. Moolchandani, I. Afanasyev, et al.<br>
    <em>ACM Transactions on Cyber-Physical Systems</em>, Vol. 6(4), 2022.<br>
    <a href="https://doi.org/10.1145/3565270" target="_blank">DOI</a></p>
    
    <p><strong>Intelligent Systems & IoT</strong><br>
    4. <strong>Towards the Internet of Robotic Things: Analysis, Architecture, Components and Challenges.</strong><br>
    I. Afanasyev, et al.<br>
    <em>12th International Conference on Developments in eSystems Engineering (DeSE)</em>, 2019.<br>
    [Cited by ~80] <a href="https://arxiv.org/abs/1907.03817" target="_blank">arXiv</a></p>
    
    <p><strong>Patents (Hardware & UAV)</strong><br>
    5. <strong>Modular multi-rotor unmanned aerial vehicle of vertical take-off and landing.</strong><br>
    M. Galimov, I. Afanasyev, et al.<br>
    <em>Patent RU 2706765</em>, 2019.<br>
    <a href="https://patents.google.com/patent/RU2706765C1/en" target="_blank">Google Patents</a></p>

    <h2>🎓 Teaching (Highlights)</h2>
    
    <ul class="research-list">
      <li><strong>Advanced Robotics</strong> (Master's level) – Innopolis University (2025-2026)</li>
      <li><strong>Optoelectronic Detecting Technology</strong> – ITMO & CUST (China), Changchun, China, 2025</li>
      <li><strong>Foundation of Robotics & Computer Vision with OpenCV</strong> – Kazan Federal University, 2021-2022</li>
      <li><strong>Sensors & Sensing</strong> – Innopolis University (2018-2020), SPbPU (2021)</li>
      <li><strong>Intelligent Mobile Robotics</strong> – Innopolis University (2016-2020)</li>
      <li><strong>Control Theory</strong> – Innopolis University (2016-2019)</li>
    </ul>

    <div class="last-updated">
      <small>Last updated: January 2025</small>
    </div>
  </div>
</div>

<!-- Lightbox modal for timeline image -->
<div id="lightbox" class="lightbox-modal">
  <span class="lightbox-close" onclick="closeLightbox(event)">&times;</span>
  <img class="lightbox-image" src="timeline.png" alt="Career Timeline (2000-2025)">
</div>

<script>
  function openLightbox() {
    document.getElementById('lightbox').classList.add('active');
    document.body.style.overflow = 'hidden';
  }

  function closeLightbox(event) {
    event.stopPropagation();
    document.getElementById('lightbox').classList.remove('active');
    document.body.style.overflow = 'auto';
  }

  document.getElementById('lightbox').addEventListener('click', function(event) {
    if (event.target === this) {
      closeLightbox(event);
    }
  });

  document.addEventListener('keydown', function(event) {
    if (event.key === 'Escape') {
      document.getElementById('lightbox').classList.remove('active');
      document.body.style.overflow = 'auto';
    }
  });
</script>
