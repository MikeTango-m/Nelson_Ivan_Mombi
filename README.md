# 👩🏻‍💻 Nelson Ivan Mombi

**`Desenvolvedor`**

Me chamo Nelson Ivan Mombi, tenho 21 anos e sou natural de Maputo. Concluí o ensino médio no Colegio adventista da Liberdade, com o curso técnico em informática. Atualmente, estou cursando eng.informática no ISCTEM. Sou apaixonadO por tecnologia e sempre estou disposto a aprender o maximo que poder, estou a aprender a desenvolver projetos web, através do Instagram desenvolvo as minhas habilidades em Markting.

---

### 🤖 Linguagens e Tecnologias

<img 
    align="left" 
    alt="HTML"
    title="HTML" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" 
/>
<img 
    align="left" 
    alt="CSS" 
    title="CSS"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" 
/>
<img 
    align="left" 
    alt="JavaScript" 
    title="JavaScript"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" 
/>
<img 
    align="left" 
    alt="React"
    title="React" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/react/react-original.svg" 
/>
<img 
    align="left" 
    alt="Next.js" 
    title="Next.js"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nextjs/nextjs-original.svg" 
/>
<img 
    align="left" 
    alt="PHP" 
    title="PHP"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/php/php-original.svg" 
/>
<img 
    align="left" 
    alt="Python" 
    title="Python"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" 
/>

<br/>
<br/>

### 📊 Estatísticas

<p>
<img 
      align="left" 
      alt="GitHub Stats" 
      height="200" 
      src="https://github-readme-stats.vercel.app/api/top-langs/?username=larissakich&theme=tokyonight&layout=compact&custom_title=Tecnologias&langs_count=9" 
  />

  <img 
  alt="GitHub Stats" 
  height="200" 
  src="https://github-readme-stats.vercel.app/api?username=NelsonIvanMombi&show_icons=true&theme=tokyonight" 
/>




<!DOCTYPE html>
<html lang="pt">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Estatísticas GitHub</title>
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
</head>
<body style="background:#0d1117; color:white; font-family:Arial; text-align:center;">

  <h1>Estatísticas do meu GitHub 🚀</h1>
  <canvas id="linguagensChart" width="400" height="200"></canvas>

  <script>
    async function carregarLinguagens() {
      const username = "NelsonIvanMombi";
      const repos = await fetch(`https://api.github.com/users/${username}/repos`);
      const reposData = await repos.json();

      let linguagens = {};

      for (let repo of reposData) {
        if (repo.language) {
          linguagens[repo.language] = (linguagens[repo.language] || 0) + 1;
        }
      }

      const ctx = document.getElementById("linguagensChart").getContext("2d");
      new Chart(ctx, {
        type: "pie",
        data: {
          labels: Object.keys(linguagens),
          datasets: [{
            label: "Linguagens mais usadas",
            data: Object.values(linguagens),
            backgroundColor: ["#f87171","#60a5fa","#34d399","#fbbf24","#a78bfa","#f472b6"]
          }]
        }
      });
    }

    carregarLinguagens();
  </script>

</body>
</html>


</p>
