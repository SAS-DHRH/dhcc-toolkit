---
title: "Minimal computing"
date: 2022-05-17
draft: false
weight: 2
slug: 'minimal-computing'
---

# Minimal computing  {#2-minimal-computing}

{{< hint info >}}
_‘We use “minimal computing” to refer to computing done under some set of significant constraints of hardware, software, education, network capacity, power, **or other factors**.’_

[GO:DH Minimal Computing group](https://go-dh.github.io/mincomp/about/)
{{< /hint >}}


{{< hint info >}}
_As a society we need to start treating computational resources as finite and precious, to be utilised only when necessary, and as effectively as possible. We need frugal computing: achieving the same results for less energy._

[Wim Vanderbauwhede](https://wimvanderbauwhede.github.io/articles/frugal-computing/)
{{< /hint >}}


{{< hint info >}}
_‘Digital technology has ushered in an age of inconspicuous consumption. It is easy to understand the environmental impact of buying 'stuff' or flying across the Atlantic. It is harder to wrap your head around how much energy it takes to fly data across the web.’_

[Arwa Mahdawi, The Guardian](https://www.theguardian.com/commentisfree/2020/feb/12/real-problem-netflix-addiction-arbon-emissions)
{{< /hint >}}


What can researchers do to resist techno-utopian, carbon-intensive technological traps? How can we support environmentally responsible design—even if software filled with cool unnecessary features may forever tug on our heartstrings? **Minimal computing** has at least some of the answers.

Minimal computing is a set of practices that aims to reduce both environmental impact and barriers to access and engagement. It offers an important set of thinking tools to make responsible, frugal, and nuanced digital decisions. As [Jentery Sayers](https://go-dh.github.io/mincomp/thoughts/2016/10/02/minimal-definitions/) has written:

> a minimal approach reduces the need for not only substantial storage and processing power but also a reliance on middleware, databases, peripherals, and substantial pieces of hardware. Such reduction should increase access while decreasing technology’s environmental effects (e.g., by reducing waste and energy consumption).

The label ‘low tech’ or ‘frugal’ does not mean unsophisticated—it means efficient and more accessible. By sharing content without bells and whistles (such as software dependencies that the content doesn’t really need), minimalist approaches offer a better chance that content will be accessible to most users. Low-tech solutions can significantly reduce data transfer in comparison to regular, database-driven websites. As Tim Frick has said, bad UX design is not just bad for users, it trashes the planet (see Frick’s book _[Designing for Sustainability](https://www.oreilly.com/library/view/designing-for-sustainability/9781491935767/)_, 2016).

Since 2016, when the first Minimal Computing in DH workshop was held at the [Digital Humanities ’16 conference](https://dh2016.adho.org/workshops/index.html), the constraints in which we conduct research have changed. There is now an urgent need to address the environmental consequences of digital technologies. This constraint has been growing for many decades, and is now a top priority out of necessity – we have procrastinated as a species and our paper was due yesterday!

Our aim here is not to give black-and-white instructions. Oftentimes there is not one right answer for computing solutions, and one downside of minimal computing, as Quinn Dombrowski has pointed out, is that it can be labour-intensive. Rather, by having a sense of the carbon cost of different methods of data modelling and web design, we are more able to make informed and proportional choices to suit our needs.



## Static versus dynamic websites {#static-versus-dynamic-websites}

A static website has fixed content which appears the same to every user (until it is manually updated). A dynamic website is generated “on the fly” and is more associated with interactivity. Social media sites are dynamic websites, since they are woven together from a variety of user generated content. More technically:

* A **dynamic** site uses server-side programming languages and technologies to pull information from a database and show it on your browser. All project data and content is stored in a content management system (CMS), which allows for bespoke, personalised, and automated changes to websites. Dynamic sites tend to be content-heavy and user-driven (that is to say the users are interacting with the content in specific ways).
* A **static** site consists of a directory of files that lives on the server. This means that when you are accessing web content, you are directly accessing a file in the site directory rather than making a request to a database or CMS for content. Pages are therefore accessed as-is, and changes need to be made page-by-page (unlike dynamic sites).
* A **hybrid** web site uses both elements of dynamic and static content.


*Why might you choose one or the other (or both)?*

There are good reasons to create dynamic websites, but a lot of scholarly projects will do just fine with static sites. Most of us are simply trying to communicate information on our websites: blogs, portfolios, project websites, magazines, documentation sites all can be made cheaply and hassle-free with static site generators. For example, if you are putting your CV online, you do not need a WordPress site to do that well. Static site generators, such as [Hugo](https://gohugo.io/), even have excellent themes (e.g. [Academic](https://themes.gohugo.io/themes/hugo-academic/)) for creating content such as CVs. If you have a collection of transcribed manuscripts, you can also publish that as a static site. Dynamic sites work better and are more appropriate for more complex projects that have interactive features like [API](https://en.wikipedia.org/wiki/API)s, search engines, data visualisations and other structured information stored in databases. That said, even a hybrid site that mixes some dynamic and static content will reduce its carbon impact.

*Although, it’s a little more complicated*

The benefit from a static site is a little more blurred nowadays, because of the way data gets cached. Browsers store certain data to speed up repeat visits. The browser may send the website an ETag to quickly check if a piece of content has changed. If not, it uses its cached copy. Service providers have similar caching techniques. This means it is not always clear what parts of your backend infrastructure are being hit when you use a dynamic site. A good proportion of the content might actually already be stored on your device.


### Static site generators and minimal Content Management Systems {#static-site-generators-and-minimal-content-management-systems}

Use a static site where possible. You can do so using a **static site generator** such as [Jekyll](https://jekyllrb.com/) or [Hugo](https://gohugo.io/).
- Jekyll has a longer history but also has more dependencies (it relies on [Ruby on Rails](https://rubyonrails.org/)).
- Hugo, which runs on the Go programming language, has fewer dependencies and attractive templates (this tool-kit runs on Hugo, by the way). Another good option is [GitHub Pages](https://pages.github.com/), and there are [many more](https://github.com/myles/awesome-static-generators).

If you are accustomed to building websites with tools like SquareSpace, Wix, or Wordpress, there may be a bit of a learning curve. But it is probably not as steep as it looks, and well worth investing the time.

For those of you who are creating **digital collections**, consider also using a stripped-down digital collection platform. Many people use [Omeka](https://omeka.org/) or [Drupal](https://www.drupal.org/), but consider using instead the [Wax platform](https://minicomp.github.io/wax/), which is 'producing digital exhibitions focused on longevity, low costs, and flexibility'.

Static sites won’t be suitable for everything. A **content management system** (CMS) is a tool that helps you create a dynamic website without coding. WordPress and Drupal are well-known examples, but there are lightweight alternatives you can use instead:

* [Strapi](https://strapi.io/): An open-source modern [headless CMS](https://www.contentful.com/r/knowledgebase/what-is-headless-cms/) alternative to WordPress.
* [Ghost](https://ghost.org/): A lightweight headless CMS designed for content creators.
* [Gatsby](https://www.gatsbyjs.com/): Good for single-page layouts, landing pages, web applications, portfolios, and institutional websites.
* [Mukurtu](https://mukurtu.org/): A grassroots CMS project aiming to empower communities to manage, share, narrate, and exchange their digital heritage in culturally relevant and ethically-minded ways.


## Tips for creating sustainable websites {#tips-for-creating-sustainable-websites}


{{< hint warning >}}
**Minimal web design for absolute beginners**

* Use fewer videos and images. Make the ones you do use really count!
* Shrink your images using a tool like [Squoosh](https://squoosh.app/).
* Use the newer WebP image format (instead of JPEG or PNG).
* Create an attractive, accessible design that favours dark colours. On [some screen types](https://www.wholegraindigital.com/blog/dark-colour-web-design/) they use less energy.
* Do some research and try to pick a green hosting provider. The [Green Web Foundation’s directory](https://www.thegreenwebfoundation.org/directory/) is one useful resource.
* Use a tool such as [Ecograder](https://ecograder.com/) to see the carbon impact of your site, and learn more about unnecessary elements (e.g. unused Javascript).

{{< /hint >}}


### Images and Lazy Loading {#images-and-lazy-loading}

According to [HTTP Archive](https://httparchive.org/reports/state-of-images), images constitute 50% of the average web page size. [WebP](https://en.wikipedia.org/wiki/WebP) instead of JPEG or PNG can [reduce file size by 25-35%](https://web.dev/serve-images-webp/) while increasing page speed performance. Switching icons and logos to SVG format can also significantly reduce page weight.

Enabling [lazy loading](https://developer.mozilla.org/en-US/docs/Web/Performance/Lazy_loading) will optimise image and video content. Instead of loading all of the page’s resources simultaneously, the browser only loads what’s above the fold and then fetches additional images and thumbnails as the user scrolls.


### Minify HTML and CSS or normalize space {#minify-html-and-css-or-normalize-space}

‘Minifying’ is a process of removing unnecessary whitespace, reducing file sizes, and increasing page speed. Most text editors have plug-ins or packages to minify code (see e.g. [Sublime text minify](https://packagecontrol.io/packages/Minify) and [Atom minify](https://atom.io/packages/atom-minify)). If you’re using XSLT, then use the `normalize-space()` function. E.g.


```
<xsl:template match="text()">
<xsl:value-of select="normalize-space(.)"/>
</xsl:template>
```



### Fonts {#fonts}

Your site’s font can actually have a carbon impact and affect [accessibility](https://usabilitygeek.com/10-free-web-based-web-site-accessibility-evaluation-tools/). For example, lightweight sans serif fonts such as Trebuchet are not only good for people with disabilities but they have less ‘weight’ (less tails and flourishes) and therefore require fewer pixels to be displayed. Verdana is also good because it is set wider than most fonts (making it more legible without adding weight). Use one of <span style="text-decoration:underline;">18 [web-safe fonts](https://blog.hubspot.com/website/web-safe-html-css-fonts)</span> to make the content compatible with all browsers and screen readers.


### Consider Mobile-First Design {#consider-mobile-first-design}

Many users throughout the world access internet content through mobile phones, so a mobile-friendly design ensures more access as well as a lightweight design. Loading an image or watching a video on a phone uses less energy than on a great big screen.


### Reduce client-side features (i.e. JavaScript)

Web pages need to load, and they can be loaded just once, but when you implement user interaction features, JavaScript continuously runs in the background. For example, it’s now very common for sites to have [parallax scrolling](https://www.youtube.com/watch?v=uTIzW5fZn_4) that redraws the screen when you scroll down the page, but this means that the web page must continuously consume energy on the device.


### Hosting {#hosting}

The Green Web Foundation has a [hosting directory](https://www.thegreenwebfoundation.org/directory/) of hundreds of green hosting providers across dozens of countries. In the UK, [Kualo](https://www.kualo.co.uk/webhosting/green-web-hosting) is a very good option.


## Applying Minimal Computing principles {#applying-minimal-computing-principles}

[Sayers (2016)](https://go-dh.github.io/mincomp/thoughts/2016/10/02/minimal-definitions/) notes how a minimal approach can create complex questions and trade-offs. To work in minimal ways means “to define, often implicitly, what and for whom ‘excess’ and ‘essential’ mean in the first place.” For example, it may be important “to share the mess of development with others, and minimalist aesthetics may all too easily afford an impression that everything has been polished or refined from the start.”

Here are some ways you might apply minimal computing principles in service of environmental sustainability. For the full list of Minimal principles, see Jentery Sayers’s ‘[Minimal Definitions](https://go-dh.github.io/mincomp/thoughts/2016/10/02/minimal-definitions/)’ (2016) at the Minimal Computing GO::DH site.

**Minimal languages.** Using an efficient programming language can improve environmental impacts.  If you have the liberty to make the language decision for yourself, there is some literature about the ecological impacts of these choices. How much energy, time and memory these languages require play an important role here. Humanities researchers often default to high level scripting languages, such as Python (perhaps they are easier for our humanist brains to understand). However, there are consequences for not thinking critically about our choice of programming languages.

Python, the go-to language of choice for many Digital Humanities researchers, can be observed in the following table (Pereira_ _et. al. 2017) comparing the energy and time factors of Python. Note that ‘time’ in this context means compute time, which is the time the computer takes to run the scripts, and not the time it takes to learn to write the language (although learning time is an important cost of labour factor, it is not a direct environmental factor of _computational_ research activity):


![alt_text](images/image1.png "image_tooltip")


_Energy Efficiency across Programming Languages (Pereira et. al. 2017)._

**Minimal design**

Specifying full minimal stack containers/machines.

**Minimal consumption**

* Serverless instances which only consume compute time on demand. However, these require an understanding of the research and technical side to coordinate and operate.
* Shared libraries at the operating system levels, between the disk sharing and network sharing all add costs. The big providers use lots of memory, which is cheaper than hitting disk, but the consequence is you need big hardware and large scale data centres.

**Minimal maintenance**

- Why are you still running it?

- On demand infrastructure.

- Creating cost models

- Infrastructure is declared - a knowledge system to load the YAML file into to get your emissions costs back would be great - instead of the calculators.

- Get the ICT service catalogue to update with emissions/costs.



* Minimal barriers, Minimal internet, Minimal externals, Minimal automation, Minimal space,

**Minimal ephemerality, Minimal visibility**

* Maximum access, Maximum accessibility, Maximum impact, Maximum mobility, Maximising your resource

## Minimal computing, critical design, and system change

Joana Moll’s project _[The Hidden Life of an Amazon User](https://www.janavirgin.com/AMZ/amazon.html)_ seeks to make visible the huge amount of code involved in making one simple purchase from Amazon:


> In order to purchase the book, the Amazon website forces the customer to go through twelve different interfaces composed of large amounts of code, which is normally invisible to the average user. This code carries out all sorts of operations, such as organizing and styling the site’s content, allowing interactivity, and recording the user’s activity. Overall, I was able to track 1,307 different requests to all sort of scripts and documents, totaling 8,724 A4 pages worth of printed code, adding up to 87.33MB of information. The amount of energy needed to load each of the twelve web interfaces, along with each one’s endless fragments of code, was approximately 30 wh. ([Moll 2019](https://www.janavirgin.com/AMZ/))

Do we really have to burn coal so that every user can get personalised recommendations whether they want them or not? Yet these maximalist approaches are pervasive. This means minimal computing can sometimes feel like fighting a losing battle. So how do we also work toward larger structural change? We need to do two things:



* Adopt and promote **behaviour change** (such as minimal computing), and
* advocate for **deeper structural changes** to support those changes in the longer term.

Although the first point is vital, on its own it is not enough. E.g. a review of interventions at the household level concludes that: “taken in isolation, behavioural interventions have a very small positive effect on climate change mitigation behaviours while the intervention is in place. Once the intervention stops, there is no evidence that such interventions produce lasting positive changes” (Nisa et al., 2019). Rather, lasting positive changes come when there are structures that support and encourage them.

The design of technological interfaces and systems, where the human meets the machine, are among the structures that must change. So are cultural norms, the rules and norms of communities and organisations, and legal and economic structures. So we might think of the link between Minimal computing and system change as a series of opportunities:



* When a user behaviour is wasteful, there is an opportunity to transform that behaviour.
* When a user behaviour resists transformation, there is an opportunity to redesign the technical environment.
* When a technical environment resists transformation, it is an opportunity to redesign the institutional environment.
* Whenever the institutional environment resists transformation, it is an opportunity to push for deeper legal and economic changes.

In this way, the everyday use of digital systems (for research and other purposes) reveals an abundance of research questions, data gaps, design challenges, exercises you might set your students, opportunities for technological innovation or entrepreneurship, as well as ways to focus and refine advocacy and activism for deeper system change. See “Advocating Within Your Institution” for further ideas.


## Minimal computing case studies

{{< hint info >}}
* _[Low-tech Magazine](https://www.lowtechmagazine.com/)_: This magazine runs a static website on a solar panel. In 2018, they outlined how they built a low-carbon website, ‘[How to Build a Low-tech Website?](https://www.lowtechmagazine.com/2018/09/how-to-build-a-lowtech-website.html)’ which offers some practical suggestions for digital publishing.
* [Solar Protocol](http://solarprotocol.net/): A platform of small solar-powered servers across different global locations. “The network routes internet traffic according to the logic of the sun, where page requests are sent to whichever server is enjoying the most sunlight at the time.”
* [Making and Knowing Project](https://www.makingandknowing.org/): this project published a static digital critical edition of [BnF MS Fr. 640](https://edition640.makingandknowing.org/#/), which uses minimal computing principles. See the ‘[Digital Development](https://edition640.makingandknowing.org/#/content/about)’ section of the site for more information.
* [Herman Melville Electronic Library](https://melville.electroniclibrary.org/): This project is a good example of a hybrid site; it has minimised its dependencies by hosting most of its web components on a static Jekyll site served through GitHub and Netlify, but it also has a bespoke dynamic tool called [TextLab](https://melville.electroniclibrary.org/textlab.html) rendered through Heroku app. For more information on this process, see [this seminar recording](https://www.youtube.com/watch?v=c0B5RFAjsi0&list=PLSTJ8CQ1p25BM4NF249Gy2ImFKCnKG2ft).
* [Fast Familiar](https://workroom.fastfamiliar.com/we-made-our-first-carbon-neutral-project/) are a group of artists creating socially and environmentally inclusive artworks and projects. They have written blog posts detailing how they have improved the carbon consumption of their website and projects: ‘[We Made Our First Carbon Neutral Project](https://workroom.fastfamiliar.com/we-made-our-first-carbon-neutral-project/)’ and ‘[How We Made Our Website Use 50% Less Energy](https://workroom.fastfamiliar.com/how-we-made-our-website-use-50-less-energy/).’

{{< /hint >}}


## Further reading on Minimal Computing

_[Digital Humanities Quarterly](http://digitalhumanities.org/dhq/)_ cluster on minimal computing, forthcoming.

Pasek, Anne and Benedetta Piantella. July 2021. [Solar-Powered Media](http://lowcarbonmethods.com/local/zine.html).

De Decker, Kris. “[How to Build a Low-tech Website](https://solar.lowtechmagazine.com/2018/09/how-to-build-a-lowtech-website.html).” _Low Tech Magazine_, 24 September 2018,

Frick, Tim. _Designing for Sustainability_, O’Reilly, 2016. [https://www.oreilly.com/library/view/designing-for-sustainability/9781491935767/](https://www.oreilly.com/library/view/designing-for-sustainability/9781491935767/).

GO::DH Minimal Computing Working Group ‘Thought Pieces’. [https://go-dh.github.io/mincomp/thoughts/](https://go-dh.github.io/mincomp/thoughts/).

Jarrett, Tom. “Designing Sustainable Interaction Design Principles.” Branch Magazine, 15 October 2020, [https://branch.climateaction.tech/2020/10/15/designing-branch-sustainable-interaction-design-principles/](https://branch.climateaction.tech/2020/10/15/designing-branch-sustainable-interaction-design-principles/).

Piantella, Benedetta, Alex Nathanson, Tega Brain, and Keita Ohshiro. ‘Solar-Powered Server: Designing for a More Energy Positive Internet’. 2020 CHI Conference on Human Factors in Computing Systems. New York, NY, USA: Association for Computing Machinery, 2020. [https://doi.org/10.1145/3334480.3383155](https://doi.org/10.1145/3334480.3383155).

Roscam Abbing, Roel. ‘“[This Is a Solar-Powered Website, Which Means It Sometimes Goes Offline”: A Design Inquiry into Degrowth and ICT](https://computingwithinlimits.org/2021/papers/limits21-abbing.pdf)’. In LIMITS’21: Workshop on Computing within Limits, June 14–15, 2021.

Pereira, Rui, Marco Couto, Francisco Ribeiro, Rui Rua, Jácome Cunha, João Paulo Fernandes, and João Saraiva. ‘Energy Efficiency across Programming Languages: How Do Energy, Time, and Memory Relate?’ In _Proceedings of the 10th ACM SIGPLAN International Conference on Software Language Engineering_, 256–67. Vancouver BC Canada: ACM, 2017. [https://doi.org/10.1145/3136014.3136031](https://doi.org/10.1145/3136014.3136031).
