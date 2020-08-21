---
ID: 8845
post_title: >
  Customizing Sublime Text for Python Web
  Development
post_name: customizing-sublime-text-for-python
author: Kim Desmond
post_date: 2018-05-17 11:07:53
layout: post
link: >
  https://codingnomads.co/blog/learn-to-code/customizing-sublime-text-for-python/
published: true
tags: [ ]
categories:
  - Learn to Code
  - Software Engineering
---
&nbsp;

&nbsp;
<h6>by Martin Breuss, CodingNomads</h6>
<em>This article was originally published on <a href="https://medium.com/@martin.breuss/customizing-sublime-text-for-python-web-development-de31873d2d06">Medium.com</a>.</em>

Sublime Text’s rich package ecosystem makes it possible to fine-tune the text editor specifically to what you are using it for. Some of the packages are universally helpful, others, such as syntax checking, are specific to the programming language you are working with.

Changing settings is easy and might also help to clarify how to do further customizations — if that is where your ❤ is at.

&nbsp;

<section class="section section--body">
<div class="section-content">
<div class="section-inner sectionLayout--insetColumn">
<h3 id="4140" class="graf graf--h3 graf--leading">Sublime Settings</h3>
<p id="fb83" class="graf graf--p graf-after--h3">Before moving onto installing plugins, there are a couple of useful settings that can help to tailor Sublime for python development. Go to <strong class="markup--strong markup--p-strong">Sublime Text → Preferences → Settings</strong> and in the <em class="markup--em markup--p-em">Preferences.sublime.settings-User</em> file enter the following rules:</p>

<pre class="graf graf--pre graf-after--p">{
    "spell_check": false,
    "rulers":
    [
        72, 79
    ],
    "tab_size": 4,
    "translate_tabs_to_spaces": true,
    "trim_trailing_white_space_on_save": true,
    "ensure_newline_at_eof_on_save": true
}

</pre>
I personally prefer to keep "spell_check" on false because I don’t like to see red lines everywhere when writing non-dictionary-compliant words. Maybe I’m just damaged by the school system. If you have a different opinion on this, simply set "spell_check" to true.

The magic numbers for the "rulers" setting originate from pythons PEP8. Docstrings and comments should be limited to 72 characters and all other lines should not be longer than 79 characters. The ruler lines can help to remind you when you are approaching these limits.

In good python fashion we set the "tab_size" to 4 and "translat_tabs_to_spaces" to <a class="markup--anchor markup--p-anchor" href="https://www.youtube.com/watch?v=SsoOG6ZeyUI" target="_blank" rel="nofollow noopener noreferrer" data-href="https://www.youtube.com/watch?v=SsoOG6ZeyUI">avoid relationship troubles</a>.
<figure id="e66c" class="graf graf--figure graf--iframe graf-after--p">
<div class="aspectRatioPlaceholder is-locked">
<div></div>
<div class="aspectRatioPlaceholder-fill"> [embedyt]https://www.youtube.com/watch?v=SsoOG6ZeyUI[/embedyt]</div>
<div></div>
</div></figure>
<p id="31aa" class="graf graf--p graf-after--figure graf--trailing">
Finally, we can get another PEP8 compliance automation with "ensure_newline_at_eof_on_save" which does just that: adding a single newline at the end of the file when you save the document.</p>
&nbsp;

</div>
</div>
</section><section class="section section--body">
<div class="section-content">
<div class="section-inner sectionLayout--insetColumn">
<h3 id="0bed" class="graf graf--h3 graf--leading">Packages (Plugins)</h3>
<p id="01fd" class="graf graf--p graf-after--h3">And now we dive right into the pool of great packages for Sublime Text that extend its functionality and can make your life as a programmer easier and more colorful!</p>
&nbsp;
<h4></h4>
<h4 id="1d53" class="graf graf--h4 graf-after--p"><u><a class="markup--anchor markup--h4-anchor" href="https://github.com/SideBarEnhancements-org/SideBarEnhancements" target="_blank" rel="nofollow noopener noreferrer" data-href="https://github.com/SideBarEnhancements-org/SideBarEnhancements">SidebarEnhancement</a></u></h4>
<p id="493b" class="graf graf--p graf-after--h4">Power-up for the ST sidebar, introducing useful features such as being able to create new files directly from there and sending files to the recycle bin when they are deleted from inside Sublime.</p>

<figure id="c5f1" class="graf graf--figure graf-after--p">
<div class="aspectRatioPlaceholder is-locked">
<div class="progressiveMedia js-progressiveMedia graf-image is-canvasLoaded is-imageLoaded" data-image-id="1*Du8DeCowEFtdwQLAjV0OKQ.jpeg" data-width="244" data-height="207" data-scroll="native"><canvas class="progressiveMedia-canvas js-progressiveMedia-canvas" width="75" height="62"></canvas><img class="progressiveMedia-image js-progressiveMedia-image aligncenter" src="https://cdn-images-1.medium.com/max/800/1*Du8DeCowEFtdwQLAjV0OKQ.jpeg" data-src="https://cdn-images-1.medium.com/max/800/1*Du8DeCowEFtdwQLAjV0OKQ.jpeg" /></div>
</div></figure>
&nbsp;
<h4 id="2284" class="graf graf--h4 graf-after--figure"><span style="text-decoration: underline;"><a class="markup--anchor markup--h4-anchor" href="http://damnwidget.github.io/anaconda/" target="_blank" rel="nofollow noopener noreferrer" data-href="http://damnwidget.github.io/anaconda/">Anaconda</a></span></h4>
<blockquote id="7959" class="graf graf--blockquote graf-after--h4"><strong class="markup--strong markup--blockquote-strong">Note: </strong>this is <em class="markup--em markup--blockquote-em">not </em>the popular python distribution often used for data science that goes by the same name.</blockquote>
<p id="fec7" class="graf graf--p graf-after--blockquote">The Sublime Text Anaconda plugin helps to make ST more IDE-like while keeping it still operating much quicker than most IDEs. It introduces easy access to useful features such as:</p>

<ul class="postList">
 	<li id="bb2c" class="graf graf--li graf-after--p">Code autocompletion</li>
 	<li id="8753" class="graf graf--li graf-after--li">Code linting: syntax errors</li>
 	<li id="629e" class="graf graf--li graf-after--li">Code linting: highlight and automatically fix PEP8 violations</li>
 	<li id="b16e" class="graf graf--li graf-after--li">Python documentation on class, method or function under the cursor</li>
 	<li id="1f6d" class="graf graf--li graf-after--li">Goto Python definition anywhere in the project</li>
 	<li id="5ad1" class="graf graf--li graf-after--li">Find object usage across the project</li>
 	<li id="4081" class="graf graf--li graf-after--li">and lots more…</li>
</ul>
&nbsp;
<h4 id="000b" class="graf graf--h4 graf-after--li"><span style="text-decoration: underline;"><a class="markup--anchor markup--h4-anchor" href="https://packagecontrol.io/packages/AutoDocstring" target="_blank" rel="nofollow noopener noreferrer" data-href="https://packagecontrol.io/packages/AutoDocstring">Auto Docstring</a></span></h4>
<p id="752e" class="graf graf--p graf-after--h4">Auto Docstring does just what its name suggests — it allows you to swiftly create a Python docstring template for your selected function, method or class. You can even add docstrings for every function in a file and change between Google and Numpy style even after the docstrings were created. A very basic auto-generated example would look like this:</p>

<pre id="d6b9" class="graf graf--pre graf-after--p">def my_function():
    """Summary
    
    Returns:
        TYPE: Description
    """
	return None</pre>
<h4 id="167b" class="graf graf--h4 graf-after--pre"><span style="text-decoration: underline;"><a class="markup--anchor markup--h4-anchor" href="http://www.sublimelinter.com/en/stable/" target="_blank" rel="nofollow noopener noreferrer" data-href="http://www.sublimelinter.com/en/stable/">SublimeLinter</a></span></h4>
<p id="6a64" class="graf graf--p graf-after--h4">For python syntax and PEP8 you could stick with using the linting provided through the Anaconda plugin. However, using <strong class="markup--strong markup--p-strong">SublimeLinter</strong> has the advantage that it is extensible also with other linters that are useful for web development. That’s why I would suggest to disable Anaconda’s linter, like so:</p>
<p id="0015" class="graf graf--p graf-after--p">Use the file menu: <strong class="markup--strong markup--p-strong">Sublime → Preferences → Package Settings → Anaconda → Settings — User </strong>to go to the user-defined Anaconda settings file. Then set: <code class="markup--code markup--p-code">{"anaconda_linting": false}</code></p>
<p id="f0c5" class="graf graf--p graf-after--p">Now, install <strong class="markup--strong markup--p-strong">SublimeLinter</strong> using the Package Manager.</p>
&nbsp;
<blockquote id="a2bc" class="graf graf--blockquote graf-after--p"><strong class="markup--strong markup--blockquote-strong">Note: </strong>Most of the linters require additional packages to operate correctly, so make sure to read the instructions carefully</blockquote>
&nbsp;
<p id="adb4" class="graf graf--p graf-after--blockquote"><span style="text-decoration: underline;"><a class="markup--anchor markup--p-anchor" href="https://github.com/SublimeLinter/SublimeLinter-pyflakes" target="_blank" rel="nofollow noopener noreferrer" data-href="https://github.com/SublimeLinter/SublimeLinter-pyflakes"><strong class="markup--strong markup--p-strong">SublimeLinter-pyflakes</strong></a></span><strong class="markup--strong markup--p-strong">
pyflakes</strong> performs syntax checking on python files. This package needs to be installed using pip before adding it to ST with the Package Manager</p>
&nbsp;
<p id="0ecc" class="graf graf--p graf-after--p"><span style="text-decoration: underline;"><a class="markup--anchor markup--p-anchor" href="https://github.com/PyCQA/pycodestyle" target="_blank" rel="nofollow noopener noreferrer" data-href="https://github.com/PyCQA/pycodestyle"><strong class="markup--strong markup--p-strong">SublimeLinter-pycodestyle</strong></a></span><strong class="markup--strong markup--p-strong">
pycodestyle</strong> is the new name of the pep8 package. Install it using pip, then add it to Sublime using the Package Manager for PEP8-compliant code style linting.</p>
&nbsp;
<p id="1782" class="graf graf--p graf-after--p"><strong class="markup--strong markup--p-strong">Other useful linters for web development:</strong></p>

<ul class="postList">
 	<li id="2c13" class="graf graf--li graf-after--p"><span style="text-decoration: underline;"><a class="markup--anchor markup--li-anchor" href="https://sublime.wbond.net/packages/SublimeLinter-json" target="_blank" rel="noopener nofollow noreferrer" data-href="https://sublime.wbond.net/packages/SublimeLinter-json">SublimeLinter-json</a></span></li>
 	<li id="81b4" class="graf graf--li graf-after--li"><span style="text-decoration: underline;"><a class="markup--anchor markup--li-anchor" href="https://sublime.wbond.net/packages/SublimeLinter-jshint" target="_blank" rel="nofollow noopener noreferrer" data-href="https://sublime.wbond.net/packages/SublimeLinter-jshint">SublimeLinter-jshint</a></span></li>
 	<li id="288d" class="graf graf--li graf-after--li"><span style="text-decoration: underline;"><a class="markup--anchor markup--li-anchor" href="https://sublime.wbond.net/packages/SublimeLinter-csslint" target="_blank" rel="nofollow noopener noreferrer" data-href="https://sublime.wbond.net/packages/SublimeLinter-csslint">SublimeLinter-csslint</a></span></li>
 	<li id="a2d9" class="graf graf--li graf-after--li"><span style="text-decoration: underline;"><a class="markup--anchor markup--li-anchor" href="https://sublime.wbond.net/packages/SublimeLinter-html-tidy" target="_blank" rel="nofollow noopener noreferrer" data-href="https://sublime.wbond.net/packages/SublimeLinter-html-tidy">SublimeLinter-html-tidy</a></span></li>
 	<li id="5038" class="graf graf--li graf-after--li"><span style="text-decoration: underline;"><a class="markup--anchor markup--li-anchor" href="https://sublime.wbond.net/packages/SublimeLinter-pyyaml" target="_blank" rel="nofollow noopener noreferrer" data-href="https://sublime.wbond.net/packages/SublimeLinter-pyyaml">SublimeLinter-pyyaml</a></span></li>
</ul>
&nbsp;
<h4 id="7e21" class="graf graf--h4 graf-after--li"><span style="text-decoration: underline;"><a class="markup--anchor markup--h4-anchor" href="https://github.com/squ1b3r/Djaneiro" target="_blank" rel="noopener nofollow noreferrer" data-href="https://github.com/squ1b3r/Djaneiro">Djaneiro</a></span></h4>
<p id="bbd0" class="graf graf--p graf-after--h4">This useful plugin adds a couple of handy Django snippets with tab autocompletion into ST to make working on web projects quicker.</p>
&nbsp;
<p id="c1d4" class="graf graf--p graf-after--p">E.g. block + TAB generates {% block %}{% endblock %}</p>
&nbsp;
<figure id="c617" class="graf graf--figure graf-after--p">
<div class="aspectRatioPlaceholder is-locked">
<div class="aspectRatioPlaceholder-fill"></div>
<div class="progressiveMedia js-progressiveMedia graf-image is-canvasLoaded is-imageLoaded" data-image-id="1*_D7FGqRxT_tIUw7wLEeqcg.gif" data-width="278" data-height="192" data-scroll="native"><canvas class="progressiveMedia-canvas js-progressiveMedia-canvas" width="75" height="50"></canvas><img class="progressiveMedia-image js-progressiveMedia-image aligncenter" src="https://cdn-images-1.medium.com/max/800/1*_D7FGqRxT_tIUw7wLEeqcg.gif" data-src="https://cdn-images-1.medium.com/max/800/1*_D7FGqRxT_tIUw7wLEeqcg.gif" /></div>
</div></figure>
&nbsp;
<p id="facd" class="graf graf--p graf-after--figure">Very cool. Check out all it has to offer <a class="markup--anchor markup--p-anchor" href="https://github.com/squ1b3r/Djaneiro" target="_blank" rel="nofollow noopener noreferrer" data-href="https://github.com/squ1b3r/Djaneiro">here</a>!</p>
&nbsp;
<h4></h4>
<h4 id="0df0" class="graf graf--h4 graf-after--p"><span style="text-decoration: underline;"><a class="markup--anchor markup--h4-anchor" href="https://github.com/kemayo/sublime-text-git/wiki" target="_blank" rel="nofollow noopener noreferrer" data-href="https://github.com/kemayo/sublime-text-git/wiki">Git</a></span></h4>
<p id="a903" class="graf graf--p graf-after--h4">Allows to do the most common set of git commands from within Sublime.
git add, commit, push etc. right from your favorite text editor.</p>
&nbsp;
<h4></h4>
<h4 id="e4fd" class="graf graf--h4 graf-after--p"><span style="text-decoration: underline;"><a class="markup--anchor markup--h4-anchor" href="https://github.com/jisaacks/GitGutter" target="_blank" rel="nofollow noopener noreferrer" data-href="https://github.com/jisaacks/GitGutter">GitGutter</a></span></h4>
<p id="ddf5" class="graf graf--p graf-after--h4">GitGutter helps to keep track of which files have been edited since the last commit. It adds small symbols next to the line numbers that indicate their status in relation to the git repository.</p>
&nbsp;
<figure id="3f0d" class="graf graf--figure graf-after--p">
<div class="aspectRatioPlaceholder is-locked">
<div class="aspectRatioPlaceholder-fill"></div>
<div class="progressiveMedia js-progressiveMedia graf-image is-canvasLoaded is-imageLoaded" data-image-id="1*LfrYvdN2-0vx_uDLWGN9sw.png" data-width="349" data-height="154" data-scroll="native"><canvas class="progressiveMedia-canvas js-progressiveMedia-canvas" width="75" height="32"></canvas><img class="progressiveMedia-image js-progressiveMedia-image" src="https://cdn-images-1.medium.com/max/800/1*LfrYvdN2-0vx_uDLWGN9sw.png" data-src="https://cdn-images-1.medium.com/max/800/1*LfrYvdN2-0vx_uDLWGN9sw.png" /></div>
</div></figure>
&nbsp;
<h4 id="2a5e" class="graf graf--h4 graf-after--figure"><span style="text-decoration: underline;"><a class="markup--anchor markup--h4-anchor" href="https://github.com/wuub/requirementstxt" target="_blank" rel="nofollow noopener noreferrer" data-href="https://github.com/wuub/requirementstxt">requirementstxt</a></span></h4>
<p id="a0b0" class="graf graf--p graf-after--h4">Introduces syntax highlighting for <em class="markup--em markup--p-em">requirements.txt</em> files. Be good to your 👀!</p>
&nbsp;
<h4></h4>
<h4 id="1edb" class="graf graf--h4 graf-after--p"><span style="text-decoration: underline;"><a class="markup--anchor markup--h4-anchor" href="https://facelessuser.github.io/MarkdownPreview/" target="_blank" rel="nofollow noopener noreferrer" data-href="https://facelessuser.github.io/MarkdownPreview/">Markdown Preview</a></span></h4>
<p id="21f6" class="graf graf--p graf-after--h4">Allows to preview Markdown documents in your browser — build them using different available flavors!</p>
&nbsp;
<h4 id="5168" class="graf graf--h4 graf-after--p">Other useful Web Dev Packages</h4>
<p id="7f8f" class="graf graf--p graf-after--h4"><span style="text-decoration: underline;"><a class="markup--anchor markup--p-anchor" href="https://github.com/y0ssar1an/CSS3" target="_blank" rel="nofollow noopener noreferrer" data-href="https://github.com/y0ssar1an/CSS3"><strong class="markup--strong markup--p-strong">CSS3</strong></a></span><strong class="markup--strong markup--p-strong">
</strong>The CSS3 plugin allows for futuristic CSS syntax highlighting. You’ll need to tweak the rest of the settings a bit, but it’s easy to follow along the steps here:</p>
&nbsp;
<p id="05b3" class="graf graf--p graf-after--p"><span style="text-decoration: underline;"><a class="markup--anchor markup--p-anchor" href="https://github.com/Monnoroch/ColorHighlighter" target="_blank" rel="nofollow noopener noreferrer" data-href="https://github.com/Monnoroch/ColorHighlighter"><strong class="markup--strong markup--p-strong">ColorHighlighter</strong></a></span><strong class="markup--strong markup--p-strong">
</strong>This one is fun. Adds more 🌈 to your code. Hex color values will be displayed with the corresponding color as background. Makes it easier to remember what color you were adding where.</p>
&nbsp;
<p id="ab10" class="graf graf--p graf-after--p graf--trailing"><span style="text-decoration: underline;"><a class="markup--anchor markup--p-anchor" href="https://emmet.io/" target="_blank" rel="nofollow noopener noreferrer" data-href="https://emmet.io/"><strong class="markup--strong markup--p-strong">Emmet</strong></a></span><strong class="markup--strong markup--p-strong">
</strong>If you’re excited about automating the repetitive parts of your web development work, then Emmet can be a big help. Install the <a class="markup--anchor markup--p-anchor" href="https://github.com/sergeche/emmet-sublime" target="_blank" rel="nofollow noopener noreferrer" data-href="https://github.com/sergeche/emmet-sublime">package</a>, then learn how to benefit: <a class="markup--anchor markup--p-anchor" href="https://docs.emmet.io/cheat-sheet/" target="_blank" rel="nofollow noopener noreferrer" data-href="https://docs.emmet.io/cheat-sheet/">https://docs.emmet.io/cheat-sheet/
</a></p>

</div>
</div>
&nbsp;

</section><section class="section section--body">
<div class="section-content">
<div class="section-inner sectionLayout--insetColumn">
<h4 id="5168" class="graf graf--h4 graf-after--p">Want to learn more?</h4>
<p id="c7f1" class="graf graf--p graf--leading">With adding these packages and tweaking the settings as mentioned above, Sublime Text becomes a lightweight but powerful editor for web development with Python.</p>
<p id="2391" class="graf graf--p graf-after--p">If you are just getting started and are looking for a <strong class="markup--strong markup--p-strong">fun and affordable bootcamp</strong> that helps you to learn programming and gets you to travel and see the world, check out CodingNomads' <a target="blank" href="https://codingnomads.co/#courses" rel="noopener noreferrer">upcoming Python courses</a>. 🌇 💻 🎒🏝</p>
&nbsp;
<h3 id="9ca8" class="graf graf--h3 graf-after--figure">More Info:</h3>
<ul class="postList">
 	<li id="1abc" class="graf graf--li graf-after--h3"><a class="markup--anchor markup--li-anchor" href="https://medium.com/@arshamshirvani/sync-your-sublime-text-3-configurations-safely-and-easy-b493021c80da" target="_blank" rel="noopener noreferrer" data-href="https://medium.com/@arshamshirvani/sync-your-sublime-text-3-configurations-safely-and-easy-b493021c80da">Sync your settings to GitHub</a></li>
</ul>
<p id="dbba" class="graf graf--p graf-after--li"><strong class="markup--strong markup--p-strong">Plugin Setup:</strong></p>

<ul class="postList">
 	<li id="1936" class="graf graf--li graf-after--p"><a class="markup--anchor markup--li-anchor" href="http://www.gtlambert.com/blog/python-sublime-text-3" target="_blank" rel="nofollow noopener noreferrer" data-href="http://www.gtlambert.com/blog/python-sublime-text-3">http://www.gtlambert.com/blog/python-sublime-text-3</a></li>
 	<li id="5efd" class="graf graf--li graf-after--li"><a class="markup--anchor markup--li-anchor" href="https://www.fullstackpython.com/sublime-text.html" target="_blank" rel="nofollow noopener noreferrer" data-href="https://www.fullstackpython.com/sublime-text.html">https://www.fullstackpython.com/sublime-text.html</a></li>
 	<li id="74bc" class="graf graf--li graf-after--li"><a class="markup--anchor markup--li-anchor" href="https://realpython.com/setting-up-sublime-text-3-for-full-stack-python-development/" target="_blank" rel="nofollow noopener noreferrer" data-href="https://realpython.com/setting-up-sublime-text-3-for-full-stack-python-development/">https://realpython.com/setting-up-sublime-text-3-for-full-stack-python-development/</a></li>
 	<li id="56b8" class="graf graf--li graf-after--li"><a class="markup--anchor markup--li-anchor" href="https://nazrul.me/2017/05/17/make-sublime-text-as-the-best-ide-for-full-stack-python-development/" target="_blank" rel="nofollow noopener noreferrer" data-href="https://nazrul.me/2017/05/17/make-sublime-text-as-the-best-ide-for-full-stack-python-development/">https://nazrul.me/2017/05/17/make-sublime-text-as-the-best-ide-for-full-stack-python-development/</a></li>
</ul>
<p id="1608" class="graf graf--p graf-after--li"><strong class="markup--strong markup--p-strong">Learn to increase your performance when working with ST3:</strong></p>

<ul class="postList">
 	<li id="1ca5" class="graf graf--li graf-after--p"><a class="markup--anchor markup--li-anchor" href="https://hackernoon.com/super-charge-your-sublime-text-3-to-increase-your-productivity-5d02c2c1b356" target="_blank" rel="nofollow noopener noreferrer" data-href="https://hackernoon.com/super-charge-your-sublime-text-3-to-increase-your-productivity-5d02c2c1b356">https://hackernoon.com/super-charge-your-sublime-text-3-to-increase-your-productivity-5d02c2c1b356</a></li>
</ul>
</div>
</div>
</section>&nbsp;
<h4><b>READ NEXT</b>: <a href="https://codingnomads.co/how-to-find-a-job-after-a-coding-bootcamp/" target="_blank" rel="noopener noreferrer">How to find a job after a coding bootcamp</a></h4>