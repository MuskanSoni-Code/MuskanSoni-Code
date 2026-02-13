<svg width="360" height="360" viewBox="0 0 360 360" xmlns="http://www.w3.org/2000/svg">

  <!-- ROTATING RING -->
  <g opacity="0.9">
    <animateTransform attributeName="transform"
      type="rotate"
      from="0 180 180"
      to="360 180 180"
      dur="16s"
      repeatCount="indefinite" />

    

  <!-- CIRCLE MASK -->
  <defs>
    <clipPath id="profileMask">
      <circle cx="180" cy="180" r="85"/>
    </clipPath>
  </defs>

  <!-- PROFILE IMAGE -->
  <image
    href="https://raw.githubusercontent.com/MuskanSoni-Code/MuskanSoni-Code/main/profile.png"
    x="95"
    y="95"
    width="170"
    height="170"
    clip-path="url(#profileMask)"
    preserveAspectRatio="xMidYMid slice" />

  <!-- BORDER -->
  <circle cx="180" cy="180" r="88"
    fill="none"
    stroke="#1f6feb"
    stroke-width="2"/>

</svg>
