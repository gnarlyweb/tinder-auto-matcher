
<body data-images="true" data-mode="solarized-dark" data-font="sans-serif" data-loaded="true" style="">

  <a id="reader-domain" href="https://gnarlyweb.github.io/tinder-auto-matcher/">
    <span>gnarlyweb.github.io</span>
    
    <span>/tinder-auto-matcher/</span>
    
  </a>
  <h1 dir="auto" id="reader-title">Tinder Auto-Matcher</h1>
  <div dir="auto" id="reader-credits"></div>
  <div dir="auto" id="reader-estimated-time">2-2 minutes</div>
  <hr>
  <div id="readability-page-1" class="page"><div>
        

<p><img src="https://user-images.githubusercontent.com/9092290/68415516-d6463600-0192-11ea-9820-ba391e4582f3.png"></p>

<h2 id="overview">Overview</h2>
<p>The goal of Tinder Auto-Matcher is to dehumanize as much as it can social interactions. This is achieved by automatically
liking back people who liked you Tinder to create a match without having to swipe one second. The next step would be to
send you an email everyday with recapitulation of today’s matches.</p>

<h2 id="usage">Usage</h2>
<ul>
  <li>First you need your Tinder’s authentication token. Log in to <a href="https://tinder.com/">tinder.com</a>, open the developer console, type <code data-beeline-skip="true">localStorage.getItem("TinderWeb/APIToken")</code> and save the returned value.</li>
  <li>Write the <em>X-Auth-Token</em> value in the token key in Tinder.AutoMatcher/appsettings.json.</li>
  <li>Install <a href="https://dotnet.microsoft.com/download">.NET Core SDK 3.X</a>.</li>
  <li>Finally, <code data-beeline-skip="true">dotnet run -p Tinder.AutoMatcher</code> to launch the worker.</li>
</ul>

<h2 id="how-does-it-work">How does it work?</h2>
<p>Tinder has a section where one can see the blurred pictures of the people who liked you.
To see the real profiles, you have to get Tinder Gold.</p>
<p><img src="https://user-images.githubusercontent.com/9092290/68415518-d6463600-0192-11ea-8c1e-be4a3e32d021.jpg"></p>

<p>However the Tinder API send unblurred pictures and the blurring is computed on the client side.
Thereby, you can see the real pictures just by disabling some CSS rules. These pictures are in very low definition though.</p>
<p><img src="https://user-images.githubusercontent.com/9092290/68415517-d6463600-0192-11ea-8606-0e61ac9a6320.jpg"></p>

<p>This project works by saving the ids of the “blurred” images and then finds them in your recommendations feed.</p>

<h2 id="faq">F.A.Q</h2>
<p><strong>Q:</strong> I didn’t get any match even tough Tinder tells me that I got X+ likes!?</p>

<p><strong>A:</strong> Several reasons could explain that:</p>
<ul>
  <li>These users are now out of range</li>
  <li>They are not in your elo anymore</li>
  <li>You swiped them left when you were swiping like a muggle</li>
  <li>Recommendations are sometimes really random so the program works better in the long run. Don’t except to match everyone on the first try</li>
</ul>

