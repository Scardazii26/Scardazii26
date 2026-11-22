<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 180" width="1000" height="180" role="img" aria-label="Logistics and operations animation">
  <defs>
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0" stop-color="#0A1AFF"/>
      <stop offset="1" stop-color="#00E5FF"/>
    </linearGradient>
  </defs>

  <!-- Fundo -->
  <rect width="1000" height="180" fill="url(#bg)"/>

  <!-- Rota tracejada animada -->
  <path d="M60 85 C 200 40, 350 110, 500 70 S 800 40, 940 80"
        fill="none" stroke="#fff" stroke-opacity="0.55" stroke-width="2.5" stroke-dasharray="6 8">
    <animate attributeName="stroke-dashoffset" from="0" to="-56" dur="2s" repeatCount="indefinite"/>
  </path>

  <!-- Pontos de rastreio pulsando -->
  <g fill="#fff">
    <circle cx="60" cy="85" r="4"/>
    <circle cx="500" cy="70" r="4"/>
    <circle cx="940" cy="80" r="4"/>
  </g>
  <g fill="none" stroke="#fff" stroke-width="2">
    <circle cx="60" cy="85" r="5">
      <animate attributeName="r" from="5" to="16" dur="2s" repeatCount="indefinite"/>
      <animate attributeName="opacity" from="0.8" to="0" dur="2s" repeatCount="indefinite"/>
    </circle>
    <circle cx="500" cy="70" r="5">
      <animate attributeName="r" from="5" to="16" dur="2s" begin="0.6s" repeatCount="indefinite"/>
      <animate attributeName="opacity" from="0.8" to="0" dur="2s" begin="0.6s" repeatCount="indefinite"/>
    </circle>
    <circle cx="940" cy="80" r="5">
      <animate attributeName="r" from="5" to="16" dur="2s" begin="1.2s" repeatCount="indefinite"/>
      <animate attributeName="opacity" from="0.8" to="0" dur="2s" begin="1.2s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- Avião cargueiro -->
  <g transform="translate(0,28)">
    <g>
      <animateTransform attributeName="transform" type="translate" from="-80 0" to="1080 0" dur="18s" repeatCount="indefinite"/>
      <polygon points="-24,-2 -32,-14 -26,-14 -14,-2" fill="#fff"/>
      <ellipse cx="0" cy="0" rx="28" ry="5" fill="#fff"/>
      <polygon points="-4,0 -14,14 -6,14 8,0" fill="#fff" fill-opacity="0.85"/>
    </g>
  </g>

  <!-- Galpão (esquerda) -->
  <g fill="#0b1030" fill-opacity="0.55">
    <rect x="40" y="108" width="130" height="32"/>
    <polygon points="34,108 105,92 176,108"/>
  </g>
  <g fill="#fff" fill-opacity="0.35">
    <rect x="52" y="120" width="26" height="20"/>
    <rect x="92" y="120" width="26" height="20"/>
    <rect x="132" y="120" width="26" height="20"/>
  </g>

  <!-- Contêineres (direita) -->
  <g fill-opacity="0.55">
    <rect x="850" y="124" width="46" height="16" fill="#0b1030"/>
    <rect x="900" y="124" width="46" height="16" fill="#fff"/>
    <rect x="875" y="107" width="46" height="16" fill="#fff"/>
    <rect x="925" y="107" width="46" height="16" fill="#0b1030"/>
  </g>

  <!-- Estrada -->
  <rect y="140" width="1000" height="40" fill="#0b1030" fill-opacity="0.85"/>
  <line x1="0" y1="162" x2="1000" y2="162" stroke="#fff" stroke-width="3" stroke-dasharray="30 24">
    <animate attributeName="stroke-dashoffset" from="0" to="-54" dur="0.8s" repeatCount="indefinite"/>
  </line>

  <!-- Caminhão -->
  <g transform="translate(0,148)">
    <g>
      <animateTransform attributeName="transform" type="translate" from="-170 0" to="1050 0" dur="14s" repeatCount="indefinite"/>
      <!-- Baú -->
      <rect x="0" y="-34" width="84" height="34" rx="3" fill="#fff"/>
      <rect x="0" y="-18" width="84" height="5" fill="#00E5FF"/>
      <!-- Cabine -->
      <path d="M86 -26 h20 l12 12 v14 h-32 z" fill="#00E5FF"/>
      <path d="M92 -21 h12 l8 8 h-20 z" fill="#0b1030" fill-opacity="0.7"/>
      <!-- Rodas -->
      <g transform="translate(20,2)">
        <circle r="8" fill="#0b1030" stroke="#fff" stroke-width="2"/>
        <g><line x1="-5" x2="5" stroke="#fff" stroke-width="2"/>
          <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="0.6s" repeatCount="indefinite"/></g>
      </g>
      <g transform="translate(58,2)">
        <circle r="8" fill="#0b1030" stroke="#fff" stroke-width="2"/>
        <g><line x1="-5" x2="5" stroke="#fff" stroke-width="2"/>
          <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="0.6s" repeatCount="indefinite"/></g>
      </g>
      <g transform="translate(104,2)">
        <circle r="8" fill="#0b1030" stroke="#fff" stroke-width="2"/>
        <g><line x1="-5" x2="5" stroke="#fff" stroke-width="2"/>
          <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="0.6s" repeatCount="indefinite"/></g>
      </g>
    </g>
  </g>
</svg>
