Listen to a podcast about Transitioning from Hand-Coding to Web Content Authoring &amp; Google Sites

# Podcast Transcript: Web Content Authoring & Google Sites

Duration 17:11 · Host 1 and Host 2

**[00:00] Host 1:** Welcome to today's Deep Dive. You know, you spend months learning HTML, CSS, and JavaScript.

**[00:05] Host 2:** Yeah, wrestling with divs and margins.

**[00:07] Host 1:** Right, exactly. You painstakingly build your first web pages from scratch, just making sure your scripts actually fire. But then you look at a massive dynamic website out in the real world.

**[00:16] Host 2:** And a stark realization hits you.

**[00:18] Host 1:** Totally. You realize there is absolutely no way human beings are manually typing out raw code every single time they need to publish a blog post or, you know, update a calendar.

**[00:27] Host 2:** It's a sobering moment for any developer, really. I mean, you learn the foundational languages, which gives you this incredible power over the browser.

**[00:34] Host 1:** Yeah, absolute control.

**[00:35] Host 2:** But then you immediately run into the problem of scale. Hand coding every single page update is simply not a sustainable business model for content-heavy sites.

**[00:44] Host 1:** So today, our mission for this deep dive is to explore the architecture of how the web actually scales.

**[00:49] Host 2:** Right, we are looking at the transition from the nitty-gritty of hand coding into the highly visual, streamlined world of web content authoring.

**[00:57] Host 1:** Specifically, we're looking under the hood of website builders like Google Sites. And just to set the tone right up front, this isn't a debate about which method is objectively better or some purist argument about real coders.

**[01:08] Host 2:** No, not at all. It's about architecture. It's about you knowing exactly which tool to pull from your tool belt, depending on the specific job requirements.

**[01:17] Host 1:** Because if you are building a quick community hub or a simple portfolio, your architectural needs are vastly different than if you're building a bespoke web app with complex data routing.

**[01:27] Host 2:** Exactly. And this deep dive is about giving you the framework to analyze those requirements and make a confident choice.

**[01:33] Host 1:** Okay, let's unpack this. As someone who is used to living in VS Code, giving up access to my style sheet and the raw DOM feels like a massive leap of faith.

**[01:43] Host 2:** Oh, absolutely. When you move into a WYSIWYG environment…

**[01:46] Host 1:** Where you're basically trading your text editor for a visual interface.

**[01:50] Host 2:** Right. You have to fundamentally change how you think about constructing a page. You are no longer a coder in that environment. You are a content author.

**[01:59] Host 1:** And the technical philosophy driving the shift is an extreme separation of concerns.

**[02:04] Host 2:** Exactly. Hand coding is like building a house completely from scratch. You're mixing your own concrete. You're running the wiring yourself.

**[02:12] Host 1:** But web authoring is like moving into a pre-built house where you just choose the paint colors and arrange the furniture.

**[02:17] Host 2:** That's a perfect way to look at it. In a builder like Google Sites, the content, so your text, the raw image files, the video links, it's kept completely hermetically sealed away from the design layer.

**[02:29] Host 1:** Right, which is essentially the golden rule of CSS anyway, right? Keep your styling logic in one document and your structural HTML in another.

**[02:36] Host 2:** Yes. Website builders are just taking that exact same philosophy and abstracting it so far up that you, the user, never even see the brackets.

**[02:44] Host 1:** You just swap the theme and everything changes.

**[02:46] Host 2:** What's fascinating here is how that abstraction completely redefines user roles. Because the styling is handled by a globally applied template, you don't need to know how to write CSS to change the look of the site.

**[02:58] Host 1:** So you can just hand over the keys to a marketing team or a copywriter.

**[03:01] Host 2:** Precisely. Instead of managing server access and deployment pipelines, you're simply managing permissions. Owners who control the domain, editors who manipulate the content, and viewers who consume it.

**[03:14] Host 1:** I see the appeal for a team environment, definitely, but I have to push back a little on the execution here.

**[03:20] Host 2:** Sure, go on.

**[03:20] Host 1:** If the tool is silently writing all the HTML and perfectly formatting the CSS variables in the background, doesn't that make the process entirely frictionless?

**[03:30] Host 2:** Yes, it does.

**[03:31] Host 1:** And isn't friction sometimes a good thing? Like, it stops us from making terrible design choices. If the tool does all the heavy lifting, is it really that easy to mess up?

**[03:40] Host 2:** You've hit on the exact paradox of website builders. That frictionless environment is precisely what makes it so easy to create a structural disaster.

**[03:48] Host 1:** Because there's no code to slow you down.

**[03:50] Host 2:** Right. When you hand code a page, the sheer effort required to write the HTML, link the style sheets, and test the layout forces you to stop and ask, "Do I really need this page?"

**[04:01] Host 1:** But in a builder, you can just spawn 10 new pages in 10 seconds.

**[04:04] Host 2:** And suddenly you have a bloated labyrinthine site with a navigation menu that requires a map and compass to get through.

**[04:10] Host 1:** Yeah, that makes perfect sense. Because builders abstract the code away and make adding pages so incredibly easy, it creates a new problem, the temptation to just start clicking.

**[04:19] Host 2:** Exactly. The lack of technical friction means that rigorous, analog planning — literally drawing a site map on paper before you ever open the software — is actually more critical when using a builder than when hand coding.

**[04:31] Host 1:** You have to draw the blueprint yourself, because the tool won't stop you from building a house with 15 bathrooms and no front door.

**[04:37] Host 2:** That's spot on. You have to intentionally design constraints for yourself. For instance, limiting your main navigation menu to about 5-7 essential items.

**[04:45] Host 1:** Which is deeply rooted in human psychology, right? Working memory can only hold so many discrete items at once.

**[04:51] Host 2:** Right. If your navigation menu has 20 links, you aren't providing options, you're inducing cognitive overload.

**[04:58] Host 1:** And this ties directly into how you have to adapt your writing style for the web too. People do not read web pages like they read a novel.

**[05:05] Host 2:** No, they scan them. They scan in an F-shaped pattern, looking for keywords that match their intent.

**[05:11] Host 1:** Yes. The temptation in a builder is to just drop a massive text box onto the page and paste in a thousand word essay.

**[05:17] Host 2:** Which is a huge mistake.

**[05:19] Host 1:** Because users scan, you have to invert your writing style. You put the core conclusion in the very first sentence.

**[05:25] Host 2:** And keep your paragraphs ruthlessly short.

**[05:28] Host 1:** Like two to four sentences max.

**[05:30] Host 2:** Right? Use plain language.

**[05:32] Host 1:** You are optimizing for rapid information retrieval, not narrative flow.

**[05:36] Host 2:** And optimizing for retrieval brings us to a critical, often overlooked aspect of planning, hyperlink architecture. There is a strict rule in web authoring against ever using the phrase "click here" as your link text.

**[05:48] Host 1:** Oh, this is a huge pet peeve of mine, and it goes way beyond just bad aesthetics.

**[05:53] Host 2:** It really does.

**[05:54] Host 1:** If you just write "click here" for a link, think about the underlying HTML mechanics and how an assistive device interprets them.

**[06:01] Host 2:** A screen reader doesn't just read the page top to bottom.

**[06:04] Host 1:** Exactly. A user can command it to pull up an array of all the anchor tags on that page so they can navigate quickly.

**[06:09] Host 2:** And if it parses those anchor tags, and the inner text just says, click here, click here, click here.

**[06:15] Host 1:** The user receives a disconnected list of identical commands with zero context about the destination. It renders the entire navigation tree useless.

**[06:23] Host 2:** You have to write contextually meaningful text like ""View our 2027 product catalog"" and that exact same logic applies to how you handle images during the blueprint phase too.

**[06:34] Host 1:** Image rules are so important.

**[06:36] Host 2:** Image rules. A common mistake is designing a beautiful promotional poster in Photoshop complete with event dates and locations and just uploading that single JPEG to the builder.

**[06:46] Host 1:** Which is a massive architectural failure.

**[06:49] Host 2:** You've trapped crucial textual data inside a raster graphic.

**[06:53] Host 1:** It can't be resized. It can't be searched.

**[06:56] Host 2:** Right? A search engine scraper can't parse those pixels to index your event. A user on a phone can't highlight the address to copy it. And a screen reader just sees an image file with no readable nodes.

**[07:06] Host 1:** So assuming you've done this rigorous planning, you have a lean site map, scannable text, contextual links, and isolated visual assets, you finally open the Google Sites editor. And the way it translates your actions into code is actually quite elegant. I was looking at the structure of a Google Sites page, and instead of the basic layer cake analogy they usually teach beginners, it really operates as a visual wrapper for CSS Flexbox and Grid.

**[07:30] Host 2:** It really does. You start with a header component at the top, but the core of the page is built using what they call sections.

**[07:36] Host 1:** And those sections are essentially flex containers stacked vertically.

**[07:40] Host 2:** Exactly. You drop a section onto the page and then within that section you apply a layout.

**[07:46] Host 1:** Which acts like a predefined CSS grid template, maybe a three column or a two column asymmetrical split.

**[07:52] Host 2:** Right, and finally you insert your items, the actual text nodes and image tags, into those grid tracks.

**[07:58] Host 1:** The interface is doing all the math for the flex spaces and grid template columns in the background. It continuously adjusts the breakpoints for mobile, tablet, and desktop views automatically.

**[08:07] Host 2:** It completely removes the mathematical headache of responsive design. To manipulate this DOM, you really only manage three core panels on the side. Insert, pages, and themes.

**[08:18] Host 1:** Insert is your element toolbox, pages is where you manage your routing, and themes is your global CSS control panel. Changing a theme changes every page instantly.

**[08:27] Host 2:** It's incredibly fast. But because it's a dynamic system connected to a cloud backend, that creates a new bottleneck that catches a lot of the developers off guard.

**[08:36] Host 1:** The caching and versioning system.

**[08:37] Host 2:** Specifically the massive difference between your private draft and the live published state.

**[08:43] Host 1:** It's a fundamental concept in web authoring. What you see in the WYSIWYG editor is a localized private draft. It is not connected to the public-facing URL. Visitors only see the published version.

**[08:54] Host 2:** Yes, they are being served a cached version of the site from the exact timestamp of when you last pressed the publish button.

**[09:01] Host 1:** Which means if you spend four hours perfectly tweaking a layout and then just close your browser tab…

**[09:07] Host 2:** Those changes exist in the database, but they are invisible to the world.

**[09:11] Host 1:** You have to remember to click Publish. And once you do hit Publish, we have to talk about how the internet actually routes traffic to that layout.

**[09:18] Host 2:** Right, the web addresses. By default, a platform like Google Sites provisions a free subdomain URL for you.

**[09:24] Host 1:** Like sites.google.com/view/ your site name.

**[09:29] Host 2:** It's functional, routing through their DNS, but it's long and clearly flags the site as a free hosted project.

**[09:37] Host 1:** Which is totally fine if you're building an internal wiki for your dev team. But if you're launching a startup, you need a custom domain.

**[09:44] Host 2:** And here is where the platform abstraction breaks down a little. Because only the site owner can connect that custom domain. And you actually have to interface with external registrars and manage DNS records.

**[09:56] Host 1:** It's also vital to understand the illusion of privacy once that domain goes live. There's a vital warning here about privacy in search engines.

**[10:04] Host 2:** Oh absolutely. Google Sites offers a toggle switch asking public search engines not to index your site. But we have to be clear, asking them not to show your site is purely a request.

**[10:16] Host 1:** It is not a guarantee. It's a please keep off the grass sign, not a 10 foot concrete wall.

**[10:21] Host 2:** Exactly. The tool will not protect private info like phone numbers or addresses if you make the site public. Malicious scrapers might still index it.

**[10:29] Host 1:** So what does this all mean? We've established that website builders handle the responsive math, they abstract away the server maintenance, and they allow non-technical teams to publish content instantly.

**[10:39] Host 2:** It's incredibly efficient.

**[10:41] Host 1:** It begs a very pragmatic question for anyone listening. If they're this fast, why would anyone ever willingly choose to hand code a project again? Do builders make us lose too much control?

**[10:52] Host 2:** When you analyze enterprise-level workflows, the decision between hand coding and using a builder boils down to three core pillars, maintenance, collaboration, and portability.

**[11:02] Host 1:** Okay, let's look at collaboration first. Hand coding with multiple authors requires Git.

**[11:07] Host 2:** Right, it's highly technical. You need everyone to understand branching strategies, you need to resolve merge conflicts when two people edit the same file. It's complex code skills.

**[11:16] Host 1:** It's an entire ecosystem of tooling just to allow two people to type at the same time.

**[11:20] Host 2:** But with a platform like Google Sites, collaboration operates exactly like a Google Doc. You just share an editor link. Multiple stakeholders can manipulate the visual DOM simultaneously. The friction is zero.

**[11:31] Host 1:** But that massive advantage demands a heavy toll when it comes to portability. Hand-coded sites offer ultimate architectural freedom. They are easy to move, you just copy the HTML files to a new host.

**[11:43] Host 2:** Yes, your source code belongs to you, but website builders fundamentally lock you in.

**[11:48] Host 1:** You cannot export a Google site as a directory of raw, ready-to-host HTML files.

**[11:53] Host 2:** Exactly. The data is bound to their proprietary database. If you decide to migrate away in three years, you aren't moving files, you are starting over from scratch.

**[12:02] Host 1:** Our sources actually highlight a brilliant practical example to weigh these trade-offs. Take a local [unclear] office.

**[12:07] Host 2:** Right, great scenario.

**[12:08] Host 1:** They need a simple webpage for weekly public health announcements. The person updating it is a municipal clerk with zero coding skills.

**[12:16] Host 2:** In that scenario, a website builder is the optimal architectural choice. The zero friction collaboration outweighs the lock-in effect.

**[12:23] Host 1:** But let's pivot the requirements.

**[12:24] Host 2:** What if that same municipal office needs a custom database search for local property records or special layouts? Or what if they are legally mandated to meet strict federal web accessibility standards, requiring absolute control over the DOM?

**[12:39] Host 1:** In that case, they must hand code. Here's where it gets really interesting because there is a massive misconception in the industry regarding automated tools.

**[12:49] Host 2:** Oh, the accessibility misconception.

**[12:51] Host 1:** Yes, people assume that because a massive tech company built the platform, it automatically makes your website fully accessible.

**[12:58] Host 2:** If we connect this to the bigger picture, it goes back to the difference between a tool's capabilities and its implementation. A builder provides an interface with accessibility features, yes…

**[13:09] Host 1:** But the author is entirely responsible for using them.

**[13:11] Host 2:** Exactly. And more critically, because the builder obscures the raw HTML, you lose the ability to manually intervene when the automated code fails. You cannot add custom ARIA attributes.

**[13:23] Host 1:** You can't just open the inspector, find a broken div, and fix the underlying code issues. You are entirely at the mercy of whatever markup the platform spits out.

**[13:32] Host 2:** Which means, as a content author, your vigilance has to be significantly higher. Our sources outline some very strict do's and don'ts for authoring in this environment.

**[13:41] Host 1:** All right, like the do's. You absolutely must add alt text to all informative images, and that includes background banners and hero images.

**[13:50] Host 2:** You also have to enforce semantic heading structures. You have to use real heading styles in order, not just making text big and bold.

**[13:57] Host 1:** Visually it might look like a header, but structurally the screen reader just sees a paragraph. You also need to check contrast and provide transcripts for video embeds.

**[14:08] Host 2:** But then there are the specific don'ts, particularly the limitations in Google Sites. For example, avoid embedding dynamic charts directly from Google Sheets.

**[14:17] Host 1:** Because they have no alt text option. You're flying blind for any user relying on an assistive device.

**[14:23] Host 2:** You have to engineer a workaround, like exporting it as a static PNG. Also be aware that buttons in Google Sites are frequently parsed by screen readers simply as links.

**[14:33] Host 1:** Oh, so if the button just says "Submit" without clear context, it creates severe navigation confusion.

**[14:39] Host 2:** Exactly. And avoid collapsible text panels, those accordion menus.

**[14:44] Host 1:** Why are those bad?

**[14:45] Host 2:** The JavaScript handling them often fails to dynamically update the attributes, so a screen reader may not know if the panel is open or closed.

**[14:52] Host 1:** Leaving the user completely guessing. What about carousels or automated slideshows?

**[14:57] Host 2:** Avoid them entirely. They are notoriously hard to navigate with the keyboard. Users get stuck endlessly cycling through hidden image panels.

**[15:05] Host 1:** So the final verdict on accessibility really forces your hand architecturally. If a project requires strict adherence to accessibility standards, hand-coding gives the necessary control.

**[15:15] Host 2:** Yes. Builders are fine for smaller projects provided the author is highly vigilant about these specific limits.

**[15:22] Host 1:** Well, to briefly recap our journey today, we've seen how web authoring separates content from design.

**[15:28] Host 2:** And the absolute necessity of rigorous planning before you start clicking.

**[15:32] Host 1:** We covered the mechanics and trade-offs of Google Sites and the vital role of the human author in maintaining accessibility.

**[15:38] Host 2:** It's a profound shift in mindset.

**[15:40] Host 1:** It really is. I mean, remind yourself, you aren't just coders or content editors anymore. You are web architects.

**[15:47] Host 2:** You have a complete toolkit now.

**[15:49] Host 1:** Exactly. You know exactly when to pour the concrete yourself and when to use a pre-built frame. It's empowering.

**[15:55] Host 2:** It is. Though, looking at the trajectory of these tools, it does introduce a final, highly provocative thought to mull over.

**[16:02] Host 1:** Oh, lay it on me.

**[16:03] Host 2:** If website builders currently limit our ability to fix underlying accessibility code and hand coding offers ultimate control, what happens when automated AI-driven builders become so advanced that their underlying code generation is completely flawless and universally accessible?

**[16:22] Host 1:** Wait, like the machine writes better, more accessible DOM structures than a human ever could?

**[16:28] Host 2:** Exactly. Will the act of hand coding HTML eventually become a lost art? Will it transition from a foundational web skill into something practiced only by a hyper specialized few?

**[16:40] Host 1:** Oh wow, much like writing assembly languages today.

**[16:43] Host 2:** Precisely.

**[16:45] Host 1:** That is an incredible thought to end on. We might literally be watching the slow transition of HTML from a daily tool into an ancient specialized craft. Definitely something to mull over or explore on your own as you architect your next project.

**[16:59] Host 2:** Whether you are opening VS Code or dragging a layout onto a visual canvas.

**[17:04] Host 1:** Thank you so much for joining us on this deep dive. Keep exploring, keep questioning the tools you use, and we will catch you next time.
