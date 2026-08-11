---
layout: default
permalink: /group/
---

# PhD Students

<div style="display: flex; flex-direction: row; gap: 60px; align-items: flex-start; flex-wrap: wrap; margin-bottom: 80px;">
  <div style="text-align: center;">
    <img src="{{ site.baseurl }}/assets/students/stephen.jpg" alt="Stephen Cheng" style="width: 150px; height: 150px; object-fit: cover; border-radius: 8px;">
    <p style="margin-top: 10px; margin-bottom: 5px; font-weight: bold;"><a href="https://step-cheng.github.io/" target="_blank" rel="noopener">Stephen Cheng</a></p>
    <p style="margin: 0; font-size: 0.9em; color: #666;">CS PhD (2025-)</p>
    <p style="margin: 0; font-size: 0.85em; color: #888;">Co-advised with Dinesh Manocha</p>
  </div>
  <div style="text-align: center;">
    <img src="{{ site.baseurl }}/assets/students/connor.jpg" alt="Connor Dilgren" style="width: 150px; height: 150px; object-fit: cover; border-radius: 8px;">
    <p style="margin-top: 10px; margin-bottom: 5px; font-weight: bold;"><a href="https://connordilgren.github.io/" target="_blank" rel="noopener">Connor Dilgren</a></p>
    <p style="margin: 0; font-size: 0.9em; color: #666;">CS PhD (2026-)</p>
    <p style="margin: 0; font-size: 0.85em; color: #888;"></p>
  </div>
  <div style="text-align: center;">
    <img src="{{ site.baseurl }}/assets/students/yiksiu.jpg" alt="Yik Siu Chan" style="width: 150px; height: 150px; object-fit: cover; border-radius: 8px;">
    <p style="margin-top: 10px; margin-bottom: 5px; font-weight: bold;"><a href="https://yiksiu-chan.github.io/" target="_blank" rel="noopener">Yik Siu Chan</a></p>
    <p style="margin: 0; font-size: 0.9em; color: #666;">CS PhD (2026-)</p>
    <p style="margin: 0; font-size: 0.85em; color: #888;">Co-advised with Hal Daumé III</p>
  </div>
</div>

# Group Photos

<div style="position: relative; width: 600px; margin: 0;">
  <div style="position: relative; width: 600px; height: auto;">
    <img id="carouselImg" src="{{ site.baseurl }}/assets/group/sp26_01.jpg" alt="Group photo" style="width: 600px; height: auto; border-radius: 8px; display: block;">
  </div>
  <button onclick="previousPhoto()" style="position: absolute; left: -60px; top: 50%; transform: translateY(-50%); background: none; border: none; font-size: 32px; cursor: pointer; color: #666;">❮</button>
  <button onclick="nextPhoto()" style="position: absolute; right: -60px; top: 50%; transform: translateY(-50%); background: none; border: none; font-size: 32px; cursor: pointer; color: #666;">❯</button>
  <p id="photoCounter" style="text-align: left; margin-top: 10px; font-size: 0.9em; color: #666;">1 of 3</p>
</div>

<script>
  const photos = [
    "{{ site.baseurl }}/assets/group/sp26_01.jpg",
    "{{ site.baseurl }}/assets/group/sp26_02.jpeg",
    "{{ site.baseurl }}/assets/group/sp26_03.jpg"
  ];
  let currentPhotoIndex = 0;

  function updatePhoto() {
    document.getElementById('carouselImg').src = photos[currentPhotoIndex];
    document.getElementById('photoCounter').textContent = (currentPhotoIndex + 1) + ' of ' + photos.length;
  }

  function nextPhoto() {
    currentPhotoIndex = (currentPhotoIndex + 1) % photos.length;
    updatePhoto();
  }

  function previousPhoto() {
    currentPhotoIndex = (currentPhotoIndex - 1 + photos.length) % photos.length;
    updatePhoto();
  }
</script>

# Alumni
**<a href="https://www.nishkal.xyz/" >Nishkal Hundia</a>**, B.S. 2026, CS & Math --> PhD student at Boston University