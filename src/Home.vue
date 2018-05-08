<template lang='pug'>
.frontpage(style="font-family: 'Roboto Condensed', sans-serif;")
  .top
  .content
    .centered.top-text
      h1 Phishing
      h2 Wes Jonas, Nicolette Lucido, Alex Mork, and Brett Stockglausner


    .thumbnails.centered
    .box-card(v-for='slideshow in slideshows')
      .caption.centered
        h3 {{slideshow.infos.title}}
      router-link(:to='slideshow.infos.path' @click.native="click")
        .embedded-slideshow-container
          component(:is="slideshow", :embedded='true',
          :keyboardNavigation='false',
          :mouseNavigation='false')

    h2 Executive Summary
    p.
      In a time when technology is constantly becoming more and more advanced,
      security should be at the top of the list of priorities for any company that
      utilizes any form of computer system and the internet, which in 2018 is virtually
      100% of all businesses. The risk associated with a lack of security depends on
      many things like the size of the business, and the importance of the information
      that they utilize and could be subject to a data breach. While you may think of
      information security and immediately jump to security flaws like flaws in a program,
      or rudimentary network protections, the biggest threat to any entity’s information
      security is actually the people who utilize the system. This doesn’t just include
      the people who carry out cyber attacks against a network, but in most cases is
      actually referring to the end users who end up becoming a security risk due to lack
      of knowledge about a system, and even plain ignorance. This can come in the form of
      not following company procedures, like locking a workstation when it’s unoccupied,
      or sharing passwords and other sensitive information. One of the most common ways
      that an employee can become a security risk is due to phishing emails. Even the
      best of employees at an organization could still be very susceptible to a phishing
      email due to how sophisticated they’ve become in recent years. Phishing is
      fraudulent emails sent to someone in hopes that they comply to whatever the email
      asks of them, in hopes to coerce them to divulge sensitive information, download
      a malicious attachment, or grant access to what should be a secure system.
      Companies have begun to catch onto this clever attack style, combatting it with
      simulated attacks and formal education to teach employees what to look out for,
      but alas, the threat persists, and is an ever evolving issue, which makes it that
      much more of a security risk to even the largest of corporations moving forward.

    h2 Introduction
    p.
      Information security is more than just various firewalls in place to keep attackers out of a company’s, or individual’s system. Humans are just as susceptible to attack as a machine, and if not properly educated, they can inadvertently cause just as much harm. Phishing is a method used by attackers, often through email, to gain access or information about a person, or an organization through seemingly legitimate messages. These messages can direct the victim to fake websites, ask them to install malicious software, or ask them to respond directly with information like usernames and passwords. For large companies, phishing scams can cost millions; this creates the need for education and security systems that are designed to help filter possible malicious mail.

    h2 Problem Statement
    p.
      In a society that is ever expanding and evolving into a more technology dependent world, cybersecurity is of the utmost importance. Cybersecurity encompasses all things related to the protection and preservation of assets and information that are connected to, and stored on the internet. One of the most common threats to information security in the corporate, and personal world is that of Phishing. Its’ ability to be utilized in many different ways makes it a threat that must be handled on all fronts, and must be seen as a top priority to combat in the world of information security.

    h2 Security Implications of Phishing (END USER FOLLY)
    p.
      Phishing may seem like a rather cut and dry security issue. End users receive an email, and whether or not they recognize the address of the sender, or regardless of what the email contains or references in the title line, their curiosity, or other external factor causes them to overlook skepticism and instead click on links, open up attachments, or comply in whatever other way the email asks them too. Phishing is a much more complex issue because it can be so difficult to spot, and can result in so many varying implications for a business unit, or network that it is afflicted by.

    h2 Different forms of phishing
    p.
      Phishing is so dangerous because of its level of unpredictability. It can hit at any point, and can show up in an infinite amount of different forms. The basics are simple, a malicious actor sends an email to an individual that in some way, shape, or form, gains access to their computer or obtains personal information. How they do this can vary greatly. In a business sense, an email can appear to be coming from a CEO, or other trusted official, asking for certain confidential documents to be sent in return. An unsuspecting employee may see this email and act without haste to appease the needs of whatever other employee is requesting the item. Unfortunately, modern technology can allow someone to “spoof” or fake their name or email address, which can be used to trick someone into complying, even though they aren’t who they say they are.
    p.
      A research study conducted in 2017 by KnowBe4 aimed to find the subject lines in phishing emails that most commonly resulted in someone being successfully phished. They used a real business, and sent out mock phishing emails to the employees. The ones included all made it through spam filters on employee emails, and resulted in the following statistics.
    .block(style="margin-left: 10%")
      p Security Alert – 21%
      p Revised Vacation & Sick Time Policy – 14%
      p UPS Label Delivery 1ZBE312TNY00015011 – 10%
      p BREAKING: United Airlines Passenger Dies from Brain Hemorrhage – VIDEO – 10%
      p A Delivery Attempt was made – 10%
      p All Employees: Update your Healthcare Info – 9%
      p Change of Password Required Immediately – 8%
      p Password Check Required Immediately – 7%
      p Unusual sign-in activity – 6%
      p Urgent Action Required – 6%

    p.
      What this research proves is that phishing emails have the advantage of being able to take on many forms. Phishing emails have gained so much sophistication in such a short amount of time. Those “Nigerian Prince” emails everyone used to talk about, where someone would receive an email claiming to be from an international person, who for some ridiculous and outlandish reason, wanted to send a crazy amount of money to you for safe keeping. These were phishing emails. While they may seem childishly simple to see through, some users simply seem to not be able to resist the possibility of coming into such fortune randomly. Since this point, phishing has become a much more far reaching security threat. Attackers will design elaborate emails that look to be coming from trusted and reputable brands, or even an email that looks like it comes from someone inside of your company’s network. All of these attempts have one thing in common. They all are wanting to persuade you to comply with whatever it asks. Whether that be clicking on a link provided, downloading an attached file, or sending back private information to the requesting party. This level of variance in the world of phishing is what causes it to be such a serious issue.

    h2 Current Approaches
    p.
      Companies with a high value on their information security are already taking steps to combat phishing in many different ways. While 100% security is not considered to be a possibility in a realistic setting, minimizing the risk of a security breach or an attack on a network does help to keep security at a rather high level, and keep daily operations running smoothly. Some companies, such as Emerson, go as far to have an entire department dedicated to security awareness and prevention of future security risks. These “awareness teams” play a crucial role in teaching employees how to conduct themselves in the workplace which in turn can lead to less risk for information breaches. These teams may focus on things like content creation, where they create physical and visual aids such as posters and handouts that explain the risks associated with different security threats like Phishing.
    p.
      These materials may be distributed or posted in places where they are visible to employees, or in places around an office where they’re more relevant (i.e. a poster next to a set of cubicles that reminds employees to lock their computer when they leave their workstation, which helps to cut down on unsecure nodes that could be utilized for malicious intent). While making security awareness visible to employees, and using this visual aids as constant reminders to how they can be practicing good information security policies is important, as the old saying goes, practice makes perfect. For this reason, companies of all structures and sizes have begun leveraging the use of phishing simulations or “mock phishing” to combat the ever growing threat of employees who can't differentiate a legitimate email from a fraudulent one, and end up clicking on a malicious link, or divulging sensitive personal, or confidential information to an attacker, who could then use that information against the user, or the entire company based on its severity. In a mock phishing campaign, a phishing email template is designed, much like in a real phishing situation, and is strategically made to try and trick the recipient into clicking on the link. The desired outcome is that either they see this email and realize it’s probably phishing, and it reminds them how to conduct themselves when viewing emails in the future, or if they do click on it, the experience can serve as a valuable lesson on what not to do, without the repercussions of clicking on an actual phishing email.

    h2 How Does a Breach Take Place from a Technical Standpoint
    p
      i “How harmful can one of these “phishing emails” truly be? All you have to do is not click on it and just delete it.”
    p.
      Phishing has grown in its sophistication and implementation. Phishing emails of the past were rudimentary, and easy to spot. Now days they can be very similar to an email you may expect to receive from your favorite online retailers like Amazon, or an email that looks identical to your bank statement. When a user receives an email that looks like something they’re used to, and seems to be coming from a familiar source, they’re more apt to trust it and click away. Unfortunately, the other end of that link that claims to direct users to an exclusive product offer or shipping invoice that needs to be approved may actually be a link that downloads malicious software. Other phishing emails ask for a user to comply by giving out sensitive personal or enterprise information. In both cases, the end result is not acceptable. Login credentials that are leaked via coercion can be used to gain unauthorized access into a system or program, which could lead to huge financial and reputational implications. Getting access into a system may also give a hacker the ability to implement some form of malware to bring down, or take control of a piece of the network.
    p.
      On the other end, a malicious link or attachment could cause the system to download a worm with a malicious payload. Infecting the initial node within the network could create a foothold that an attacker could use to infect the rest of the network as well but utilizing a worm to replicate and spread its payload throughout the entire enterprise network. There’s no static template for using phishing against people, meaning that malicious actors can create incredibly realistic and diverse phishing emails that may be very difficult to detect, even for someone who knows the telltale signs to look for. This dimension of adaptability doesn’t just mean that the phishing attempt is harder to recognize. It also means that attackers can tailor them to the audience which they are trying to attack, in hopes to make them more successful due to susceptibility, or the content that is regarded in the phony email. Imagine getting an email that claims to be from a superior, asking you to review the attached document, and claims that they’ll be calling you in 15 minutes to discuss its contents. The average user will see this is an urgent matter, and immediately open the attachment without thinking. “But how is this possible? If it’s coming from their email address, it has to actually be them!”. Unfortunately it’s not that simple. Typosquatting is a technique used by hackers to trick you into believing the validity of the person sending an email to you.
    p.
    .block(style="margin-left: 10%")
      p EmilyJackson@Email.com
      p ErnilyJackson@Email.com
      p Emliy.Jackson@Email.com
      p EmilyJackson@Ernail.com
    p.
      At a quick glance, this may look like the same email listed 4 times, but in reality each one is actually slightly different than the rest. This psychological lapse in judgement that causes us to trust what we are relatively familiar with can be exploited to make us believe the legitimacy of a phishing email. Since Phishing is merely a medium with which malicious actors use to gain access into a system, or network (and in some cases, gain direct information), The list of possibilities regarding the implications of each different attack, and their severities is virtually limitless. It is for this reason that all phishing related threats must be handled with the utmost priority, because in some cases, it may only take one to cripple an entire operation.
    p.
      Since phishing is such a dynamic, and widespread threat, it does not have a set technical diagram of how it targets and infects a system. Phishing can be carried out on a widespread company scope, in hopes to just fool as many employees as possible, no matter their level within the organization, allowing access into a network. Another form called Spear Phishing is more targeted to a smaller group, usually higher level officials or CEOs. These phishing emails will likely be more sophisticated, and probably personally tailored to make them as believable as possible to each individual. However, no matter the type of phishing, or the targeted system or information, simply put, phishing is the process of using fraudulent emails to persuade individuals into complying with whatever is asked of them. Phishing is a textbook example of social engineering.

    h2 Innovative Approaches to Creating User Awareness
    p.
      In an industry such as technology, and information security, innovation and evolution of processes, and procedures is tantamount to staying competitive against all of the cyber threats in the world. As we’ve previously discussed, there’s no such thing as perfect information security, and hackers are tirelessly searching for the newest way around the latest security upgrades. Companies have begun to realize just how important data security is, even if they’re not a technology company directly, we are living in a time in which essentially all companies, and people across the entire world are affected by it in some form or fashion. Simulated phishing has become a very popular tactic to inform and educate employees of what they should be looking out for in regards to phishing attempts. These mock phishing campaigns are run through in-house, or 3rd party programs and allow companies to test their employees susceptibility to different types of phishing.
    p.
      This form of training is usually coupled with a more orthodox training module that may include videos, quizzes, etc. which aim to instill long term knowledge about phishing and how to prevent becoming a victim of it to all employees. While education is an absolute must, and is certainly argued as the most effective way to combat phishing, companies also leverage different filters and security measures to seek out potential phishing emails and other malicious content from ever making it into the inboxes of their employees. These programs are able to scan contents of an email, including attachments, to attempt to determine whether or not it could be risky to open it. This helps to cut down on the likelihood of a system being infected by simply reducing the amount of malicious content to begin with. Unfortunately, these can cost a lot of money to utilize, or man hours to create in-house, so they are typically only utilized by larger organizations that may also hold a higher risk of being targeted for phishing attacks.
    p.
      When a company utilizes their own phishing campaign, the scope of the campaign is very important. Sending an email to as many employees as possible across the company will generate the best results for future educational sessions. HR is most commonly the department associated with creating and sending the fake phishing emails. There is more than just making a suspicious email and sending it; to be able to gather data that can be used later to educate, HR needs to create a system that will report back various information. Valuable information collected would include the number of times a link was clicked, and the amount of reports of phishing filed. To ensure the highest awareness of phishing company wide, repeating this campaign monthly or quarterly is important; but just as important is changing the form of attack. After a few fake emails, many employees will catch on to scheme and will know which emails are intended for training purposes; rather distribute different types of phishing attacks: links, attachments, fake websites requesting usernames and passwords, and requests to download potentially harmful applications. Making the attacks seem as real as possible makes for a real challenge when it can be identical to an email that the department of specific employee might receive. Just as important as the content of a phishing attack, the recipients of the attack are also important. Managers and other “high ups” receive large amounts of emails per day potentially making them an even larger target for phishing attacks. Along with receiving more emails, managers also are more likely to be holding more sensitive information. Promoting positivity after each campaign and educating more on the importance of security will create a more serious environment for the employees. Employees who feel rewarded for their actions are more likely to repeat those actions of reporting suspicious emails.
    p.
      One company that is offering third-party service for phishing education and software for a company to use is KnowBe4. They are a company that helps you train your employees on the importance of spam, phishing, spear phishing, malware, ransomware, and social engineering. Their point is to prove to companies that they can have the best technology to filter out as many threats that it can, but the company needs to build up their “human firewall”, or their employees. Their training programs start with a baseline test, to see where you currently stand with the company’s human firewall. Then you train the employees in the company, and then put them through the test with automated phishing attacks. These attacks are crucial in helping the employees see real world examples of what these attacks can look like. Then with the results, the company can see what they need to educate more on and what areas the employees are susceptible to. This cycle continues as often that the company wants to keep their employees on their toes, because security needs to be in every employee’s mind when thinking about what to click and what not to click.
    p.
      KnowBe4 posts their quarterly test results of the top-clicked phishing tests. The company uses the data collected from the companies that use their services to get a more accurate, wide spread test results from what was clicked by employees. From all the tests run by their customers, the results are as followed for their Q1 from 2018.
    .block(style="margin-left: 10%")
      p LinkedIn related subject lines - 45%
      p Tagged Photo on Facebook - 15%
      p Password Change on Facebook - 14%
      p Login Alert - 13%
      p New Voice Message - 8%
    p.
      In the results, KnowBe4 details out that under LinkedIn the subjects lines were, “Add Me”, “Join Network”, “Reset Password”, and “New Message”. The main plot for these types of emails are to make people feel important or alarmed, which makes them more likely to click on the links/emails. This information is important to keep track of. People actually trying to hack can come up with some clever subject lines, and interesting ways to get employees to click on them. But it is important to companies to see not only what the general population is falling for, but more specifically what their company’s employees are falling for. Companies need to tailor their fake attacks to what they think their employees will click on and to show them what they fell for and what they need to work on.

    h2 Conclusion
    p.
      Phishing is becoming a very diverse and hard to spot form of attack. Malicious emails can be made to look and sound identical to one that is real but have very different results. Detection for even those who know what to look for can often be very difficult. The most important thing that can be done to help identify if an email is legitimate or not, is to determine that the email is in fact from the person it is claiming to be from. To do this, even if the email is marked urgent, to take a step back and verify that there are no slight changes to the email. By taking 10 second to do this, an employee can potentially save their company both time and money.
    p.
      Cybersecurity is a an extremely important aspect to every business, regardless of number of employees. One misconceptions that companies make when it comes to cybersecurity, is that the only thing you need to protect your company and employees from phishing plots is a really good software. Software that filters through emails can only do so much when it comes to protection. Attackers will continue to come up with creative ways to get around software. KnowBe4 call the employees for a company their “human firewall”. It is a fitting name, because employees are arguably the most import aspect when trying to combat phishing plots. Training and education is the key to making sure a company has a strong human firewall.
    p
    h2 References

    .references
      div
        p KnowBe4. “Kevin Mitnick Security Awareness Training.” KnowBe4. 2016.
        a(href="https://www.knowbe4.com/products/kevin-mitnick-security-awareness-training/") www.knowbe4.com/products/kevin-mitnick-security-awareness-training/.
      div
        p Morgan, Steve. “Top 10 Phishing Email Subject Lines That Launch Ransomware.” CSO Online. InfoWorld. 18 July 2017.
        a(href="https://www.csoonline.com/article/3209086/phishing/top-10-phishing-email-subjuect-lines-that-launch-ronasomware.html") www.csoonline.com/article/3209086/phishing/top-10-phishing-email-subjuect-lines-that-launch-ronasomware.html.
      div
        p Sjouwerman, Stu. “Q1 2018 Top Clicked Phishing Emails Subjects [INFOGRAPHIC].” Blog. 4 May 2018.
        a(href="https://blog.knowbe4.com/q1-2018-top-clicked-phishing-email-subjects") blog.knowbe4.com/q1-2018-top-clicked-phishing-email-subjects.
      div
        p Wattman, Kathy. “KnowBe4 Releases Quarterly Top-Clicked Phishing Report for Q2 2017.” PRWeb, 12 July 2017.
        a(href="http://www.prweb.com/releases/2017/prweb14499138.htm") www.prweb.com/releases/2017/prweb14499138.htm.
</template>

<script>
import slideshows from 'slideshows/slideshows'

export default {
  data: function () {
    return {
      slideshows: slideshows.list
    }
  },
  mounted: function () {
    console.log(this.slideshows)
    document.currentSlide = {}
  },
  methods: {
    click: function (evt) {
      evt.stopPropagation()
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss' scoped>
/*@import "node_modules/eagle.js/src/themes/frontpage/frontpage";*/
.eg-slide {
  width: 25%;
  height: 25%;
}
.graph-container {
  display: flex;
  width: 100%;
  height: 100%;
  flex-direction: column;
  overflow: hidden;
}
.graph {
  min-width: 100%;
  min-height: 550px;
  flex-grow: 1;
  border: none;
  margin: 0 auto;
  padding: 0;
}
.embedded-slideshow-container {
  position: relative;
  width: 150px;
  height: 120px;
  margin: 0 auto;
  overflow: hidden;
  border: solid 1px rgba(30, 30, 30, 0.1);
}
  .eg-theme-agrume embedded-slideshow {
    font-size: 4.8px;
    visibility: visible;
  }
  .eg-slideshow {
    margin-top: 0;
    background-color: black;
    background-attachment: fixed;
    position: absolute;
    height: 100%;
    width: 100%;
    overflow: hidden;
  }
  .content {
    width:60%;
    margin: 0 auto;
    z-index: 999;
    position: relative;
  }

  .centered {
    z-index: -1;
    margin: 0 auto;
    text-align: center;
  }
  .top {
    min-width: 100%;
    min-height: 250px;
    background: #42a4d2;
    position: relative;
    margin-top:-250px;
    z-index: 0;
    top: 250px;
    box-shadow: 0px -15px 25px 15px #2c3e50;
    border-bottom: solid 1px rgba(30, 30, 30, 0.1);
  }
  .top-text{
    h1 {
      font-size: 45px;
    }
    color: #eeeeee;
  }

  html body {
    height: 100%;
    width: 100%;
    margin: 0;
    padding: 0;
  }

  .references {
    div {
      margin-bottom: 40px;
    }
  }
  .frontpage {

  }
</style>
