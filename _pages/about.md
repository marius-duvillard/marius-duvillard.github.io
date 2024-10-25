---
permalink: /
title: "Welcome to My Personal Website! 🌟"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

👨‍🎓 PhD in Applied Mathematics | 🎓 École Polytechnique | ⚡CEA

Currently working with CEA at Cadarache on cutting-edge research for nuclear fuel manufacturing.
I'm part of the X/Inria project-team [PLATON](https://team.inria.fr/platon/).

<div id="countdown" class="countdown" data-role="countdown" data-stoptimer="2025-01-16 00:00"></div>

## 🔬 Fields of Interest

- **Data Assimilation & UQ**: Advanced techniques for integrating data into simulations and Uncertainty Quantification methods.
- **Machine Learning & Data-Driven Methods**: Applying ML and data-driven techniques to mechanical modeling in the paradigm of SciML.
- **Data Analysis**: Analyzing diverse datasets to uncover insights and transform raw data into actionable information.  
- **Solid Mechanics**: Innovative approaches to understanding and simulating solid mechanics.


📚 [**Publications and Research**](publications/): Discover my contributions to numerical simulation, machine learning, and data assimilation.

🎤 [**Conferences**](talks/): Check out my presentations.

🎵 **Hobbies**: Ancient and traditional music 🎼, rowing 🚣‍♂️, hiking 🌄 and literature 📖.

feel free to browse through [**my CV**](cv/) 📄 I'm open to new opportunities and collaborations, so don't hesitate to get in touch! 🤝


<!-- jQuery -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
<!-- Plugin metro-countdown.js -->
<script src="{{ '/assets/js/metro-countdown.js' | relative_url }}"></script>

<script>
  $(document).ready(function() {
    $("#countdown").countdown({
      style: {
        background: "bg-blue", // Classe pour l'arrière-plan du décompte
        foreground: "fg-white", // Classe pour le texte
        divider: "fg-red"       // Classe pour le séparateur
      },
      blink: true, // Activer le clignotement du séparateur
      stoptimer: "2025-01-01 00:00", // Date de fin du décompte
      ontick: function(d, h, m, s) {
        console.log(`Temps restant : ${d}j ${h}h ${m}m ${s}s`);
      },
      onstop: function() {
        alert("Temps écoulé !");
      }
    });
  });
</script>