# the-goat-sir-made-this-with-the-sir-family.github.com
<div id="x_"></div>

<script>
(function () {

  const container = document.getElementById("x_");

  container.innerHTML = `
    <div style="font-family:Inter,Arial,sans-serif;text-align:center;padding:20px;background:#111;color:#eee;border-radius:12px;max-width:420px;margin:auto;">
      <h2 style="font-weight:600;">Launch Keo</h2>
      <p>How do you want to launch Keo? <span style="opacity:.7">(cloak recommended)</span></p>
      <button id="c_" style="all:unset;cursor:pointer;background:#222;padding:10px 18px;border-radius:10px;margin:6px;transition:.2s">Cloaked</button>
      <button id="n_" style="all:unset;cursor:pointer;background:#333;padding:10px 18px;border-radius:10px;margin:6px;transition:.2s">Normal</button>
    </div>
  `;

  const url = "https://keoffical.vercel.app/";

  // cloaked (about:blank iframe)
  document.getElementById("c_").onclick = function () {
    const w = window.open("about:blank", "_blank");
    if (!w) return;

    w.document.body.style.margin = "0";
    w.document.body.innerHTML = `
      <iframe 
        src="${url}" 
        style="position:fixed;top:0;left:0;width:100%;height:100%;border:none;">
      </iframe>
    `;
  };

  // normal
  document.getElementById("n_").onclick = function () {
    window.open(url, "_blank");
  };

})();
</script>
