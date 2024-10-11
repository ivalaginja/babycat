---
title: About
layout: single
classes: wide
permalink: /about/
sidebar:
  nav: "about"
---

## What is a Coronagraph?

A coronagraph is an optical instrument used in astronomical observations. It [manipulates the light from a star](https://www.stsci.edu/contents/annual-reports/2019/manipulating-starlight) in order to
allow observations of faint objects around it. Originally, the solar coronagraph was developed to observe the Sun's corona. After
adaptations in the 60's and 70's, stellar coronagraphs can be used to find exoplanets, study a star's environment, and
observe circumstellar disks. NASA's next flagship mission, the Habitable Worlds Observatory (HWO), will be specifically
designed for coronagraphy in order to find and characterize several tens of potentially habitable, Earth-like exoplanets.

A coronagraph consists of various masks that, when used in combination, attenuate the starlight while allowing the faint
planet light to shine through. There are many different types of coronagraphs, as the optical masks can be located in
different optical planes (pupil planes and focal planes) and act on either component of the electrical field (amplitude or phase).

The original Lyot coronagraph is a simple design that uses a pair of masks to block the starlight. The
focal-plane mask (FPM) is an opaque, sharp-edge disk in the focal plane placed over the core of the stellar point-spread
function (PSF). The Lyot stop (LS) is an annular mask in the pupil plane that blocks the light diffracted by the FPM.

For more information on coronagraphy, see the [references](#resources) below.

## Purpose of the Project

The BabyCAT project is a demonstration bench that uses a Lyot coronagraph to show how coronagraphy works. It provides 
hands-on experience with coronagraphy and is designed to help students, researchers, and enthusiasts learn about it.
The setup is inspired by the need for easy-to-build optical setups that can be used in classrooms, labs, and transported
easily to conferences and outreach events.

## Background

The BabyCAT project was designed in 2019 by a team of scientists at the
[Russell B. Makidon Optics Laboratory](https://www.stsci.edu/stsci-research/research-topics-and-programs/russell-b-makidon-optics-laboratory)
at the [Space Telescope Science Institute](https://www.stsci.edu/).
Its goal is to make advanced optical techniques more accessible to a wider audience.

The first ever BabyCAT coronagraph demonstration bench was built in 2019 and has since been used in various educational
and research settings. Most of the documentation and educational materials were created by SASP
([Space Astronomy Summer Program](https://www.stsci.edu/opportunities/space-astronomy-summer-program)) intern Lucas Batista,
who worked with the RMOL team and STScI's Office of Public Outreach (OPO) during the summer of 2019.

{: .notice--info}
**The name:** Why "BabyCAT"? The workhorse project of the RMOL team is the [HiCAT testbed](https://ui.adsabs.harvard.edu/abs/2024arXiv240912931S/abstract) - the
"High-contrast imager for Complex Aperture Telescopes" testbed. Since the demo coronagraph was supposed to illustrate a
mini version of HiCAT, the name "BabyCAT" seemed immediately evident.

The second demo bench, BabyCAT 2.0, was also assembled at the Makidon lab and later delivered to ExEP at NASA's Jet
Propulsion Laboratory (JPL). Its upgraded design is the one that is presented on this website. 

## Where This Setup Is Used

The following institutions and groups own their own version of BabyCAT:

- **Institution Name**: RMOL at STScI
  - **Location**: Baltimore (MD), USA
  - **Demo name**: BabyCAT

- **Institution Name**: ExEP at JPL, NASA
  - **Location**: Pasadena (CA), USA
  - **Demo name**: BabyCAT 2.0

- **Institution Name**: UC Santa Cruz
  - **Location**: Santa Cruz (CA), USA
  - **Demo name**: sealPUP

## Resources

- How a coronagraph works, combined with wavefront correction: [Video](https://www.youtube.com/watch?v=zkTHuqiH_1Y)
- Introduction to optics, Iva Laginja at the Sagan Summer Workshop 2024: [Video](https://www.youtube.com/watch?v=vq6YOuWVIuk)
- Introduction to coronagraphy, David Doelman at the Sagan Summer Workshop 2024: [Video](https://www.youtube.com/watch?v=SYHAL5hxEbQ)

- SASP student presentation by Lucas Batista: [Recording](https://cloudproject.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=9bb1e9b5-8229-426e-a6fc-aaa400fe927a) - starting at 31:18
- Batista et al. (2020): [BAAS, Vol. 52, No. 1](https://ui.adsabs.harvard.edu/abs/2020AAS...23520313B/abstract) - [Poster](https://github.com/ivalaginja/babycat/tree/main/assets/pdfs/Batista-et-al_AAS-poster-Jan-2020.pdf)
- RMOL publication list: [ADS library](https://ui.adsabs.harvard.edu/public-libraries/0jrikEsaQ6W3ubvGa3ZivA)
- RMOL website: [RMOL](https://www.stsci.edu/stsci-research/research-topics-and-programs/russell-b-makidon-optics-laboratory)
- STScI website: [STScI](https://www.stsci.edu/)
- Habitable Worlds Observatory: [HWO](https://habitableworldsobservatory.org/home)

## Team

- **Website**: [Iva Laginja](https://ivalaginja.github.io/)
- **Project lead and optical design**: Rémi Soummer
- **Alignments, star and planet simulator**: Greg Brady, Pete Petrone, Evelyn McChesney
- **Educational and outreach materials**: Lucas Batista, Timothy Rhue, Alexandra Lockwood
- **Documentation and parts lists**: Greg Brady, Iva Laginja, Jules Fowler, Scott Will, Maggie Kautz, Lucas Batista


## License and Attribution

The content of this project itself is licensed under the [Creative Commons Attribution-Noncommercial 4.0 International license](https://creativecommons.org/licenses/by-nc/4.0/deed.en),
and the underlying source code used to format and display that content is licensed under the [MIT license](https://github.com/ivalaginja/babycat/blob/main/LICENSE.md).

If you decide to build your own BabyCAT, we would appreciate it if you could let us know! If you can, please open a new
pull request on our [repo](https://github.com/ivalaginja/babycat) and add your setup to the "Where This Setup Is Used"
section on the [About page](https://github.com/ivalaginja/babycat/blob/103fcb7ee5d4079e2fa5718537a93478276de5b8/_pages/about.md?plain=1#L53).
Alternatively, you can open a [GitHub issue](https://github.com/ivalaginja/babycat/issues) or email us (see [Team](#team))
and we will do this for you. We can also include some of your pictures in our [gallery](/gallery/) if you would like!

{: .notice--info}

If you are presenting a demo coronagraph built after our base design, please give us credit by **including the website URL**
on presentation slides and associated materials, showing the [logo](https://github.com/ivalaginja/babycat/blob/main/assets/images/Babycat_logo_text.jpeg)
if possible.

If you are preparing a publication that cites references, please cite the website with:

```bibtex
@software{Laginja2024BabyCATwebsite,
  author       = {Laginja, Iva and
                  Soummer, Rémi and
                  Brady, Greg and
                  Petrone, Peter and
                  McChesney, Evelyn and
                  Batista, Lucas and
                  Rhue, Timothy and
                  Lockwood, Alexandra and
                  Fowler, Jules and
                  Will, Scott and
                  Kautz, Maggie},
  title        = {ivalaginja/babycat: BabyCAT launch},
  month        = oct,
  year         = 2024,
  publisher    = {Zenodo},
  version      = {v0.1.0},
  doi          = {10.5281/zenodo.13916899},
  url          = {https://doi.org/10.5281/zenodo.13916899}
}
```

## Disclaimer

The information provided on this website, including parts lists, specifications, estimated prices, and sources, is
intended for educational purposes only. While we strive to ensure accuracy, we make no guarantees regarding the
completeness, correctness, or currentness of the information. Prices listed are only estimates and may vary depending
on supplier and market conditions.

We are not affiliated with, nor do we endorse or receive sponsorship from, any of the vendors mentioned on this website.
All product references and links to external sources are provided for convenience and should not be taken as an endorsement.

By using this website, you acknowledge and agree that we cannot be held responsible or liable for any errors, omissions,
or discrepancies in the information provided, nor for any actions taken based on this information. Users are encouraged
to verify details independently before making purchases or relying on the provided information.
