# 🗓️ Planejamento Semanal – Cidade da Criança

<section class="cc-week-plan">

<style>
  :root {
    --cc-azul: #0286B4;
    --cc-fundo: #23B4B6;
    --cc-amarelo: #FAAE39;
    --cc-laranja: #FB5E1C;
    --cc-verde: #00ABB2;
    --cc-vermelho: #FB454C;
  }

  .cc-week-plan {
    font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    margin: 0 auto 2rem;
    max-width: 1080px;
  }

  .cc-week-header {
    background: linear-gradient(90deg, var(--cc-amarelo), var(--cc-laranja));
    color: #1F2933;
    padding: 1rem 1.5rem;
    border-radius: 16px;
    margin-bottom: 1.5rem;
    box-shadow: 0 10px 24px rgba(0,0,0,0.12);
  }

  .cc-week-header h2 {
    margin: 0;
    font-size: 1.4rem;
  }

  .cc-week-header p {
    margin: .25rem 0 0;
    font-size: .9rem;
  }

  /* Tudo em coluna única */
  .cc-week-grid {
    display: flex;
    flex-direction: column;
    gap: 1.2rem;
  }

  .cc-day-card {
    background: #FFFFFF;
    border-radius: 14px;
    padding: 1rem 1.1rem 1.2rem;
    box-shadow: 0 8px 20px rgba(0,0,0,0.08);

    /* Borda em volta de cada dia */
    border: 2px solid rgba(2, 134, 180, 0.4);
  }

  .cc-day-header {
    display: flex;
    align-items: baseline;
    justify-content: space-between;
    gap: .75rem;
    margin-bottom: .5rem;
  }

  .cc-day-name {
    font-weight: 700;
    font-size: 1.1rem;
    color: #111827;
  }

  .cc-badge {
    background: var(--cc-verde);
    color: #FFFFFF;
    border-radius: 999px;
    padding: .15rem .7rem;
    font-size: .75rem;
    text-transform: uppercase;
    letter-spacing: .03em;
  }

  .cc-field-label {
    font-size: .85rem;
    font-weight: 600;
    color: #4B5563;
    margin-bottom: .15rem;
  }

  /* Data e Tema com “pills” coloridas */
  .cc-field-label--data,
  .cc-field-label--tema {
    display: inline-flex;
    align-items: center;
    gap: .4rem;
    padding: .1rem .55rem;
    border-radius: 999px;
    font-size: .8rem;
    color: #FFFFFF;
    margin-bottom: .2rem;
  }

  .cc-field-label--data {
    background: var(--cc-azul);
  }

  .cc-field-label--tema {
    background: var(--cc-verde);
  }

  .cc-field-label--data::before,
  .cc-field-label--tema::before {
    content: "•";
    font-size: 1rem;
  }

  .cc-line-input {
    display: block;
    width: 100%;
    border-bottom: 1px dashed #CBD5E1;
    padding-bottom: .25rem;
    margin-bottom: .45rem;
    font-size: .88rem;
    color: #111827;
  }

  .cc-line-input--multiline {
    min-height: 3.2rem;
  }

  .cc-subtitle {
    font-size: .8rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: .06em;
    color: #6B7280;
    margin-bottom: .3rem;
  }

  /* Turnos com cores diferentes */
  .cc-session {
    margin-top: .4rem;
    padding: .6rem .75rem .65rem;
    border-radius: 10px;
    border: 1px dashed #E5E7EB;
  }

  .cc-session--manha {
    background: rgba(250, 174, 57, 0.08);  /* amarelo suave */
    border-left: 4px solid var(--cc-amarelo);
  }

  .cc-session--tarde {
    background: rgba(251, 94, 28, 0.08);   /* laranja suave */
    border-left: 4px solid var(--cc-laranja);
  }

  .cc-school-row {
    font-size: .84rem;
    margin-top: .4rem;
  }

  .cc-school-row strong {
    color: #111827;
  }

  .cc-school-meta {
    font-size: .8rem;
    color: #4B5563;
    margin-top: .15rem;
  }

  .cc-school-checks span {
    display: inline-block;
    margin-right: .4rem;
    padding: .05rem .4rem;
    border-radius: 999px;
    border: 1px solid #CBD5E1;
    font-size: .72rem;
  }

  /* Lista de anotações com bullets e espaço pra escrever */
  .cc-notes-label {
    font-size: .8rem;
    font-weight: 600;
    color: #4B5563;
    margin-top: .2rem;
  }

  .cc-notes-list {
    list-style: none;
    padding-left: 0;
    margin: .2rem 0 .1rem;
  }

  .cc-notes-list li {
    position: relative;
    padding-left: 1rem;
    margin-bottom: .15rem;
  }

  .cc-notes-list li::before {
    content: "•";
    position: absolute;
    left: 0;
    top: 0;
    color: #9CA3AF;
  }

  .cc-note-line {
    border-bottom: 1px dashed #E5E7EB;
    padding-bottom: .2rem;
    min-height: 1.1rem;
  }

  @media print {
    .cc-week-header {
      box-shadow: none;
      border: 1px solid #E5E7EB;
    }
    .cc-day-card {
      box-shadow: none;
    }
  }
</style>

<div class="cc-week-header">
  <h2>Planejamento Semanal – Exemplo de Página</h2>
  <p>Organize visitas, temas e anotações para cada dia da semana na Cidade da Criança.</p>
</div>

<div class="cc-week-grid">

  <!-- Segunda-feira -->
  <article class="cc-day-card">
    <div class="cc-day-header">
      <div class="cc-day-name">Segunda-feira</div>
      <span class="cc-badge">Planejamento</span>
    </div>

    <div>
      <div class="cc-field-label cc-field-label--data">Data</div>
      <div class="cc-line-input"></div>
    </div>

    <div>
      <div class="cc-field-label">Anotações gerais</div>
      <div class="cc-line-input cc-line-input--multiline"></div>
      <div class="cc-line-input cc-line-input--multiline"></div>
    </div>
  </article>

  <!-- Terça-feira -->
  <article class="cc-day-card">
    <div class="cc-day-header">
      <div class="cc-day-name">Terça-feira</div>
      <span class="cc-badge">Visitas</span>
    </div>

    <div>
      <div class="cc-field-label cc-field-label--data">Data</div>
      <div class="cc-line-input"></div>
    </div>

    <div>
      <div class="cc-field-label cc-field-label--tema">Tema / foco pedagógico do dia</div>
      <div class="cc-line-input"></div>
    </div>

    <div class="cc-session cc-session--manha">
      <div class="cc-subtitle">Manhã</div>

      <div class="cc-school-row">
        <strong>Escola 1</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>

      <div class="cc-school-row">
        <strong>Escola 2</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>
    </div>

    <div class="cc-session cc-session--tarde">
      <div class="cc-subtitle">Tarde</div>

      <div class="cc-school-row">
        <strong>Escola 1</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>

      <div class="cc-school-row">
        <strong>Escola 2</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>
    </div>
  </article>

  <!-- Quarta-feira -->
  <article class="cc-day-card">
    <div class="cc-day-header">
      <div class="cc-day-name">Quarta-feira</div>
      <span class="cc-badge">Visitas</span>
    </div>

    <div>
      <div class="cc-field-label cc-field-label--data">Data</div>
      <div class="cc-line-input"></div>
    </div>

    <div>
      <div class="cc-field-label cc-field-label--tema">Tema / foco pedagógico do dia</div>
      <div class="cc-line-input"></div>
    </div>

    <div class="cc-session cc-session--manha">
      <div class="cc-subtitle">Manhã</div>

      <div class="cc-school-row">
        <strong>Escola 1</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>

      <div class="cc-school-row">
        <strong>Escola 2</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>
    </div>

    <div class="cc-session cc-session--tarde">
      <div class="cc-subtitle">Tarde</div>

      <div class="cc-school-row">
        <strong>Escola 1</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>

      <div class="cc-school-row">
        <strong>Escola 2</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>
    </div>
  </article>

  <!-- Quinta-feira -->
  <article class="cc-day-card">
    <div class="cc-day-header">
      <div class="cc-day-name">Quinta-feira</div>
      <span class="cc-badge">Visitas</span>
    </div>

    <div>
      <div class="cc-field-label cc-field-label--data">Data</div>
      <div class="cc-line-input"></div>
    </div>

    <div>
      <div class="cc-field-label cc-field-label--tema">Tema / foco pedagógico do dia</div>
      <div class="cc-line-input"></div>
    </div>

    <div class="cc-session cc-session--manha">
      <div class="cc-subtitle">Manhã</div>

      <div class="cc-school-row">
        <strong>Escola 1</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>

      <div class="cc-school-row">
        <strong>Escola 2</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>
    </div>

    <div class="cc-session cc-session--tarde">
      <div class="cc-subtitle">Tarde</div>

      <div class="cc-school-row">
        <strong>Escola 1</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>

      <div class="cc-school-row">
        <strong>Escola 2</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>
    </div>
  </article>

  <!-- Sexta-feira -->
  <article class="cc-day-card">
    <div class="cc-day-header">
      <div class="cc-day-name">Sexta-feira</div>
      <span class="cc-badge">Visitas</span>
    </div>

    <div>
      <div class="cc-field-label cc-field-label--data">Data</div>
      <div class="cc-line-input"></div>
    </div>

    <div>
      <div class="cc-field-label cc-field-label--tema">Tema / foco pedagógico do dia</div>
      <div class="cc-line-input"></div>
    </div>

    <div class="cc-session cc-session--manha">
      <div class="cc-subtitle">Manhã</div>

      <div class="cc-school-row">
        <strong>Escola 1</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>

      <div class="cc-school-row">
        <strong>Escola 2</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>
    </div>

    <div class="cc-session cc-session--tarde">
      <div class="cc-subtitle">Tarde</div>

      <div class="cc-school-row">
        <strong>Escola 1</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>

      <div class="cc-school-row">
        <strong>Escola 2</strong>
        <div class="cc-field-label">Nome da instituição</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Quantidade de alunos</div>
        <div class="cc-line-input"></div>

        <div class="cc-field-label">Tipo de instituição</div>
        <div class="cc-school-meta cc-school-checks">
          <span>( ) Pública</span><span>( ) Particular</span><span>( ) Instituto</span>
        </div>

        <div class="cc-notes-label">Anotações</div>
        <ul class="cc-notes-list">
          <li><div class="cc-note-line"></div></li>
          <li><div class="cc-note-line"></div></li>
        </ul>
      </div>
    </div>
  </article>

  <!-- Sábado / Domingo -->
  <article class="cc-day-card">
    <div class="cc-day-header">
      <div class="cc-day-name">Sábado / Domingo</div>
      <span class="cc-badge">Eventos / Notas</span>
    </div>

    <div>
      <div class="cc-field-label cc-field-label--data">Data</div>
      <div class="cc-line-input"></div>
    </div>

    <div>
      <div class="cc-field-label">Anotações gerais</div>
      <div class="cc-line-input cc-line-input--multiline"></div>
      <div class="cc-line-input cc-line-input--multiline"></div>
    </div>
  </article>

</div> <!-- fim .cc-week-grid -->

</section>
