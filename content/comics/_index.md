---
title: "Food system comics"
---

With the undergraduates in ENVS 323: Sustainable Food Systems and illustrator [Maris Wicks](https://www.mariswicks.com/), we made *That's Bananas! A Comics Food History of Banana Bread*. More food comics are on the way.

<div class="comic-reader" id="comic">
<div class="comic-nav" hidden>
<button type="button" class="btn btn-wheat" data-step="-1">← Previous</button>
<span class="comic-count" aria-live="polite"></span>
<button type="button" class="btn btn-wheat" data-step="1">Next →</button>
</div>
<div class="comic">
<img src="/comics/pages/page-01.jpg" alt="Cover of That's Bananas! A Comics Food History of Banana Bread" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-02.jpg" alt="That's Bananas!, page 2" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-03.jpg" alt="That's Bananas!, page 3" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-04.jpg" alt="That's Bananas!, page 4" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-05.jpg" alt="That's Bananas!, page 5" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-06.jpg" alt="That's Bananas!, page 6" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-07.jpg" alt="That's Bananas!, page 7" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-08.jpg" alt="That's Bananas!, page 8" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-09.jpg" alt="That's Bananas!, page 9" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-10.jpg" alt="That's Bananas!, page 10" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-11.jpg" alt="That's Bananas!, page 11" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-12.jpg" alt="That's Bananas!, page 12" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-13.jpg" alt="That's Bananas!, page 13" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-14.jpg" alt="That's Bananas!, page 14" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-15.jpg" alt="That's Bananas!, page 15" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-16.jpg" alt="That's Bananas!, page 16" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-17.jpg" alt="That's Bananas!, page 17" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-18.jpg" alt="That's Bananas!, page 18" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-19.jpg" alt="That's Bananas!, page 19" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-20.jpg" alt="That's Bananas!, page 20" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-21.jpg" alt="That's Bananas!, page 21" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-22.jpg" alt="That's Bananas!, page 22" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-23.jpg" alt="That's Bananas!, page 23" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-24.jpg" alt="That's Bananas!, page 24" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-25.jpg" alt="That's Bananas!, page 25" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-26.jpg" alt="That's Bananas!, page 26" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-27.jpg" alt="That's Bananas!, page 27" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-28.jpg" alt="That's Bananas!, page 28" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-29.jpg" alt="That's Bananas!, page 29" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-30.jpg" alt="That's Bananas!, page 30" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-31.jpg" alt="That's Bananas!, page 31" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-32.jpg" alt="That's Bananas!, page 32" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-33.jpg" alt="That's Bananas!, page 33" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-34.jpg" alt="That's Bananas!, page 34" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-35.jpg" alt="That's Bananas!, page 35" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-36.jpg" alt="That's Bananas!, page 36" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-37.jpg" alt="That's Bananas!, page 37" width="850" height="1100" loading="lazy">
<img src="/comics/pages/page-38.jpg" alt="That's Bananas!, page 38" width="850" height="1100" loading="lazy">
</div>
<div class="comic-nav" hidden>
<button type="button" class="btn btn-wheat" data-step="-1">← Previous</button>
<span class="comic-count" aria-live="polite"></span>
<button type="button" class="btn btn-wheat" data-step="1">Next →</button>
</div>
</div>

<script>
(function () {
  var r = document.getElementById("comic"); if (!r) return;
  var pages = r.querySelectorAll(".comic img"), n = pages.length, i = 0;
  var counts = r.querySelectorAll(".comic-count"), navs = r.querySelectorAll(".comic-nav");
  r.classList.add("paged"); navs.forEach(function (x) { x.hidden = false; });
  function show(k, scroll) {
    i = Math.max(0, Math.min(n - 1, k));
    pages.forEach(function (p, j) { p.classList.toggle("on", j === i); });
    if (pages[i + 1]) pages[i + 1].loading = "eager";
    counts.forEach(function (c) { c.textContent = "Page " + (i + 1) + " of " + n; });
    r.querySelectorAll('[data-step="-1"]').forEach(function (b) { b.disabled = i === 0; });
    r.querySelectorAll('[data-step="1"]').forEach(function (b) { b.disabled = i === n - 1; });
    if (scroll && r.getBoundingClientRect().top < 0) r.scrollIntoView({ block: "start" });
  }
  r.addEventListener("click", function (e) {
    var b = e.target.closest("[data-step]");
    if (b) { show(i + Number(b.dataset.step), b.parentNode === navs[1]); return; }
    if (e.target.tagName === "IMG") {
      var box = e.target.getBoundingClientRect();
      show(i + (e.clientX - box.left > box.width / 2 ? 1 : -1), false);
    }
  });
  document.addEventListener("keydown", function (e) {
    if (e.key === "ArrowRight") show(i + 1, false);
    if (e.key === "ArrowLeft") show(i - 1, false);
  });
  var x0 = null;
  r.addEventListener("touchstart", function (e) { x0 = e.touches[0].clientX; }, { passive: true });
  r.addEventListener("touchend", function (e) {
    if (x0 === null) return; var dx = e.changedTouches[0].clientX - x0; x0 = null;
    if (Math.abs(dx) > 50) show(i + (dx < 0 ? 1 : -1), false);
  });
  show(0, false);
})();
</script>

<p><a href="/comics/TB.pdf">Download the comic (PDF, 23 MB)</a></p>
