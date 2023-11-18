---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
comments:
  host: neuromatch.social
  username: jonny
  id: 111390390531316777
image: assets/img/cover.png
author:
  twitter: json_dirs
  name: Jonny Saunders
  url: https://jon-e.net
seo:
  name: "Reimagining Archives and Scholarly Communication with Social-First Peer-to-Peer Infrastructures"
  type: PresentationDigitalDocument
  links:
    - https://www.abstractsonline.com/pp8/#!/10892/presentation/35685
---

<div class="toc" markdown="1">
* toc
{:toc}
</div>

<h2 markdown="1">**Reimagining Archives and Scholarly Communication with Social-First Peer-to-Peer Infrastructures**</h2>

*Jonny Saunders, Daniel Aharoni*

![CC-BY-SA License](assets/img/by-sa.svg)

- [AbstractsOnline](https://www.abstractsonline.com/pp8/#!/10892/presentation/35685)
- PSTR241.22 / WW65
- November 13, 2023, 8:00 AM - 12:00 PM
- WCC Halls A-C 
- Contact: [j@nny.fyi](mailto:j@nny.fyi)
- Page Source: [https://github.com/sneakers-the-rat/sfn23](https://github.com/sneakers-the-rat/sfn23)

# Poster

[.pdf (49.8MB)](assets/img/2023-sfn-jlsaunders.pdf)

![Alt text contained in the expandable poster-alt-text element below](assets/img/2023-sfn-jlsaunders.png){: aria-describedby="poster-alt-text"}
<details class="alt-text">
  <summary>Expand/Collapse Alt Text</summary>
  <div id="poster-alt-text" markdown="1">
  **Structural overview:** The poster is in several sections, roughly grouped in three columns. From the left, a sentence (below) frames the main content of the poster, center. The poster title and a set of boxes labeled "come talk to me about..." are on the right.

  **Title:** Social-First P2P<br>
  **Subtitle:** Strategies for Joy, Agency, and Ethics in Digital Infrastructure<br>
  **Authors:** Jonny Saunders, Daniel Aharoni<br>
  **Affiliations:** UCLA, Department of Neurology (Jonny, Daniel), Institute of Pirate Technology (Jonny)<br>
  **Web:** <https://jon-e.net/sfn23><br>
  **Contact:** j@nny.fyi

  **Leftmost framing sentence** (bold text, white, pink and yellow on black, intended to draw intention from a distance): If our wildest dreams for "open science" are pay amazon to rent our own data, pay microsoft to generate papers nobody wrote, pay elsevier to publish papers nobody reads to survive another day on the prestige treadmill, those are nightmares. We need better dreams.

  **Main content design:** Several subsections in the poster are laid out against a skull and crossbones as the main structuring element. The eyes of the skull and crossbones are schematic depictions of "the cloud" labeled AWS, with radial lines pointing inwards towards a large pink and black swirl, and the other eye is labeled "p2p" with many smaller circles connecting between each other. The abstract is in the forehead of the skull, framed by the phrase "Beyond the cloud" above, and "The swarm" below.

  **Abstract:** Open data is the next theater of enclosure for scientific infrastructure. In a race for an ill-specified “AI”-driven future thirsty for data, researchers and funding agencies alike are sleep walking into a trap. The cloud isn’t optimal or inevitable: it’s a business model intent on injecting ever-increasing storage and compute costs into the practice of science[1], profoundly limiting what our infrastructures could be. Peer to peer (p2p) infrastructures are the alternative. We present groundwork in data formats, sketching plans to build a new kind of social-first, graphical p2p system based on continuous, vernacular expression. Avoiding utopian pipe dreams, keeping close to actual practice,  we invite you to join us bridging work from private to public; local to global; across domains like data, compute, and publishing. We can have better dreams!

  ---

  The first two boxes on the leftmost ends of the "bones" in the skull and crossbones:

  **Delocalizing Archives:** Archives are social! We love our archivists, but why should they have all the fun? We can value their hard work, contribute what we can with eg. schema curation and tool development, and help defray the complexity and cost of hosting with P2P archive mirrors. We scraped DANDI and are using it as a test case for social organization of complex data.

  **NWB -> LinkML:** Formats should be vernacular! To facilitate fluid use of structured data, we developed nwb-linkml, an independent implementation of Neurodata Without Borders, translating it to LinkML in the process. This allows us to use NWB data with multiple backends (eg. relational databases, triple stores), write code-free schema extensions, and simplify its API with pydantic.

  ---

  Beneath, a hierarchical dataset is depicted as being broken up into a graph of nodes, which leads into a section of interconnected vignettes around a continuous graph, each of the sections are described below:

  The first section transitions from a hierarchical data structure representing the existing NWB format to a triple graph, with the text box **"to triples!"** labeling: "Inspired by RDF, subject-predicate-object triples model arbitrary data." An example shows a triple with two nodes "data" and "jonny" collected by the predicate 'collectedBy.'

  Above, a box **"Vernacular schema"** explains "Peers can make schemas as-needed, negotiating relationships between terms as a continuous languagelike social process." with an example of "mySchema" having a custom field "recordedWith tetrode" and "spunBy person" being declared "sameAs" my colleagues custom schema. 

  Beneath, a box **"Keep your files!"** shows how the graph dataset could be written to disk: "Git is great because it slips invisibly underneath files. Bittorrent is great because .torrents are just files. Separating the metadata graph from binary files gives us content addressability + friendly UX" with a schematic diagram of a merkle tree coupled with a metadata graph showing the format, shape, and order of the stored array.

  The center of the graph is a cluster of icons representing people, servers, computers, and datasets all connected to show different features of a **"Federated P2P"** system: "You’ve got multiple computers, so does your colleague and your university. Share resources between your rig computer and data server, rehost your colleague’s data, build archives and review co-ops. We can make new kinds of scientific societies beyond maintainers of traditional conferences and journals: federations of peers that govern and maintain common infrastructure for common good."

  The diagram shows one user "santi" with a draft dataset shared between their rig and analysis machines, backed up by a department server. The department server is mirrored by a lab server as well as a larger public archive, which holds many datasets. Other users "rumbly" and "ora" share data between multiple lab and department servers during a collaboration. A user "violet" is depicted as making use of a dataset from "ora," described in another box:

  **"Peer Review, Reuse, and Governance in Co-Op Mode"**: What if the alternative to journals was simply the existing social reality of research made visible? What’s more impressive, an h-index, or the extended graph of your contributions to the commons? P2P can help realign incentives towards cooperation - the very act of reusing someone’s work is to credit and rehost it. A continual process of contextualization isn’t the end of peer review, quite the opposite: it’s an opportunity for an unimaginably richer means of collaboratively evaluating work.

  This shows "violet" writing a post that referenced some academic rivals' post, using data from ora, an analysis pipeline from rumbly, which both rehosts and gives credit to the underlying work that it makes use of.

  Finally, at the bottom of the graph is a box **"Radical Interoperability!"**: "We don’t need a new platform or journal, we need to glue them together. We’ll be exploring...

  - Direct export data from and import config to experimental tooling
  - Crawlers to treat existing HTTP, RDBMS, S3, etc. resources as peers
  - Delegated identity and discovery from existing eg. social media."

  The accompanying diagram shows many different data sources from experimental tools to existing data repositories being linked to a dataset shared among peers. 

  ---

  The right two "bones" in the jolly roger are two final main text sections:

  **Public Spaces: Neuromatch.social** - Twitter showed us how direly we need social infrastructure - what if it was built to support us rather than mine our attention? Neuromatch.social is an experiment in cooperatively governed scientific infrastructure - and a lovely, blossoming community. We run a fork of Mastodon, a federated social media server, and invite all members to hack on the software, propose policies, and take ownership as co-equal members. It will be the social heart of our next phase, federation to p2p.

  **Local Organization: Wikis, Chat** - Organizing labor as a million google docs and slack messages is not our best work. We wrote chatbridge to bridge proprietary chat silos with a few clicks, and wikibot to gradually enrich chat streams with wiki gardens. We’ve seen fluidly structured semantic wikis change patterns of work across organizations, and will be working on p2p wikis for labs, unions, any group organizing people and information. 

  ---

  Finally, on the right side underneath the psoter title, are a set of boxes titled "Come talk to me about..."

  **Distributed Identity:** P2P systems are usually very lonely since peers typically have ephemeral or anonymous identities and don’t form a persistent social graph. The culture of BitTorrent trackers shows us that social organization is determinative of successful distributed archives, but how will identity work in clearnet p2p? Can we bootstrap identity from existing systems? Can we reverse the anarcho-capitalist plague of zero-trust “web 3” with explicit networks of trust?

  **Vernacular Schema:** A recurring failure mode of linked data information systems is a drift towards few, authoritative schema warded by a closed ontological priesthood[2]. Language doesn’t work like that, though, and language rocks. Can we do that instead? Can we create an evolving system of computer-readable meaning? How shall we negotiate, fork, and merge infinite variations of expression? Can we use social graphs as context to infer what is meant without needing to get a complete URI involved every time? 

  **Adversarial Interoperability:** The only thing scientists love more than pining for better infrastructure is getting absolutely steamrolled by billion-dollar industries when we try. Surveillance publishers and cloud giants are not our friends. Friends don’t turn calls for “open science” into new, more extractive, more inequitable models. How can anti-profitable technologies use the walled gardens without being captured by them? What openings might give us the upper hand? Can we build bridges for our colleagues stuck in information industry traps?  

  **Cooperative Governance:** Let’s not get distracted amidst the graphs and technology: the problems of scholarly infrastructure are primarily social organizing problems. Organizational modalities carry their own logic. Traditional board-run nonprofits will hold listening sessions and mean well, but power always flows from the top of a hierarchy. P2P systems require us to cooperate, but can academics cooperate if it means genuinely ceding power? Can we move past shopping for Infra as a Service and believe in our collective power to make it ourselves?

  ---

  A set of references in the bottom right corner:

  nwb-linkml     

  - source: <https://github.com/p2p-ld/nwb-linkml/>
  - docs:   <https://nwb-linkml.readthedocs.io>

  chatbridge    

  - source: <https://git.jon-e.net/jonny/chatbridge>

  neuromatch.social 

  - source: <https://github.com/NeuromatchAcademy/mastodon>
  - docs:   <https://wiki.neuromatch.social>

  miniscope-io      

  - source: <https://github.com/Aharoni-Lab/miniscope-io>
  - docs:   <https://miniscope-io.readthedocs.io>

  p2p-ld          

  - docs:   <https://piracy.solutions/docs/>

  autopilot  

  - source: <https://github.com/auto-pi-lot/autopilot>
  - docs:   <https://docs.auto-pi-lot.com>

  wikibot   

  - source: <https://git.jon-e.net/jonny/wiki-postbot/>

[1] Saunders, J. (2022) “Decentralized Infrastructure for (Neuro)-Science” doi:[10.48550/arXiv.2209.07493](https://doi.org/10.48550/arXiv.2209.07493), <https://jon-e.net/infrastructure>

[2] Saunders, J. (2023) “Surveillance Graphs” 
    doi:[10.17613/syv8-cp10](https://doi.org/10.17613/syv8-cp10), <https://jon-e.net/surveillance-graphs>     

  </div>

</details>

# Abstract

<details class="alt-text">
  <summary>Expand/Collapse Abstract</summary>
  <div id="abstract-text" markdown="1">
> If our wildest dreams for scholarly infrastructure are to outsource our archives to Amazon and pay Elsevier for prestigious PDFs, it might be time to wake up. One can only admire the boldness of neuroscientists grappling with the staggering complexity of the brain 20 pages and 20 mice at a time. More than our ambition, skill, or resources, it is our infrastructures that constrain our work. If we consider our digital infrastructural problems separately, we find ourselves tracing familiar patterns: a mutually incompatible string of journal-like venues, cloud storage, and SaaS platforms. 
>
>We present a different strategy, a new generation of peer-to-peer (p2p) protocols for social information infrastructures to bridge data, computation, and communication. Learning from decades of prior art from p2p, decentralized messaging, Semantic Web, federated social media, and wiki communities, we propose a protocol for content-addressed containers of linked data triples in an explicitly social system, blending the best of traditional p2p and federated systems. 
>
> In this first phase of development, we will present results from a proof of concept protocol designed to integrate data from prevailing neurophysiology formats and the wild vernacularism of hand-structured data. Rather than a backwards-incompatible system-of-everything that requires radically reconfiguring existing practice, we show how p2p can bridge resources from rig computers, lab and institutional servers, and existing cloud archives to make each more useful than in isolation. 
>
> We plot a course for future work where by taking the social reality of infrastructure seriously we can reimagine publishing data and results as a continual process of collaboration, communication, and cooperative governance, rather than some exogenous burden at the end of an experiment where we throw ourselves at the mercy of multiple adversarial industries. Beyond the practical limitations of archives with always-higher storage and egress bills and a communication system riddled with perverse incentives, sleepwalking into a near-future where we hand ownership of scientific infrastructure to a few for-profit information conglomerates would be an ethical nightmare.
>
> We can either become yet another engine of the enclosure of digital infrastructure, or we can use our rare position as publicly funded researchers not beholden to profit to seed information systems for the public good. This work is an invitation to my colleagues to join us in future phases of development, integrating existing projects with new ones, and reclaiming our joy and agency rebuilding the systems that define the daily practice of science
</div>
</details>


# References

- Saunders, J. (2022) **Decentralized Infrastructure for (Neuro)science**<br>doi:[10.48550/arXiv.2209.07493](https://doi.org/10.48550/arXiv.2209.07493), <https://jon-e.net/infrastructure><br>
*A historical, political, and technical manifesto for a cooperative web*

- Saunders, J. (2023) **Surveillance Graphs**<br>doi:[10.17613/syv8-cp10](https://doi.org/10.17613/syv8-cp10), <https://jon-e.net/surveillance-graphs><br>
*Articulating anticapitalist data infrastructures: a brief history of knowledge graphs, their cognitive pattern as a part of the cloud orthodoxy, and their fate as mass surveillance technologies when paired with large language models.*

- `nwb-linkml` - [docs](https://nwb-linkml.readthedocs.io/en/latest/), [code](https://github.com/p2p-ld/nwb-linkml/)<br>
*An independent implementation of the NWB format and a translation to LinkML.*

- `chatbridge` - [code](https://git.jon-e.net/jonny/chatbridge)<br>
*A lightweight full-stack web app for bridging channels in proprietary chat platforms. Unlike Matrix bridges which are 1:1 mirrors from one server/workspace to a matrix room, chatbridge can support all-to-all groups, handling the tricky parts of setting up API access so participants can join with an invite token and a few clicks*

- `neuromatch.social` - [wiki](https://wiki.neuromatch.social), [code](https://github.com/NeuromatchAcademy/mastodon)<br>
*Our fork-of-a-fork of Mastodon, hacking on scholarly communication and cooperative governance*


- `miniscope-io` - [docs](https://miniscope-io.readthedocs.io), [code](https://github.com/Aharoni-Lab/miniscope-io)<br>
*Rebuilding a lightweight I/O SDK for miniscopes*

- `p2p-ld` - [docs](https://piracy.solutions/docs/)<br>
*Coordinating docs for the overarching p2p project. Currently just a collection of notes :)*

- `autopilot` - [docs](https://docs.auto-pi-lot.com), [code](https://github.com/auto-pi-lot/autopilot)<br>
*A framework for complex experiments distributed across many computers*

- `wikibot` - [code](https://git.jon-e.net/jonny/wiki-postbot/)<br>
*A handful of bots for linking wikis with chat and microblogging platforms. Experiments in merging the 'garden' with the 'stream'*



<br>

# Comments

{% include comments.html %}

