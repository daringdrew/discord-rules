# discord-rules
Rules &amp; Info section

<!DOCTYPE html>
<html lang="en">

<head>
    <title>r/Avicii Archive ◢ ◤ - rules-and-info&#128203;</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">

    <style>
        /* General */

@font-face {
    font-family: Whitney;
    src: url(https://cdn.jsdelivr.net/gh/Tyrrrz/DiscordFonts@master/whitney-300.woff);
    font-weight: 300;
}

@font-face {
    font-family: Whitney;
    src: url(https://cdn.jsdelivr.net/gh/Tyrrrz/DiscordFonts@master/whitney-400.woff);
    font-weight: 400;
}

@font-face {
    font-family: Whitney;
    src: url(https://cdn.jsdelivr.net/gh/Tyrrrz/DiscordFonts@master/whitney-500.woff);
    font-weight: 500;
}

@font-face {
    font-family: Whitney;
    src: url(https://cdn.jsdelivr.net/gh/Tyrrrz/DiscordFonts@master/whitney-600.woff);
    font-weight: 600;
}

@font-face {
    font-family: Whitney;
    src: url(https://cdn.jsdelivr.net/gh/Tyrrrz/DiscordFonts@master/whitney-700.woff);
    font-weight: 700;
}

body {
    font-family: "Whitney", "Helvetica Neue", Helvetica, Arial, sans-serif;
    font-size: 17px;
}

a {
    text-decoration: none;
}

a:hover {
    text-decoration: underline;
}

img {
    object-fit: contain;
}

.markdown {
    max-width: 100%;
    line-height: 1.3;
    overflow-wrap: break-word;
}

.preserve-whitespace {
    white-space: pre-wrap;
}

.spoiler {
    /* width: fit-content; */
    display: inline-block;
    /* This is more consistent across browsers, the old attribute worked well under Chrome but not FireFox. */
}

.spoiler--hidden {
    cursor: pointer;
}

.spoiler-text {
    border-radius: 3px;
}

.spoiler--hidden .spoiler-text {
    color: rgba(0, 0, 0, 0);
}

.spoiler--hidden .spoiler-text::selection {
    color: rgba(0, 0, 0, 0);
}

.spoiler-image {
    position: relative;
    overflow: hidden;
    border-radius: 3px;
}

.spoiler--hidden .spoiler-image {
    box-shadow: 0 0 1px 1px rgba(0, 0, 0, 0.1);
}

.spoiler--hidden .spoiler-image * {
    filter: blur(44px);
}

.spoiler--hidden .spoiler-image:after {
    content: "SPOILER";
    color: #dcddde;
    background-color: rgba(0, 0, 0, 0.6);
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    font-weight: 600;
    padding: 100%;
    border-radius: 20px;
    letter-spacing: 0.05em;
    font-size: 0.9em;
}

.spoiler--hidden:hover .spoiler-image:after {
    color: #fff;
    background-color: rgba(0, 0, 0, 0.9);
}

.quote {
    margin: 0.1em 0;
    padding-left: 0.6em;
    border-left: 4px solid;
    border-radius: 3px;
}

.pre {
    font-family: "Consolas", "Courier New", Courier, monospace;
}

.pre--multiline {
    margin-top: 0.25em;
    padding: 0.5em;
    border: 2px solid;
    border-radius: 5px;
}

.pre--inline {
    padding: 2px;
    border-radius: 3px;
    font-size: 0.85em;
}

.mention {
    border-radius: 3px;
    padding: 0 2px;
    color: #7289da;
    background: rgba(114, 137, 218, .1);
    font-weight: 500;
}

.emoji {
    width: 1.25em;
    height: 1.25em;
    margin: 0 0.06em;
    vertical-align: -0.4em;
}

.emoji--small {
    width: 1em;
    height: 1em;
}

.emoji--large {
    width: 2.8em;
    height: 2.8em;
}

/* Preamble */

.preamble {
    display: grid;
    margin: 0 0.3em 0.6em 0.3em;
    max-width: 100%;
    grid-template-columns: auto 1fr;
}

.preamble__guild-icon-container {
    grid-column: 1;
}

.preamble__guild-icon {
    max-width: 88px;
    max-height: 88px;
}

.preamble__entries-container {
    grid-column: 2;
    margin-left: 0.6em;
}

.preamble__entry {
    font-size: 1.4em;
}

.preamble__entry--small {
    font-size: 1em;
}

/* Chatlog */

.chatlog {
    max-width: 100%;
}

.chatlog__message-group {
    display: grid;
    margin: 0 0.6em;
    padding: 0.9em 0;
    border-top: 1px solid;
    grid-template-columns: auto 1fr;
}

.chatlog__reference-symbol {
    grid-column: 1;
    border-style: solid;
    border-width: 2px 0 0 2px;
    border-radius: 8px 0 0 0;
    margin-left: 16px;
    margin-top: 8px;
}

.chatlog__reference {
    display: flex;
    grid-column: 2;
    margin-left: 1.2em;
    margin-bottom: 0.25em;
    font-size: 0.875em;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    align-items: center;
}

.chatlog__reference-avatar {
    border-radius: 50%;
    height: 16px;
    width: 16px;
    margin-right: 0.25em;
}

.chatlog__reference-name {
    margin-right: 0.25em;
    font-weight: 600;
}

.chatlog__reference-link {
    flex-grow: 1;
    overflow: hidden;
    text-overflow: ellipsis;
}

.chatlog__reference-link:hover {
    text-decoration: none;
}

.chatlog__reference-content > * {
    display: inline;
}

.chatlog__reference-edited-timestamp {
    margin-left: 0.25em;
    font-size: 0.8em;
}

.chatlog__author-avatar-container {
    grid-column: 1;
    width: 40px;
    height: 40px;
}

.chatlog__author-avatar {
    border-radius: 50%;
    height: 40px;
    width: 40px;
}

.chatlog__messages {
    grid-column: 2;
    margin-left: 1.2em;
    min-width: 50%;
}

.chatlog__author-name {
    font-weight: 500;
}

.chatlog__timestamp {
    margin-left: 0.3em;
    font-size: 0.75em;
}

.chatlog__message {
    padding: 0.1em 0.3em;
    margin: 0 -0.3em;
    background-color: transparent;
    transition: background-color 1s ease;
}

.chatlog__content {
    font-size: 0.95em;
    word-wrap: break-word;
}

.chatlog__edited-timestamp {
    margin-left: 0.15em;
    font-size: 0.8em;
}

.chatlog__attachment {
    margin-top: 0.3em;
}

.chatlog__attachment-thumbnail {
    vertical-align: top;
    max-width: 45vw;
    max-height: 500px;
    border-radius: 3px;
}

.chatlog__attachment-container {
    height: 40px;
    width: 100%;
    max-width: 520px;
    padding: 10px;
    border: 1px solid;
    border-radius: 3px;
    overflow: hidden;
}

.chatlog__attachment-icon {
    float: left;
    height: 100%;
    margin-right: 10px;
}

.chatlog__attachment-icon > .a {
    fill: #f4f5fb;
    d: path("M50,935a25,25,0,0,1-25-25V50A25,25,0,0,1,50,25H519.6L695,201.32V910a25,25,0,0,1-25,25Z");
}

.chatlog__attachment-icon > .b {
    fill: #7789c4;
    d: path("M509.21,50,670,211.63V910H50V50H509.21M530,0H50A50,50,0,0,0,0,50V910a50,50,0,0,0,50,50H670a50,50,0,0,0,50-50h0V191Z");
}

.chatlog__attachment-icon > .c {
    fill: #f4f5fb;
    d: path("M530,215a25,25,0,0,1-25-25V50a25,25,0,0,1,16.23-23.41L693.41,198.77A25,25,0,0,1,670,215Z");
}

.chatlog__attachment-icon > .d {
    fill: #7789c4;
    d: path("M530,70.71,649.29,190H530V70.71M530,0a50,50,0,0,0-50,50V190a50,50,0,0,0,50,50H670a50,50,0,0,0,50-50Z");
}

.chatlog__attachment-filesize {
    color: #72767d;
    font-size: 12px;
}

.chatlog__attachment-filename {
    overflow: hidden;
    white-space: nowrap;
    text-overflow: ellipsis;
}

.chatlog__embed {
    display: flex;
    margin-top: 0.3em;
    max-width: 520px;
}

.chatlog__embed-color-pill {
    flex-shrink: 0;
    width: 0.25em;
    border-top-left-radius: 3px;
    border-bottom-left-radius: 3px;
}

.chatlog__embed-content-container {
    display: flex;
    flex-direction: column;
    padding: 0.5em 0.6em;
    border: 1px solid;
    border-top-right-radius: 3px;
    border-bottom-right-radius: 3px;
}

.chatlog__embed-content {
    display: flex;
    width: 100%;
}

.chatlog__embed-text {
    flex: 1;
}

.chatlog__embed-author {
    display: flex;
    margin-bottom: 0.3em;
    align-items: center;
}

.chatlog__embed-author-icon {
    margin-right: 0.5em;
    width: 20px;
    height: 20px;
    border-radius: 50%;
}

.chatlog__embed-author-name {
    font-size: 0.875em;
    font-weight: 600;
}

.chatlog__embed-title {
    margin-bottom: 0.2em;
    font-size: 0.875em;
    font-weight: 600;
}

.chatlog__embed-description {
    font-weight: 500;
    font-size: 0.85em;
}

.chatlog__embed-fields {
    display: flex;
    flex-wrap: wrap;
}

.chatlog__embed-field {
    flex: 0;
    min-width: 100%;
    max-width: 506px;
    padding-top: 0.6em;
    font-size: 0.875em;
}

.chatlog__embed-field--inline {
    flex: 1;
    flex-basis: auto;
    min-width: 150px;
}

.chatlog__embed-field-name {
    margin-bottom: 0.2em;
    font-weight: 600;
}

.chatlog__embed-field-value {
    font-weight: 500;
}

.chatlog__embed-thumbnail {
    flex: 0;
    margin-left: 1.2em;
    max-width: 80px;
    max-height: 80px;
    border-radius: 3px;
}

.chatlog__embed-image-container {
    margin-top: 0.6em;
}

.chatlog__embed-image {
    max-width: 500px;
    max-height: 400px;
    border-radius: 3px;
}

.chatlog__embed-footer {
    margin-top: 0.6em;
}

.chatlog__embed-footer-icon {
    margin-right: 0.2em;
    width: 20px;
    height: 20px;
    border-radius: 50%;
    vertical-align: middle;
}

.chatlog__embed-footer-text {
    font-size: 0.75em;
    font-weight: 500;
}

.chatlog__reactions {
    display: flex;
}

.chatlog__reaction {
    display: flex;
    align-items: center;
    margin: 0.35em 0.1em 0.1em 0.1em;
    padding: 0.2em 0.35em;
    border-radius: 3px;
}

.chatlog__reaction-count {
    min-width: 9px;
    margin-left: 0.35em;
    font-size: 0.875em;
}

.chatlog__bot-tag {
    position: relative;
    top: -.2em;
    margin-left: 0.3em;
    padding: 0.05em 0.3em;
    border-radius: 3px;
    vertical-align: middle;
    line-height: 1.3;
    background: #7289da;
    color: #ffffff;
    font-size: 0.625em;
    font-weight: 500;
}

/* Postamble */

.postamble {
    margin: 1.4em 0.3em 0.6em 0.3em;
    padding: 1em;
    border-top: 1px solid;
}
    </style>
    <style>
        /* General */

body {
    background-color: #36393e;
    color: #dcddde;
}

a {
    color: #0096cf;
}

.spoiler-text {
    background-color: rgba(255, 255, 255, 0.1);
}

.spoiler--hidden .spoiler-text {
    background-color: #202225;
}

.spoiler--hidden:hover .spoiler-text {
    background-color: rgba(32, 34, 37, 0.8);
}

.quote {
    border-color: #4f545c;
}

.pre {
    background-color: #2f3136 !important;
}

.pre--multiline {
    border-color: #282b30 !important;
    color: #b9bbbe !important;
}

/* === Preamble === */

.preamble__entry {
    color: #ffffff;
}

/* Chatlog */

.chatlog__message-group {
    border-color: rgba(255, 255, 255, 0.1);
}

.chatlog__reference-symbol {
    border-color: #4f545c;
}

.chatlog__reference {
    color: #b5b6b8;
}

.chatlog__reference-link {
    color: #b5b6b8;
}

.chatlog__reference-link:hover {
    color: #ffffff;
}

.chatlog__reference-edited-timestamp {
    color: rgba(255, 255, 255, 0.2);
}

.chatlog__author-name {
    color: #ffffff;
}

.chatlog__timestamp {
    color: rgba(255, 255, 255, 0.2);
}

.chatlog__message--highlighted {
    background-color: rgba(114, 137, 218, 0.2) !important;
}

.chatlog__message--pinned {
    background-color: rgba(249, 168, 37, 0.05);
}

.chatlog__attachment-container {
    background-color: #2f3136;
    border-color: #292b2f;
}

.chatlog__edited-timestamp {
    color: rgba(255, 255, 255, 0.2);
}

.chatlog__embed-color-pill--default {
    background-color: rgba(79, 84, 92, 1);
}

.chatlog__embed-content-container {
    background-color: rgba(46, 48, 54, 0.3);
    border-color: rgba(46, 48, 54, 0.6);
}

.chatlog__embed-author-name {
    color: #ffffff;
}

.chatlog__embed-author-name-link {
    color: #ffffff;
}

.chatlog__embed-title {
    color: #ffffff;
}

.chatlog__embed-description {
    color: rgba(255, 255, 255, 0.6);
}

.chatlog__embed-field-name {
    color: #ffffff;
}

.chatlog__embed-field-value {
    color: rgba(255, 255, 255, 0.6);
}

.chatlog__embed-footer {
    color: rgba(255, 255, 255, 0.6);
}

.chatlog__reaction {
    background-color: rgba(255, 255, 255, 0.05);
}

.chatlog__reaction-count {
    color: rgba(255, 255, 255, 0.3);
}

/* Postamble */

.postamble {
    border-color: rgba(255, 255, 255, 0.1);
}

.postamble__entry {
    color: #ffffff;
}
    </style>

    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.15.6/styles/solarized-dark.min.css">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.15.6/highlight.min.js"></script>
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            document.querySelectorAll('.pre--multiline').forEach(block => hljs.highlightBlock(block));
        });
    </script>

    <script>
        function scrollToMessage(event, id) {
            var element = document.getElementById('message-' + id);

            if (element) {
                event.preventDefault();

                element.classList.add('chatlog__message--highlighted');

                window.scrollTo({
                    top: element.getBoundingClientRect().top - document.body.getBoundingClientRect().top - (window.innerHeight / 2),
                    behavior: 'smooth'
                });

                window.setTimeout(function() {
                    element.classList.remove('chatlog__message--highlighted');
                }, 2000);
            }
        }

        function showSpoiler(event, element) {
            if (element && element.classList.contains('spoiler--hidden')) {
                event.preventDefault();
                element.classList.remove('spoiler--hidden');
            }
        }
    </script>
</head>
<body>

<div class="preamble">
    <div class="preamble__guild-icon-container">
        <img class="preamble__guild-icon" src="https://cdn.discordapp.com/icons/346320975492808714/a_ec01f2088d2102c7aa6cfb48bdfbe37e.png" alt="Guild icon">
    </div>
    <div class="preamble__entries-container">
        <div class="preamble__entry">r/Avicii Archive ◢ ◤</div>
        <div class="preamble__entry">ℹnformation / rules-and-info&#128203;</div>


    </div>
</div>

<div class="chatlog">


<div class="chatlog__message-group">
    <div class="chatlog__author-avatar-container">
        <img class="chatlog__author-avatar" src="https://cdn.discordapp.com/avatars/165803649681850369/d1c3c86b71d36047b2466f8a55b9f69e.png" alt="Avatar">
    </div>
    <div class="chatlog__messages">
        <span class="chatlog__author-name" title="Ryuui#8715" data-user-id="165803649681850369" style="color: rgb(233,30,99)">Ryuui</span>


        <span class="chatlog__timestamp">2020-05-02 08:52 AM EST</span>

            <div class="chatlog__message " data-message-id="706125935455240292" id="message-706125935455240292">
                    <div class="chatlog__content">
                        <div class="markdown">
                            <span class="preserve-whitespace"><img class="emoji " alt="AvLogoWhite" title="AvLogoWhite" src="https://cdn.discordapp.com/emojis/585993217116209152.png"> <strong>Welcome to the Avicii Discord Server!</strong> <img class="emoji " alt="AvLogoBlack" title="AvLogoBlack" src="https://cdn.discordapp.com/emojis/460491329235845120.png">

<em>Please note that by joining this server, you put yourself at risk of exposure to leaks and all spoilers.</em>

We are a collection of all types of lovers and fans of Tim &#39;&#39;Avicii&#39;&#39; Bergling&#39;s music. From music production pros to DJs to outright music lovers we are all fans of Tim.

<u><strong>This server is to celebrate Tim&#39;s life.</strong></u>

Anything you want to talk about? We have a place to discuss anything regarding Avicii. <strong>Songs, Albums, Personal Stories, Remixes, Livesets, Everything!</strong></span>

                                <span class="chatlog__edited-timestamp" title="2020-05-05 07:19 PM EST">(edited)</span>
                        </div>
                    </div>



            </div>
            <div class="chatlog__message " data-message-id="706126282093625354" id="message-706126282093625354">
                    <div class="chatlog__content">
                        <div class="markdown">
                            <span class="preserve-whitespace"><u><strong>FAQs</strong></u> <img class="emoji " alt="timwave" title="timwave" src="https://cdn.discordapp.com/emojis/563453610692837376.png">


<img class="emoji " alt="AvLogoWhite" title="AvLogoWhite" src="https://cdn.discordapp.com/emojis/585993217116209152.png"> <strong>Why can’t I post Images/Files/Links? </strong><img class="emoji " alt="AvLogoBlack" title="AvLogoBlack" src="https://cdn.discordapp.com/emojis/460491329235845120.png"> 
We’re happy to see your images! But we have all image/file permissions restricted until you reach Le7el 5 <img class="emoji " alt="Le7els" title="Le7els" src="https://cdn.discordapp.com/emojis/638911766948216855.png">. This is to help us alleviate spam and unnecessary posts. You may ask an admin for a temporary bypass if you really want to share something.

The <span class="mention">#music-production&#127932;</span> channel is restricted to only allowing members with the Producer role to post files. Please assign a role by using <span class="mention">#assign-role</span>.

<img class="emoji " alt="AvLogoWhite" title="AvLogoWhite" src="https://cdn.discordapp.com/emojis/585993217116209152.png"> <strong>I have a suggestion. Where can I send it?</strong> <img class="emoji " alt="AvLogoBlack" title="AvLogoBlack" src="https://cdn.discordapp.com/emojis/460491329235845120.png"> 
Although we are not a large server, we are always looking to improve in places that people like. Send it to <span class="mention">#server-suggestions&#128161;</span>  and/or tag one of us <span class="mention" style="color: rgb(233, 30, 99); background-color: rgba(233, 30, 99, 0.1);">@Admin&#128081;</span>&#39;s

<img class="emoji " alt="AvLogoWhite" title="AvLogoWhite" src="https://cdn.discordapp.com/emojis/585993217116209152.png"> <strong>Where can I find the rules?</strong> <img class="emoji " alt="AvLogoBlack" title="AvLogoBlack" src="https://cdn.discordapp.com/emojis/460491329235845120.png"> 
⬇️ Rules are located below this post. ⬇️

▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬
Current Staff

   ◽  Founder: <span class="mention" title="Based Arab Oil God#2028">@Lamecat</span> 
   ◽  Owner: <span class="mention" title="JocKe#1117">@JocKe</span> 
   ◽  Moderation Team: <span class="mention" title="Ryuui#8715">@Ryuui</span> , <span class="mention" title="JocKe#1117">@JocKe</span></span>

                                <span class="chatlog__edited-timestamp" title="2020-05-05 07:18 PM EST">(edited)</span>
                        </div>
                    </div>



            </div>
            <div class="chatlog__message " data-message-id="706126675074875399" id="message-706126675074875399">
                    <div class="chatlog__content">
                        <div class="markdown">
                            <span class="preserve-whitespace">▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬

<u><strong>Server-Wide Rules</strong></u> 


<img class="emoji " alt="AvLogoWhite" title="AvLogoWhite" src="https://cdn.discordapp.com/emojis/585993217116209152.png"> <strong>Opinions are welcome, offensive conduct is not.</strong> <img class="emoji " alt="AvLogoBlack" title="AvLogoBlack" src="https://cdn.discordapp.com/emojis/460491329235845120.png"> 
All opinions are welcome, any offensive conduct is not. Keep it nice, keep it clean, and that&#39;s all that will be seen. Please do not report or downvote opinions you disagree with. Opposing opinions should be welcomed without hostility.

<img class="emoji " alt="AvLogoWhite" title="AvLogoWhite" src="https://cdn.discordapp.com/emojis/585993217116209152.png"> <strong>Be respectful of others.</strong> <img class="emoji " alt="AvLogoBlack" title="AvLogoBlack" src="https://cdn.discordapp.com/emojis/460491329235845120.png"> 
Treat others with kindness and be respectful. It&#39;s ok to disagree. We don’t take lightly to situations of excessive hostility, unfriendliness, bullying, or plain rudeness here. So don’t do it.

Please don&#39;t start or bring up any drama. Drama is not welcome here and will result in a mute, and if continued, a ban.
This goes for all channels. Please do not bring those opinions into the server.

<img class="emoji " alt="AvLogoWhite" title="AvLogoWhite" src="https://cdn.discordapp.com/emojis/585993217116209152.png"> <strong>No excessive self-promotion. (Advertising)</strong> <img class="emoji " alt="AvLogoBlack" title="AvLogoBlack" src="https://cdn.discordapp.com/emojis/460491329235845120.png"> 
Be mindful that although we are glad to see original content here, please do not flood the server with your personal website/YouTube channel. Once in a while is encouraged, just don&#39;t make it excessive.
Please contact an admin before posting a link to another Discord server.

<img class="emoji " alt="AvLogoWhite" title="AvLogoWhite" src="https://cdn.discordapp.com/emojis/585993217116209152.png"> <strong>Memes and shitposts are allowed. Spam + Cringe is not.</strong> <img class="emoji " alt="AvLogoBlack" title="AvLogoBlack" src="https://cdn.discordapp.com/emojis/460491329235845120.png"> 
Memes and shitposts are allowed. Since this is the internet, we get lots of unneeded content such as spamming the server and postings that can be very cringy content. Mods will determine when something is becoming excessive and will take action if necessary.</span>

                        </div>
                    </div>



            </div>
            <div class="chatlog__message " data-message-id="706126736135422003" id="message-706126736135422003">
                    <div class="chatlog__content">
                        <div class="markdown">
                            <span class="preserve-whitespace"><img class="emoji " alt="AvLogoWhite" title="AvLogoWhite" src="https://cdn.discordapp.com/emojis/585993217116209152.png"> <strong>Staff have final say.</strong> <img class="emoji " alt="AvLogoBlack" title="AvLogoBlack" src="https://cdn.discordapp.com/emojis/460491329235845120.png"> 
Staff can punish even if the offence isn&#39;t in the rules, as long as it is deemed fit. If you disagree with the punishment, DM a member of the leadership team or higher. If a staff member has reason to believe you should be punished, you will be punished. Anything you believe is not sensible, don’t do it.

<img class="emoji " alt="AvLogoWhite" title="AvLogoWhite" src="https://cdn.discordapp.com/emojis/585993217116209152.png"> <strong>WE DO NOT ADVOCATE PIRACY!</strong> <img class="emoji " alt="AvLogoBlack" title="AvLogoBlack" src="https://cdn.discordapp.com/emojis/460491329235845120.png"> 
Posting a link to a song or album download that could otherwise be purchased is unacceptable and will result in a ban without question or warning. Files of demos, unreleased song(s), leaks, snippets shall not be publicly posted here.
Trying to sell copies of unreleased songs online will result in an immediate ban.
In order to protect our members from any potential scams and frauds we do not allow any advertising or recruiting members for any outside activities (I.e. Groupbuys)

Trying to sell copies of unreleased songs online will result in an immediate ban.

<img class="emoji " alt="AvLogoWhite" title="AvLogoWhite" src="https://cdn.discordapp.com/emojis/585993217116209152.png"> <strong>Absolutely no violation of Discord Terms of Service (doxxing, file sharing, etc.) will be tolerated.</strong> <img class="emoji " alt="AvLogoBlack" title="AvLogoBlack" src="https://cdn.discordapp.com/emojis/460491329235845120.png"> 
It’s stated on their website, follow them. They are made to be followed.
<a href="https://discordapp.com/terms">https://discordapp.com/terms</a>
<a href="https://discordapp.com/guidelines">https://discordapp.com/guidelines</a>


▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬
Additional Information


<img class="emoji " alt="🔨" title="🔨" src="https://twemoji.maxcdn.com/2/72x72/1f528.png">   - Banned users wanting to appeal must do so via modmail ✉️ at <a href="https://www.reddit.com/message/compose?to=/r/Avicii">https://www.reddit.com/message/compose?to=/r/Avicii</a>

<img class="emoji " alt="🌎" title="🌎" src="https://twemoji.maxcdn.com/2/72x72/1f30e.png"> We have channels for users that want to speak/type in a different language.

Invite Users via: <a href="https://discord.gg/8F7PKcf">https://discord.gg/8F7PKcf</a></span>

                                <span class="chatlog__edited-timestamp" title="2020-05-02 10:58 AM EST">(edited)</span>
                        </div>
                    </div>



            </div>
    </div>
</div>

</div>

<div class="postamble">
    <div class="postamble__entry">Exported 4 message(s)</div>
</div>

</body>

</html>
