# Front-end Style Guide

## Layout

The designs were created to the following widths:

- Mobile: 375px
- Desktop: 1440px

> 💡 These are just the design sizes. Ensure content is responsive and meets WCAG requirements by testing the full range of screen sizes from 320px to large screens.

## Colors

- White: hsl(0, 0%, 100%)

- Stone 100: hsl(30, 54%, 90%)
- Stone 150: hsl(30, 18%, 87%)
- Stone 600: hsl(30, 10%, 34%)
- Stone 900: hsl(24, 5%, 18%)

- Brown 800: hsl(14, 45%, 36%)

- Rose 800: hsl(332, 51%, 32%)
- Rose 50: hsl(330, 100%, 98%)

## Typography

### Body Copy

- Font size (paragraph): 16px

### Fonts

- Family: [Young Serif](https://fonts.google.com/specimen/Young+Serif)
- Weights: 400

- Family: [Outfit](https://fonts.google.com/specimen/Outfit)
- Weights: 400, 600, 700

> 💎 [Upgrade to Pro](https://www.frontendmentor.io/pro?ref=style-guide) for design file access to see all design details and get hands-on experience using a professional workflow with tools like Figma. The design file for this challenge also includes a design system and tablet layout to help you build a more accurate solution faster.






li {
    padding-left: 1.25rem; /* Medzera medzi bodkou a textom */
    padding-top: 1rem;
    color: var(--Stone600);
}


li:last-child {
    margin-bottom: 0;      /* Posledná položka nepotrebuje spodnú medzeru */
}

/* Všeobecné nastavenie pre zoznamy */
ul, ol {
    padding-left: 1.175rem; /* Priestor pre bodky/čísla */
    margin-top: 0.75rem;
}

li {
    padding-left: 1.25rem; /* Medzera medzi bodkou a textom */
    padding-top: 0;        /* Zruš tento padding, ktorý to odsúva */
    margin-bottom: 0.5rem; /* Pridaj jemnú medzeru medzi položky */
    color: var(--Stone600);
    line-height: 1.5;      /* Zabezpečí pekné riadkovanie textu */
}


.preparation-time li::marker {
    color: var(--Rose800);
    font-size: 0.8rem;
}


/* 2. Štýlovanie jednotlivých riadkov (li) */
li {
    margin-bottom: 0.5rem;   /* Medzera medzi jednotlivými bodkami */
    padding-left: 1.35rem;      /* KĽÚČOVÉ: Medzera medzi bodkou a začiatkom textu */
    line-height: 1.55;        /* Aby sa text dobre čítal a odrážka bola v strede prvého riadku */
    color: var(--Stone600);  /* Farba textu */
}

/* Desktop Styles (Larger screens (min-width: 23.5rem)) */
@media (min-width: 48rem)  /* 48rem = 768px (tablety a desktopy) */ {
    .card {
        width: 21.75rem; 
        padding: 2.25rem 2.25rem;
    } 

    h1 {
        font-size: 1.35rem; 
        padding-block-start: 1.55rem;
    }

    .place {
        font-size: 0.76rem;
        padding-block-start: 0.55rem;
    }

    .position {
        font-size: 0.77rem;
        padding-block-start: 1.6rem;
    }

    img {
        width: 5rem; /* Fixná šírka avataru */
        height: 5rem;    
    }

    .social-links {
        padding: 1.52rem 0 0 0;
        gap: 0.9rem; /* Pridá rovnomerné medzery medzi tlačidlá */
    }

    .social-links a {
        padding: 0.8rem;    /* Trochu užšie tlačidlá pôsobia na desktope elegantnejšie */
        font-size: 0.8rem;   /* Prispôsobenie veľkosti písma k ostatným textom */
    }
}

@media (prefers-reduced-motion: reduce) {
  * {
    transition: none;
    animation: none;
  }
}