<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 600 600" width="600" height="600">

  <!-- Background -->
  <rect width="600" height="600" fill="#0f1117"/>

  <!-- Title -->
  <text x="300" y="38" text-anchor="middle" fill="#e8e0d0" font-size="13" letter-spacing="3" font-family="Georgia, serif">THE CAPABILITY FLYWHEEL</text>
  <text x="300" y="56" text-anchor="middle" fill="#555" font-size="10" letter-spacing="2" font-family="Georgia, serif">WHY LEADERS BECOME STRUCTURALLY DIFFICULT TO CATCH</text>

  <!-- Center circle -->
  <circle cx="300" cy="310" r="58" fill="#0f1117" stroke="#2a3050" stroke-width="1.5"/>
  <text x="300" y="302" text-anchor="middle" fill="#6677aa" font-size="9" letter-spacing="2" font-family="Georgia, serif">ASYMMETRICAL</text>
  <text x="300" y="317" text-anchor="middle" fill="#8899cc" font-size="11" font-weight="bold" font-family="Georgia, serif">CAPABILITY</text>
  <text x="300" y="332" text-anchor="middle" fill="#8899cc" font-size="11" font-weight="bold" font-family="Georgia, serif">ACCUMULATION</text>

  <!-- 
    5 nodes placed on a circle of radius 195, starting top and going clockwise:
    Node 1 (top):         270° → x=300, y=115
    Node 2 (upper right): 342° → x=486, y=203
    Node 3 (lower right): 54°  → x=457, y=452
    Node 4 (lower left):  126° → x=143, y=452
    Node 5 (upper left):  198° → x=114, y=203
    
    Using: cx + r*cos(angle), cy + r*sin(angle) where cy=310
    r=195
    
    Node 1: 300 + 195*cos(270°) = 300+0 = 300,  310 + 195*sin(270°) = 310-195 = 115
    Node 2: 300 + 195*cos(342°) = 300+185 = 485, 310 + 195*sin(342°) = 310-60 = 250  
    Node 3: 300 + 195*cos(54°)  = 300+115 = 415, 310 + 195*sin(54°)  = 310+158 = 468
    Node 4: 300 + 195*cos(126°) = 300-115 = 185, 310 + 195*sin(126°) = 310+158 = 468
    Node 5: 300 + 195*cos(198°) = 300-185 = 115, 310 + 195*sin(198°) = 310-60 = 250
  -->

  <!-- Curved arrows between nodes (clockwise flow) -->
  <!-- Arrow 1→2: top to upper-right -->
  <path d="M 322 128 Q 430 148 470 238" fill="none" stroke="#3a4a7a" stroke-width="2" stroke-dasharray="0"/>
  <polygon points="472,250 462,238 474,234" fill="#3a4a7a"/>

  <!-- Arrow 2→3: upper-right to lower-right -->
  <path d="M 488 264 Q 510 370 428 458" fill="none" stroke="#4a5a6a" stroke-width="2"/>
  <polygon points="420,465 424,453 434,460" fill="#4a5a6a"/>

  <!-- Arrow 3→4: lower-right to lower-left -->
  <path d="M 400 478 Q 300 510 200 478" fill="none" stroke="#4a6a5a" stroke-width="2"/>
  <polygon points="190,472 200,466 202,478" fill="#4a6a5a"/>

  <!-- Arrow 4→5: lower-left to upper-left -->
  <path d="M 172 458 Q 90 370 112 264" fill="none" stroke="#5a6a4a" stroke-width="2"/>
  <polygon points="113,252 110,264 122,262" fill="#5a6a4a"/>

  <!-- Arrow 5→1: upper-left to top -->
  <path d="M 130 238 Q 170 148 278 128" fill="none" stroke="#6a7a3a" stroke-width="2"/>
  <polygon points="290,125 278,120 280,132" fill="#6a7a3a"/>

  <!-- NODE 1 — Better Infrastructure (top) -->
  <rect x="195" y="88" width="210" height="54" rx="5" fill="#141828" stroke="#3a4a7a" stroke-width="1.5"/>
  <text x="300" y="109" text-anchor="middle" fill="#6677bb" font-size="9" letter-spacing="2" font-family="Georgia, serif">01</text>
  <text x="300" y="127" text-anchor="middle" fill="#e8e0d0" font-size="13" font-weight="bold" font-family="Georgia, serif">Better Infrastructure</text>

  <!-- NODE 2 — Better Operational Capability (upper right) -->
  <rect x="390" y="222" width="210" height="54" rx="5" fill="#141828" stroke="#4a5a6a" stroke-width="1.5"/>
  <text x="495" y="243" text-anchor="middle" fill="#667788" font-size="9" letter-spacing="2" font-family="Georgia, serif">02</text>
  <text x="495" y="264" text-anchor="middle" fill="#e8e0d0" font-size="13" font-weight="bold" font-family="Georgia, serif">Better Capability</text>

  <!-- NODE 3 — Better Data / Learning (lower right) -->
  <rect x="355" y="440" width="210" height="54" rx="5" fill="#141828" stroke="#4a6a5a" stroke-width="1.5"/>
  <text x="460" y="461" text-anchor="middle" fill="#668877" font-size="9" letter-spacing="2" font-family="Georgia, serif">03</text>
  <text x="460" y="479" text-anchor="middle" fill="#e8e0d0" font-size="13" font-weight="bold" font-family="Georgia, serif">Better Learning</text>

  <!-- NODE 4 — Better Capital Returns (lower left) -->
  <rect x="35" y="440" width="210" height="54" rx="5" fill="#141828" stroke="#4a6a5a" stroke-width="1.5"/>
  <text x="140" y="461" text-anchor="middle" fill="#779966" font-size="9" letter-spacing="2" font-family="Georgia, serif">04</text>
  <text x="140" y="479" text-anchor="middle" fill="#e8e0d0" font-size="13" font-weight="bold" font-family="Georgia, serif">Better Returns</text>

  <!-- NODE 5 — More Infrastructure Investment (upper left) -->
  <rect x="0" y="222" width="210" height="54" rx="5" fill="#141828" stroke="#6a7a3a" stroke-width="1.5"/>
  <text x="105" y="243" text-anchor="middle" fill="#889955" font-size="9" letter-spacing="2" font-family="Georgia, serif">05</text>
  <text x="105" y="264" text-anchor="middle" fill="#e8e0d0" font-size="13" font-weight="bold" font-family="Georgia, serif">More Investment</text>

  <!-- Examples below each node -->
  <text x="300" y="150" text-anchor="middle" fill="#445" font-size="9" font-family="Georgia, serif">TSMC fabs · Hyperscaler compute · Energy</text>

  <text x="495" y="282" text-anchor="middle" fill="#445" font-size="9" font-family="Georgia, serif">Yield · Translation · Operationalization</text>

  <text x="460" y="500" text-anchor="middle" fill="#445" font-size="9" font-family="Georgia, serif">Process knowledge · Data · Model performance</text>

  <text x="140" y="500" text-anchor="middle" fill="#445" font-size="9" font-family="Georgia, serif">Moats · Value capture · Platform leverage</text>

  <text x="105" y="282" text-anchor="middle" fill="#445" font-size="9" font-family="Georgia, serif">Reinvestment · Capex · R&D · Ecosystem</text>

  <!-- Reinforcement label in center bottom of center circle -->
  <text x="300" y="352" text-anchor="middle" fill="#333" font-size="9" letter-spacing="1" font-family="Georgia, serif">self-reinforcing</text>

  <!-- Bottom rule and caption -->
  <line x1="40" y1="560" x2="560" y2="560" stroke="#222" stroke-width="1"/>
  <text x="300" y="578" text-anchor="middle" fill="#444" font-size="9" letter-spacing="1" font-family="Georgia, serif">THE ENGINES BEHIND — NORTHLOGICLAB</text>
  <text x="300" y="593" text-anchor="middle" fill="#333" font-size="9" letter-spacing="1" font-family="Georgia, serif">Each rotation widens the gap between leaders and followers</text>

</svg>