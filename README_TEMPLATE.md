<style>
  .container {
    max-width: 420px;
    margin: 10px auto;
    background: linear-gradient(135deg, #e6f0ff, #b3d1ff, #80b3ff); /* Degradê azul evidente */
    border: 4px solid #0044cc; /* Borda mais grossa e destacada */
    border-radius: 12px;
    padding: 25px 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    color: #1c1e21;
    box-shadow: 0 6px 18px rgba(0,0,0,0.1);
  }

  .table {
    width: 100%;
    border-collapse: collapse;
    text-align: center;
  }

  .table th {
    font-size: 14px;
    color: #003366;
    padding: 15px 10px;
    background-color: rgba(255,255,255,0.3);
    border-bottom: 2px solid #0044cc;
  }

  .table td {
    font-size: 14px;
    color: #003366;
    padding: 20px 10px;
    vertical-align: middle;
  }

  .table img {
    height: 40px;
  }

  .header {
    text-align: center;
    margin-bottom: 10px;
    font-size: 22px;
  }

  .loading {
    text-align: center;
    color: #0044cc;
    font-style: italic;
  }

  .number {
    font-size: 24px;
    font-weight: bold;
    color: #0044cc;
    margin-bottom: 10px;
    min-height: 30px;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
  }

  .loading {
    font-size: 14px;
    color: #666;
    font-style: italic;
    animation: loadingDots 1.5s infinite;
  }

  @keyframes loadingDots {
    0%, 20% { content: ''; }
    40% { content: '.'; }
    60% { content: '..'; }
    80%, 100% { content: '...'; }
  }

  .loading::after {
    content: '';
    animation: loadingDots 1.5s infinite;
  }
</style>

<h1 class="header">Esses são dados da minha conta profissional</h1>
<div class="container">
  <div style="text-align: center; margin-bottom: 20px;">
    <a href="https://github.com/romulosuperlogica" target="_blank" style="text-decoration: none; color: inherit;">
      <h2 style="margin: 0; font-size: 22px; color: #003366;">@romulosuperlogica</h2>
      <p style="margin: 5px 0 0; font-size: 14px; color: #003366;">
        Desenvolvedor | GitHub | Contribuições Profissionais
      </p>
    </a>
  </div>

     <p style="text-align: center; font-size: 12px; color: #003366; margin: 0 0 10px 0; font-style: italic;">Last year data</p>
     <table class="table">
       <thead>
         <tr>
           <th>Commits</th>
           <th>Pull Requests Opened</th>
           <th>Pull Requests Reviewed</th>
         </tr>
       </thead>
       <tbody>
         <tr>
           <td>
             <div style="display: flex; flex-direction: column; align-items: center; gap: 10px;">
               <div class="number" id="commits"><span class="loading">...</span></div>
             </div>
           </td>
           <td>
             <div style="display: flex; flex-direction: column; align-items: center; gap: 10px;">
               <div class="number" id="prs-opened"><span class="loading">...</span></div>
             </div>
           </td>
           <td>
             <div style="display: flex; flex-direction: column; align-items: center; gap: 10px;">
               <div class="number" id="prs-reviewed"><span class="loading">...</span></div>
             </div>
           </td>
         </tr>
       </tbody>
     </table>

  <p style="text-align: center; font-size: 13px; margin: 0; color: #002244;">
    Acesse meu perfil completo:
    <a 
      href="https://github.com/romulosuperlogica" 
      style="color: #0044cc; text-decoration: none; font-weight: 600;" 
      target="_blank"
    >
      github.com/romulosuperlogica
    </a>
  </p>
</div>
