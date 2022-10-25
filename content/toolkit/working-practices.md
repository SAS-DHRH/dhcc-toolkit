---
title: "Working Practices"
date: 2022-10-25
draft: false
weight: 8
slug: working-practices
---


# Working Practices

While data management plans focus strongly on the data produced or reused by research projects, the whole research process itself represents a long path of decision-making that involves the assessment of the project’s environmental footprint. This section is intended to help you make informed decisions about the research process, from using devices to communicating with your team. See also the [Decision Trees](https://sas-dhrh.github.io/dhcc-toolkit/toolkit/decision-trees.html) and [Project Planning](https://sas-dhrh.github.io/dhcc-toolkit/toolkit/project-planning.html) sections.

{{<hint info>}}
**Read:** Bibliography and raw ideas can be found in the [Frameapad here](https://semestriel.framapad.org/p/toolkit_decisiontree-9tho?lang=en).
{{</hint>}}


## Using digital devices in general

**Device lifecycles**

Hardware has an **embodied carbon** cost, in addition to whatever electricity it uses. It is best to use devices as long as possible e.g., to repair them when possible. If you purchase a device through your institution, it is advisable to require the longest possible warranty for all newly purchased devices (this is of course also true if you purchase the device for individual use). There has been a growing awareness of the importance of repairability, which is now used as a selling point by companies. Sometimes it is more a greenwashing argument than an actual indicator of repairability (see as an example [this Greenpeace assessment of the repairability of some smartphones, laptops and tablets](https://www.greenpeace.org/static/planet4-eastasia-stateless/2019/11/47a8cd27-47a8cd27-howrepairableisyourmobiledevice.pdf)). Some companies rely on repairability of device components like [Fairphone](https://www.fairphone.com/en/) and [Framework](https://frame.work/gb/en) but there are still few of them. Therefore, think about buying a second-hand-device. Often they are sold updated with partly new hardware. 

For your old devices that are broken beyond repair, you can inquire into the forms of recycling that are possible. Check online for WEEE (Waste Electrical and Electronic Equipment, [DEEE](https://ecoinfo.cnrs.fr/thematiques/ressources-et-e-dechets/deee-ou-e-dechets/) in French, application in Germany and Europe explained in German [here](https://deutsche-recycling.de/weee-eu-richtlinie/#)). 

In order to have a precise idea of the environmental footprint of a device, you can consult the corresponding Life-Cycle Assessment ([LCA](https://en.wikipedia.org/wiki/Life-cycle_assessment), [here](https://ecoinfo.cnrs.fr/thematiques/analyse-de-cycle-de-vie/) for an explanation in French) that hardware companies usually provide. LCAs are never fully accurate - some of the information they contain are rough estimates, and the criteria that are communicated are only a handful from a long list. But they remain the best way of assessing the digital footprint of a device or hardware.

**Device types**

All in all, the fewer devices you purchase and use, the better. The choice of device also plays an important role when it comes to the amount of electricity consumed. For example, for streaming one hour of content via good wifi in HD quality, a laptop uses 9g CO2, a tablet 1.2 g and a smartphone 0.5g (and a television 48g). Source: https://www.iea.org/commentaries/the-carbon-footprint-of-streaming-video-fact-checking-the-headlines. Choices regarding peripheral hardware like mouses and keyboards can also make a difference to energy consumption. While the type of connection (cable vs. bluetooth) is marginal (see this [thread on Stackoverflow](https://hardwarerecs.stackexchange.com/questions/14045/usb-mouse-vs-bluetooth-mouse-less-battery-drain)), some devices also require batteries that need to be replaced or recharged regularly.

Sometimes, you might be able to work faster with a laptop than with a smartphone, or with two monitors rather than one. At other times, the screen size may not influence what you do or how much time you need to do it. Accordingly, it may not be necessary to switch devices or use multiple monitors for a given task; try stepping back and reflecting on the kind of device you really need for the task in hand. For example, you could unplug your second monitor and only plug it in when it helps you work more efficiently (the monitor itself not only has a considerable carbon weight but it also requires much more energy than your laptop). 

Of course, every digital device uses electricity; we don't need to stop using our devices, but should be conscious of our choices and their relative environmental costs. 

## Using an operating system

We cannot say that one operating system (like Windows, Linux, MacOS) is better from a carbon footprint point of view than another. There are too many different versions of the systems to compare them in the abstract. But we can check whether there are a lot of elements running in the background, and whether there are a lot of programs that run automatically on start-up, when we don’t need them at that moment. 

**Towards minimal operating systems**

Unikernels provide a light-weight alternative to traditional VMs or containers. Technologies such as [MirageOS](https://mirage.io/) offer a declarative way to build statically compiled binaries that can run directly over a hypervisor or even over bare metal. This approach allows minimal systems to be built which contain the exact functionality required for the task, even down to being able to specify what parts of a network stack are required. This not only provides opportunity for improving the security of the running system but also can result in energy savings compared to traditional operating systems such as Linux.

{{< hint info >}}
**Watch:** [Leaving legacy behind. Reducing carbon footprint of network services with MirageOS unikernels](https://media.ccc.de/v/36c3-11172-leaving_legacy_behind), Hannes Mehnert.
{{< /hint >}}
{{< video "https://media.ccc.de/v/36c3-11172-leaving_legacy_behind/oembed" >}}



## Day-to-day working and data traffic

New technologies for facilitating **data traffic**, like 5G, come with a massive growth of data consumption. In terms of impact, the rule of thumb for least energy intensive to most would be: Wired connection > Wifi > 3G > 4G > 5G. A poor internet connection has a better carbon footprint than a strong one. 

For example, let’s imagine you use a smartphone for one hour and you stream something in HD quality. With a “low” Wifi connection you might need 4g CO2 in total, with a “high” Wifi connection you might need 10g CO2 in total. Source: https://www.iea.org/commentaries/the-carbon-footprint-of-streaming-video-fact-checking-the-headlines 

Best practice around **emailing**, especially storage, remains a subject of debate, and we invite perspectives and evidence to inform future editions of the toolkit. You can minimise the impact of emails by following a few simple rules. First, avoid integrating an image footer as a signature in your emails. (Consider communicating to your teammates the environmental cost of including images, such an institutional logo, in email signatures). Second, avoid emailing large groups of people unless it is necessary.

Emails are stored as long as they are in your inbox or in subfolders of your inbox, so some savings may be made by clearing out your inbox regularly. You can prioritise emails with attached files (a regular email weighs 4g CO2, and an email with a photo 50g CO2). There is a small energy cost associated with deleting emails; our current understanding is that this is typically outweighed by the benefit, although such trade-offs are one reason the benefits are difficult to estimate.  

**Sharing files**. You might think about using a download link (e.g. provided by Cloud storage) to share documents instead of sending them via e-mail. It is advisable to use online documents especially when: 1) the shared document has a large file size, 2) you have a high number of recipients. 

**Documents stored in cloud or network drives** require traffic for saving files and synchronisation. Network drives usually synchronise file-by-file, which means each change will result in uploading the document completely again. Especially when editing large files, you might consider copying them once to your local drive, editing there and then copying the edited version back when you are finished. Most cloud solutions only require traffic for the modified parts of a file. On the backend, cloud storages usually synchronise automatically on every modification. You can disable the client temporarily or turn on cloud synchronisation only when you need it in order to save energy from additional, superfluous traffic. Generally, saving the document less often will reduce energy consumption if you edit remotely stored documents.

**Editing documents online together** is a good solution to avoid frequent email traffic, besides the advantage of synchronous editing or synchronisation. However, each time you open an online document, the application needs to be loaded into your browser memory, which creates a lot of traffic. Additionally, it creates traffic by permanently synchronising your edits, which you cannot turn off in an online environment (consider also traffic by tracking, see below: Browsing). It also relies on a permanent internet connection (see above: Data Traffic). Depending on the type of information you need to communicate, it is advisable to opt for a light-weight tool (e.g. EtherPad) for taking collaborative notes.

**Browsing** on the Internet causes data traffic. As a general rule, more data privacy also means less data traffic. You can track your browsing footprint with the »[Carbonalyser](https://theshiftproject.org/en/carbonalyser-browser-extension/)« tool developed by the Shift Project to identify traffic-intense websites. A lot of traffic remains invisible to the user: ads, tracking and social media functions are being processed in the background (cf. https://whotracks.me/). It is possible to avoid some of this invisible traffic with browser extensions (AdBlockPlus, Ghostery, uBlockOrigin; for general advice see [WikiHow](https://www.wikihow.com/Prevent-People-from-Tracking-You-on-the-Internet)). 

**Editing documents locally** on your machine sometimes consumes unnecessary energy when additional features are running in the background of your program. For example, you can save energy by turning off automatic grammar/spell check (and activate it for final review of a document, for example). If your document is very large and you use cloud storage or a network drive, consider turning off the autosave function, or adjust it to a larger interval in order to reduce synchronisation traffic. Also check for further features in your text editor that may not be required to run all the time – essentially everything that checks the text permanently in the background and needs to go through large vocabularies.

**Videoconferencing** is less carbon intensive with cameras switched off. This is a complex area, however, since it relates to human sociality and connection. If we try to be too strict about seeing one another's faces online, could this start to impact our decisions to travel vs. working remotely? In the future, better data on the impact of work-related videoconferencing may help to decide whether this is a carbon-saving measure worth prioritising. For now, we recommend experimenting with a mixture of cameras on and cameras off, especially once working relationships are well-established. 


## How to communicate within your team

Communicating within your project team might include sending messages, sharing documents, or videoconferences. While the carbon footprint of the applications and software you will choose is a key element in making this decision, we have included a few additional criteria to help you balance pros and cons of the most frequently used software.



**Choosing a videoconference system**

*[start of zoom measurement/estimate info - need more samples and how to factor in multiple participants]*

| Software | Carbon footprint | Accessibility | GDPR compliance |
| --- | --- | --- | --- |
| Google Meet |     | Proprietary | Very nontransparent |
| Zoom |    | Proprietary | Very nontransparent |
| BBB |    | General Public Licence; needs to be installed and maintained on an institutional server | Transparent |
| Jitsi |    | Apache Licence | Mostly transparent     |
| Webex |    | Proprietary | Relatively transparent |
| MS Teams |    | Proprietary | Very nontransparent    |


**Choosing a Team-Chat Program**

| Software | Carbon footprint | Accessibility | Functions | Data privacy | Costs |
| --- | --- | --- | --- | --- | --- |
| Discord  |   | Runs on all major systems | Messaging, Audio and Video | Bad (Data is transmitted unencrypted and the company is allowed to read and resell the data. Data can be transmitted to US-Server) | No fees |
| Element  |   | Runs on all major systems; open-source (GitHub-repo); available in 25 languages | Messaging, Audio and Video (can be unstable) | End-to-end encryption; can be hosted on own server | No fees |
| Slack |   | Runs on all major systems; Available in 8 languages | Messaging, Audio and Video | Cloud-based (can be hacked); end-to-end encryption | Basic version without fees is normally sufficient |



If the online platform you are using declares its carbon or electricity efficiencies (and it’s likely that it does not) it will help you understand which factors use electricity when using the web service. The company’s data centre and where in the world it is located, how much data the service transmits to and from your network, how efficiently their (often proprietary) software is conceived, and the energy ratings of the computing device you use are all critical factors – and extremely difficult to find! 

## Publishing your data

In this area, the key is to take advantage of infrastructure that is used by as many people as possible in order to reduce the carbon footprint per capita. Ad-hoc, tailored solutions are the most resource-intensive and should be avoided where possible. 



**Making (primary) data available**

Humanities projects with a strong digital component usually include the production of primary data in their expected outputs (as detailed in their Data Management Plan), but research in general, even classical Humanities research without a strong digital component, combines and/or creates primary resources such as texts, images, video, and audio. The simple fact that your research project deals with a specific combination of sources, connected by the research question you work on, could make it worthwhile to present this data as a publication itself (within the framework of rights associated with the data). This type of publication can be included in your publication list or integrated into a data paper publication (on data papers, see [Schöpfel et al., 2019](https://halshs.archives-ouvertes.fr/halshs-02284548/document)). 

Primary data should be hosted in a stable, sustainable environment that will provide access and reuse (reuse is key here in terms of environmental footprint). Research, Teaching and Cultural Heritage Institutions usually provide in-house, state-of-the art solutions (such as nextcloud) on dedicated servers. In some countries (like in France), national infrastructures offer this type for services as well. You can also decide to use trusted repositories like github or zenodo. The key here is to avoid one-shot solutions and maximise mutualisations. This is also in general the best way to ensure multiple site archiving and hence making sure your data will not disappear in a server crash.



**Publishing your results**

Following up on the idea that mutualized infrastructure reduces the carbon footprint, the publication on massive preprint servers like [ArXiv ](https://arxiv.org/)or [HAL](https://hal.archives-ouvertes.fr/) presents an excellent ratio in terms of visibility/resource consumptions. Green Open Access is actually green (see [here](https://en.wikipedia.org/wiki/Open_access#Definitions) the difference between Green and Gold OA). Gold Open Access comes with a few caveats. First, like for any other website, the fancier the hosting, the more resource-intensive. Pop-ups, banners, pictures, videos on the publisher’s website are loaded every time the paper is accessed and generate a substantial CO2 footprint. What is more, a wide array of well-established publishers harvests researchers’ data ([data tracking](https://www.dfg.de/download/pdf/foerderung/programme/lis/datentracking_papier_en.pdf)), which is not only problematic in terms of data privacy, but also in terms of environmental impact that comes from harvesting, storing, and using the tracked data. 



**Communicating on social media**

| Software  | Environmental footprint (scrolling 1 minute in gEqCO”) | Energy consumption (1 minute, in mAh) | Data exchange (scrolling 1 minute in MB) |
| --- | --- | --- | --- |
| Twitter   | 0.60 | 10.28 | 6.28 |
| Instagram | 1.05 | 8.9 | 32.46 |
| Facebook  | 0.79 | 12.36 | 11.15 |
| TikTok    | 2.63 | 15.81 | 96.23 |


–> The footprint is smaller with fewer videos that play automatically.  

Src: https://greenspector.com/en/social-media-2021/

## Questions to keep in mind 

* How much electricity is needed to run the software?
* Is any special hardware needed that requires resources?
* How sustainable is the workflow process (concerning people-power)?
* Data privacy: Who hosts my data? On what conditions and legal restrictions? Who has access?
* Open source software: Who can use the software, how accessible is it?
* Do I need a lot of time to learn something new? Are there communities that can help me?
* Is the tool accessible for people with disabilities or people that speak different languages? 
  
## Travel {#travel}

Travel is a huge topic. There is plenty of guidance for academics out there, such as the [Flying Less in Academia Resource Guide](http://flyinglessresourceguide.info/). More resources are linked to below. The carbon cost of flying is notorious, so it is worth putting it in perspective: globally, flying makes a far smaller impact than agriculture and forestry, or heating and lighting buildings, or road transport. But it is not insignificant, and it is an area that is comparatively easy to cut down on. 

Moratoriums on non-essential travel can be a good way for an institution to show how serious they are on climate transition. The more boldly they define 'non-essential,' the more serious they are.

**Imagining new spatialities**

Climate transition does not have to be about self-denial. At best, it can be about transformative innovation that considers justice, inclusion and wellbeing alongside carbon impact. Reducing the amount we travel, and especially the amount we fly, is an opportunity to **reimagine the spatialities** of research and education. Who should travel, where, when, for how long, for what purposes? One approach might be to replace *all* travel with videoconferencing. Would this be a good idea? The Digital Humanities have a role to play in analysing the implications.

In the transition period of the early to mid 2020s, we recommend boldly cutting back on travel, while collaboratively exploring a longer run strategy. Together we should explore questions such as: What kinds of activity should be done in person, and what should be done remotely? For online and hybrid activities, what are the nuances of various digital tools and platforms? What should we make of Meta's Metaverse, and its relatively power-hungry attempt to create virtual alternatives to physical proximity? Might we invent entirely new formats and ways of working? Conferences, workshops, sandpits, seminars, events, meetings, fieldwork: how might these all be reimagined? 

**Flying Less**

[Flying Less in Academia Resource Guide](http://flyinglessresourceguide.info/), ed. Ryan Katz-Rosen, is a large curated reading list. There have been some recent breakthroughs in Sustainable Aviation Fuels (SAFs), so flying itself may arguably become greener in the future. But it's worth noting that these biofuels require large amounts of land which could otherwise be allocated to different mitigation or adaptation functions. Some other resources about flying include:

- Nevins, Joseph. 2014. ‘Academic Jet-Setting in a Time of Climate Destabilization: Ecological Privilege and Professional Geographic Travel’. The Professional Geographer 66, no. 2 (April 3, 2014): 298–310. [https://doi.org/10.1080/00330124.2013.784954](https://doi.org/10.1080/00330124.2013.784954).
- Sheller, Mimi. 2018. _Mobility Justice: The Politics of Movement in an Age of Extremes_. London: Verso.
- Nevins, Joseph, Stephen Allen and Matt Watson 2022.  ‘A path to decolonization? Reducing air travel and resource consumption in higher education’. Travel Behaviour and Society, Volume 26, January 2022, pp.231-239. [https://doi.org/10.1016/j.tbs.2021.09.012](https://doi.org/10.1016/j.tbs.2021.09.012)
- Glover, Andre, Yolande Strengers, and Tania Lewis. ‘The Unsustainability of Academic Aeromobility in Australian Universities.’ _Sustainability: Science, Practice and Policy_ 13, no. 1 (2017): 1–12. [https://doi.org/10.1080/15487733.2017.1388620](https://doi.org/10.1080/15487733.2017.1388620)

**Remote Working and 'Rebound Effects'**

- ‘Rebound effects’ include increased demand for energy caused by remote working which can erode (or even outweigh) savings from less commuting. A good overview is Hook, Andrew, Victor Court, Benjamin K. Sovacool, and Steve Sorrell. 2020. ‘A Systematic Review of the Energy and Climate Impacts of Teleworking’. _Environmental Research Letters_ 15 (9): 093003. [https://doi.org/10.1088/1748-9326/ab8a84](https://doi.org/10.1088/1748-9326/ab8a84).
- Here is a big EU report on teleworking: Samek Lodovic, Manuela et al. 2021. _[The Impact of Teleworking and Digital Work on Workers and Society](https://www.europarl.europa.eu/RegData/etudes/ATAG/2021/662907/IPOL_ATA(2021)662907_EN.pdf)_. Committee on Employment and Social Affairs, Policy Department for Economic, Scientific and Quality of Life Policies, European Parliament, Luxembourg.

**Slow Research, Slow Travel, Slow Scholarship, Slow Food**

- Conti, Meredith. ‘Slow Academic Travel: An Antidote to “Fly Over” Scholarship in the Age of Climate Crisis’, Theatre Topics 31.1 (2021): (https://muse.jhu.edu/article/786251)[https://muse.jhu.edu/article/786251]
- Mountz, Alison, et al. ‘For slow scholarship: A feminist politics of resistance through collective action in the neoliberal university’. ACME: An International Journal for Critical Geographies 14.4 (2015): 1235-1259. [https://acme-journal.org/index.php/acme/article/view/1058](https://acme-journal.org/index.php/acme/article/view/1058)
- Günel, Gökçe, Saiba Varma, and Chika Watanabe. “A Manifesto for Patchwork Ethnography.” Fieldsights, June 9, 2020. [https://culanth.org/fieldsights/a-manifesto-for-patchwork-ethnography](https://culanth.org/fieldsights/a-manifesto-for-patchwork-ethnography)
- Jungnickel, Katrina. “Getting There… and Back: How Ethnographic Commuting (by Bicycle) Shaped a Study of Australian Backyard Technologists.” Qualitative Research 14, no. 6 (December 1, 2014): 640–55. [https://doi.org/10.1177/1468794113481792](https://doi.org/10.1177/1468794113481792)
- ‘[Should I Attend the Conference? Air Travel Conference / Meeting Justification Tool](https://www.sustainabilityexchange.ac.uk/files/eauc-scotland_air_travel_justification_tool_version_2.pdf).’ A quiz, scorecard, and suggestions for how to interpret your scores.
- A blog post by Filip Vostal criticising slow scholarship: “Research in many disciplines needs to be in synch with the world it investigates; fast and slow again work together in a dialectical interplay here.” Vostal, Filip. 2021. ‘[Four Reasons Slow Scholarship Will Not Change Academia](https://blogs.lse.ac.uk/impactofsocialsciences/2021/05/11/four-reasons-slow-scholarship-will-not-change-academia/)’. Impact of Social Sciences (blog). 11 May 2021.

**From Research Trips to Research Voyages?**

Cutting down travel is obviously important. So too is making sure that when we _do_ travel, it really counts. We might cultivate the ideal of a 'research tour' or a **'research voyage'**. This kind of travel would be infrequent, would take the greenest available transport (e.g. rail), and would think about what the researcher can do along the way (not just at the destination).

Digital Humanities researchers can explore the practical challenges of this. For example, if archival visits were done in a more networked and collaborative way, a visiting researcher could conduct proxy research on behalf of others. Might we develop a platform to support this? Such a platform could have longer term ambitions too, helping universities and other institutions to share their resources to enable slower, more sustainable research trips. For example, might institutions form hospitality networks, to offer accommodation at a discount or for free, where travel is by the greenest available method?

**Conferences: Smaller, Online, Hybrid, Unconferences, Alternatives**

- [The Nearly Carbon Neutral](https://hiltner.english.ucsb.edu/index.php/ncnc-guide/) model suggests presenters pre-recording videos.
- Haage, Verena. 2020. ‘A Survey of Travel Behaviour among Scientists in Germany and the Potential for Change’. ELife 9 (May): e56765. [https://doi.org/10.7554/eLife.56765](https://doi.org/10.7554/eLife.56765).
- Pasek, Anne, Caleb Wellum, and Emily Roehl. ‘Making and Meeting Online: A White Paper on E-Conferences, Workshops, and other Experiments in Low-Carbon Research Exchange’. Petrocultures Research Group. [https://www.energyhumanities.ca/news/making-and-meeting-online](https://www.energyhumanities.ca/news/making-and-meeting-online)
- Bautista Perpinyà, Max. "Online conferences won’t do it. Instead of ‘sustainable’ academic history, we need engaged historians working less and collaborating with activists." Historians for the Future 18 November 2021. [https://historiansforfuture.org/online-conferences-wont-do-it/](https://historiansforfuture.org/online-conferences-wont-do-it/)
- Mead, Margaret, and Paul Byers. The Small Conference: An Innovation in Communication, 2015. [https://0-doi-org.pugwash.lib.warwick.ac.uk/10.1515/9783111559100](https://0-doi-org.pugwash.lib.warwick.ac.uk/10.1515/9783111559100)
- Sarabipour, Sarvenaz. “Evaluating features of scientific conferences: A call for improvements.” 21 April 2020. [https://www.biorxiv.org/content/biorxiv/early/2020/04/21/2020.04.02.022079.full.pdf](https://www.biorxiv.org/content/biorxiv/early/2020/04/21/2020.04.02.022079.full.pdf)
- Skiles, Matthew, Euijin Yang, Orad Reshef et al. "Conference Demographics and Footprint Changed by Virtual Platforms." Nature Sustainability (2021). [https://doi.org/10.1038/s41893-021-00823-2](https://doi.org/10.1038/s41893-021-00823-2)
- Svensson, Patrik. “Some Thoughts on Making Academic Events with Particular Attention to the Mid-Sized Event,” October 15, 2019. [http://patriksv.net/some-thoughts-on-making-academic-events/](http://patriksv.net/some-thoughts-on-making-academic-events/)

## Catering events

*Serve Plant-based Food*

- Dunne, Daisy. 2020. ‘[Interactive: What Is the Climate Impact of Eating Meat and Dairy?](https://interactive.carbonbrief.org/what-is-the-climate-impact-of-eating-meat-and-dairy/)’ Carbon Brief, 2020.
- Schiermeier, Quirin. 2019. ‘Eat Less Meat: UN Climate-Change Report Calls for Change to Human Diet’. Nature 572 (7769): 291–92. [https://doi.org/10.1038/d41586-019-02409-7](https://doi.org/10.1038/d41586-019-02409-7).

