---
title: Setup
---

### Register to Copernicus Climate Data Store

We will be using the Copernicus Climate Data Store and its Python and R API so it is important to register before the workshop.

- Create an [account](https://cds.climate.copernicus.eu/user/login?destination=%2F%23!%2Fhome)

### Copernicus online learning environment (Optional)

We will be using additional training material from the Copernicus online learning environment
and if you would like to consult the materials yourself, 
register [here](https://uls.climate.copernicus.eu/login).

### Install packages

#### Basic setup

- [The Bash Shell](#shell)
- [Git](#git)
- [Text editor](#editor)
- [Anaconda Package Manager](#anaconda) 

#### Python
- [Python installation](#python) 
- [Installation of additional python packages](#python-packages) 

#### R 
- [R installation](#r) 
- [Installation of additional R libraries](#r-libraries) 


<h2 id="setup">Setup</h2>

<p>
  To participate in a
  {% if page.carpentry == "swc" %}
  Software Carpentry
  {% elsif page.carpentry == "dc" %}
  Data Carpentry
  {% elsif page.carpentry == "lc" %}
  Library Carpentry
  {% endif %}
  workshop,
  you will need access to the software described below.
  In addition, you will need an up-to-date web browser.
</p>
<p>
  We maintain a list of common issues that occur during installation as a reference for instructors
  that may be useful on the
  <a href = "{{site.swc_github}}/workshop-template/wiki/Configuration-Problems-and-Solutions">Configuration Problems and Solutions wiki page</a>.
</p>

<div id="shell"> {% comment %} Start of 'shell' section. {% endcomment %}
  <h3>The Bash Shell</h3>
  <p>
    Bash is a commonly-used shell that gives you the power to do simple
    tasks more quickly.
  </p>

  <div>
    <ul class="nav nav-tabs nav-justified" role="tablist">
      <li role="presentation" class="active"><a data-os="windows" href="#shell-windows" aria-controls="Windows" role="tab" data-toggle="tab">Windows</a></li>
      <li role="presentation"><a data-os="macos" href="#shell-macos" aria-controls="MacOS" role="tab" data-toggle="tab">MacOS</a></li>
      <li role="presentation"><a data-os="linux" href="#shell-linux" aria-controls="Linux" role="tab" data-toggle="tab">Linux</a></li>
    </ul>

    <div class="tab-content">
      <article role="tabpanel" class="tab-pane active" id="shell-windows">
        <a href="https://www.youtube.com/watch?v=339AEqk9c-8">Video Tutorial</a>
        <ol>
          <li>Download the Git for Windows <a href="https://git-for-windows.github.io/">installer</a>.</li>
          <li>Run the installer and follow the steps below:
            <ol>
              {% comment %} Git 2.18.0 Setup {% endcomment %}
              <li>
                Click on "Next" four times (two times if you've previously
                installed Git).  You don't need to change anything
                in the Information, location, components, and start menu screens.
              </li>
              <li>
                <strong>
                  Select "Use the nano editor by default" and click on "Next".
                </strong>
              </li>
              {% comment %} Adjusting your PATH environment {% endcomment %}
              <li>
                Keep "Use Git from the Windows Command Prompt" selected and click on "Next".
                If you forgot to do this programs that you need for the workshop will not work properly.
                If this happens rerun the installer and select the appropriate option.
              </li>
              {% comment %} Choosing the SSH executable {% endcomment %}
              <li>Click on "Next".</li>
              {% comment %} Configuring the line ending conversions {% endcomment %}
              <li>
                Keep "Checkout Windows-style, commit Unix-style line endings" selected and click on "Next".
              </li>
              {% comment %} Configuring the terminal emulator to use with Git Bash {% endcomment %}
              <li>
                <strong>
                  Select "Use Windows' default console window" and click on "Next".
                </strong>
              </li>
              {% comment %} Configuring experimental performance tweaks {% endcomment %}
              <li>Click on "Install".</li>
              {% comment %} Installing {% endcomment %}
              {% comment %} Completing the Git Setup Wizard {% endcomment %}
              <li>Click on "Finish".</li>
            </ol>
          </li>
          <li>
            If your "HOME" environment variable is not set (or you don't know what this is):
            <ol>
              <li>Open command prompt (Open Start Menu then type <code>cmd</code> and press [Enter])</li>
              <li>
                Type the following line into the command prompt window exactly as shown:
                <p><code>setx HOME "%USERPROFILE%"</code></p>
              </li>
              <li>Press [Enter], you should see <code>SUCCESS: Specified value was saved.</code></li>
              <li>Quit command prompt by typing <code>exit</code> then pressing [Enter]</li>
            </ol>
          </li>
        </ol>
        <p>This will provide you with both Git and Bash in the Git Bash program.</p>
      </article>
      <article role="tabpanel" class="tab-pane active" id="shell-macos">
        <p>
          The default shell in all versions of macOS is Bash, so no
          need to install anything.  You access Bash from the Terminal
          (found in
          <code>/Applications/Utilities</code>).
          See the Git installation <a href="https://www.youtube.com/watch?v=9LQhwETCdwY ">video tutorial</a>
          for an example on how to open the Terminal.
          You may want to keep
          Terminal in your dock for this workshop.
        </p>
      </article>
      <article role="tabpanel" class="tab-pane active" id="shell-linux">
        <p>
          The default shell is usually Bash, but if your
          machine is set up differently you can run it by opening a
          terminal and typing <code>bash</code>.  There is no need to
          install anything.
        </p>
      </article>
    </div>
  </div>
</div> {% comment %} End of 'shell' section. {% endcomment %}

<div id="git"> {% comment %} Start of 'Git' section. GitHub browser compatability
  is given at https://help.github.com/articles/supported-browsers/{% endcomment %}
  <h3>Git</h3>
  <p>
    Git is a version control system that lets you track who made changes
    to what when and has options for easily updating a shared or public
    version of your code
    on <a href="https://github.com/">github.com</a>. You will need a
    <a href="https://help.github.com/articles/supported-browsers/">supported
    web browser</a>.
  </p>
  <p>
    You will need an account at <a href="https://github.com/">github.com</a>
    for parts of the Git lesson. Basic GitHub accounts are free. We encourage
    you to create a GitHub account if you don't have one already.
    Please consider what personal information you'd like to reveal. For
    example, you may want to review these
    <a href="https://help.github.com/articles/keeping-your-email-address-private/">instructions
      for keeping your email address private</a> provided at GitHub.
  </p>

  <div>
    <ul class="nav nav-tabs nav-justified" role="tablist">
      <li role="presentation" class="active"><a data-os="windows" href="#git-windows" aria-controls="Windows" role="tab" data-toggle="tab">Windows</a></li>
      <li role="presentation"><a data-os="macos" href="#git-macos" aria-controls="MacOS" role="tab" data-toggle="tab">MacOS</a></li>
      <li role="presentation"><a data-os="linux" href="#git-linux" aria-controls="Linux" role="tab" data-toggle="tab">Linux</a></li>
    </ul>

    <div class="tab-content">
      <article role="tabpanel" class="tab-pane active" id="git-windows">
        <p>
          Git should be installed on your computer as part of your Bash
          install (described above).
        </p>
      </article>
      <article role="tabpanel" class="tab-pane active" id="git-macos">
        <a href="https://www.youtube.com/watch?v=9LQhwETCdwY ">Video Tutorial</a>
        <p>
          <strong>For OS X 10.9 and higher</strong>, install Git for Mac
          by downloading and running the most recent "mavericks" installer from
          <a href="http://sourceforge.net/projects/git-osx-installer/files/">this list</a>.
          Because this installer is not signed by the developer, you may have to
          right click (control click) on the .pkg file, click Open, and click
          Open on the pop up window. 
          After installing Git, there will not be anything in your <code>/Applications</code> folder,
          as Git is a command line program.
          <strong>For older versions of OS X (10.5-10.8)</strong> use the
          most recent available installer labelled "snow-leopard"
          <a href="http://sourceforge.net/projects/git-osx-installer/files/">available here</a>.
        </p>
      </article>
      <article role="tabpanel" class="tab-pane active" id="git-linux">
        <p>
          If Git is not already available on your machine you can try to
          install it via your distro's package manager. For Debian/Ubuntu run
          <code>sudo apt-get install git</code> and for Fedora run
          <code>sudo dnf install git</code>.
        </p>
      </article>
    </div>
  </div>
</div> {% comment %} End of 'Git' section. {% endcomment %}

<div id="editor"> {% comment %} Start of 'editor' section. {% endcomment %}
  <h3>Text Editor</h3>

  <p>
    When you're writing code, it's nice to have a text editor that is
    optimized for writing code, with features like automatic
    color-coding of key words. The default text editor on macOS and
    Linux is usually set to Vim, which is not famous for being
    intuitive. If you accidentally find yourself stuck in it, hit
    the <kbd>Esc</kbd> key, followed by <kbd>:</kbd>+<kbd>Q</kbd>+<kbd>!</kbd> 
    (colon, lower-case 'q', exclamation mark), then hitting <kbd>Return</kbd> to 
    return to the shell.
  </p>

  <div>
    <ul class="nav nav-tabs nav-justified" role="tablist">
      <li role="presentation" class="active"><a data-os="windows" href="#editor-windows" aria-controls="Windows" role="tab" data-toggle="tab">Windows</a></li>
      <li role="presentation"><a data-os="macos" href="#editor-macos" aria-controls="MacOS" role="tab" data-toggle="tab">MacOS</a></li>
      <li role="presentation"><a data-os="linux" href="#editor-linux" aria-controls="Linux" role="tab" data-toggle="tab">Linux</a></li>
    </ul>

    <div class="tab-content">
      <article role="tabpanel" class="tab-pane active" id="editor-windows">
        <p>
          nano is a basic editor and the default that instructors use in the workshop.
          It is installed along with Git.
        </p>
        <p>
          Others editors that you can use are
          <a href="https://notepad-plus-plus.org/">Notepad++</a> or
          <a href="https://www.sublimetext.com/">Sublime Text</a>.
          <strong>Be aware that you must
            add its installation directory to your system path.</strong>
          Please ask your instructor to help you do this.
        </p>
      </article>
      <article role="tabpanel" class="tab-pane active" id="editor-macos">
        <p>
          nano is a basic editor and the default that instructors use in the workshop.
          See the Git installation <a href="https://www.youtube.com/watch?v=9LQhwETCdwY ">video tutorial</a>
          for an example on how to open nano.
          It should be pre-installed.
        </p>
        <p>
          Others editors that you can use are
          <a href="https://www.barebones.com/products/bbedit/">BBEdit</a> or
          <a href="https://www.sublimetext.com/">Sublime Text</a>.
        </p>
      </article>
      <article role="tabpanel" class="tab-pane active" id="editor-linux">
        <p>
          nano is a basic editor and the default that instructors use in the workshop.
          It should be pre-installed.
        </p>
        <p>
          Others editors that you can use are
          <a href="https://wiki.gnome.org/Apps/Gedit">Gedit</a>,
          <a href="https://kate-editor.org/">Kate</a> or
          <a href="https://www.sublimetext.com/">Sublime Text</a>.
        </p>
      </article>
    </div>
  </div>
</div> {% comment %} End of 'editor' section. {% endcomment %}

<div id="anaconda"> {% comment %} Start of 'Python' section. Remove the third paragraph if
  the workshop will teach Python using something other than
  the Jupyter notebook.
  Details at https://jupyter-notebook.readthedocs.io/en/stable/notebook.html#browser-compatibility {% endcomment %}
  <h3>Anaconda Package Manager</h3>

  
  <p>
    Installing <a href="https://www.anaconda.com/distribution/">Anaconda</a> will allow  
    give you to easily install <a href="https://python.org">Python</a> and <a href="https://www.r-project.org/">R</a>.
	Both Python and R are popular languages for
    research computing, and great for general-purpose programming as
    well.  Installing additional research packages individually can be
    a bit difficult, so we recommend
    <a href="https://www.anaconda.com/distribution/">Anaconda</a>,
    an all-in-one installer.
  </p>

  <p>
    Regardless of how you choose to install it,
    <strong>please make sure you install Python version 3.x</strong>
    (e.g., 3.6 is fine).
  </p>

  <div>
    <ul class="nav nav-tabs nav-justified" role="tablist">
      <li role="presentation" class="active"><a data-os="windows" href="#python-windows" aria-controls="Windows" role="tab" data-toggle="tab">Windows</a></li>
      <li role="presentation"><a data-os="macos" href="#python-macos" aria-controls="MacOS" role="tab" data-toggle="tab">MacOS</a></li>
      <li role="presentation"><a data-os="linux" href="#python-linux" aria-controls="Linux" role="tab" data-toggle="tab">Linux</a></li>
    </ul>

    <div class="tab-content">
      <article role="tabpanel" class="tab-pane active" id="python-windows">
        <a href="https://www.youtube.com/watch?v=xxQ0mzZ8UvA">Video Tutorial</a>
        <ol>
          <li>Open <a href="https://www.anaconda.com/download/#windows">https://www.anaconda.com/download/#windows</a> with your web browser.</li>
          <li>Download the Python 3 installer for Windows.</li>
          <li>Install Python 3 using all of the defaults for installation <em>except</em> make sure to check <strong>Add Anaconda to my PATH environment variable</strong>.</li>
        </ol>
      </article>
      <article role="tabpanel" class="tab-pane active" id="python-macos">
        <a href="https://www.youtube.com/watch?v=TcSAln46u9U">Video Tutorial</a>
        <ol>
          <li>Open <a href="https://www.anaconda.com/download/#macos">https://www.anaconda.com/download/#macos</a> with your web browser.</li>
          <li>Download the Python 3 installer for OS X.</li>
          <li>Install Python 3 using all of the defaults for installation.</li>
        </ol>
      </article>
      <article role="tabpanel" class="tab-pane active" id="python-linux">
        <ol>
          <li>Open <a href="https://www.anaconda.com/download/#linux">https://www.anaconda.com/download/#linux</a> with your web browser.</li>
          <li>Download the Python 3 installer for Linux.<br>
            (The installation requires using the shell. If you aren't
            comfortable doing the installation yourself
            stop here and request help at the workshop.)
          </li>
          <li>
            Open a terminal window.
          </li>
          <li>
            Type <pre>bash Anaconda3-</pre> and then press
            <kbd>Tab</kbd>. The name of the file you just downloaded should
            appear. If it does not, navigate to the folder where you
            downloaded the file, for example with:
            <pre>cd Downloads</pre>
            Then, try again.
          </li>
          <li>
            Press <kbd>Return</kbd>. You will follow the text-only prompts. To move through
            the text, press <kbd>Spacebar</kbd>. Type <code>yes</code> and
            press enter to approve the license. Press enter to approve the
            default location for the files. Type <code>yes</code> and
            press enter to prepend Anaconda to your <code>PATH</code>
            (this makes the Anaconda distribution the default Python).
          </li>
          <li>
            Close the terminal window.
          </li>
        </ol>
      </article>
    </div>
  </div>
  {% comment %}
  <p>
    Once you are done installing the software listed above,
    please go to <a href="setup/index.html">this page</a>,
    which has instructions on how to test that everything was installed correctly.
  </p>
  {% endcomment %}
</div> {% comment %} End of 'Python' section. {% endcomment %}

<div id="python"> 
<h3>Python</h3>
<p>
If you have followed the previous section and installed <a href="#anaconda">Anaconda</a> then
you are ready to go with Python.
</p>
<p>
    We will teach Python using the <a href="https://jupyter.org/">Jupyter notebook</a>,
    a programming environment that runs in a web browser. For this to work you will need a reasonably
    up-to-date browser. The current versions of the Chrome, Safari and
    Firefox browsers are all
    <a href="https://jupyter-notebook.readthedocs.io/en/stable/notebook.html#browser-compatibility">supported</a>
    (some older browsers, including Internet Explorer version 9
    and below, are not).
  </p>

</div>
  
<div id="python-packages"> 

<h3>Install additional Python packages</h3>

To install additional Python packages/libraries, you need to follow the instructions below.

  <div>
    <ul class="nav nav-tabs nav-justified" role="tablist">
      <li role="presentation" class="active"><a data-os="windows" href="#python-packages-windows" aria-controls="Windows" role="tab" data-toggle="tab">Windows</a></li>
      <li role="presentation"><a data-os="macos" href="#python-packages-macos" aria-controls="MacOS" role="tab" data-toggle="tab">MacOS</a></li>
      <li role="presentation"><a data-os="linux" href="#python-packages-linux" aria-controls="Linux" role="tab" data-toggle="tab">Linux</a></li>
    </ul>

    <div class="tab-content">
      <article role="tabpanel" class="tab-pane active" id="python-packages-windows">
        <ol>
		  <li>Download <a href="environment.yml" download="environment.yml">environment.yml</a></li>
          <li><a href="https://docs.anaconda.com/anaconda/navigator/getting-started/">Open Anaconda navigator</a>.</li>
           <li>Click the Environments tab in the left menu. Then click Import and select the environment.yml file you downloaded. 
		  <img src="fig/navigator-import-environment.png" alt="Import environment">
		  </li>
        </ol>
      </article>
      <article role="tabpanel" class="tab-pane active" id="python-packages-macos">
        <ol>
          <li>Open a terminal</li>
          <li>Download <a href="environment.yml" download="environment.yml">environment.yml</a></li>
          <li>Install environment.yml: <pre>conda env create -f environment.yml</pre></li>
          <li>Close the terminal window.</li>
		</ol>
      </article>
      <article role="tabpanel" class="tab-pane active" id="python-packages-linux">
        <ol>
          <li>Open a terminal</li>
          <li>Download <a href="environment.yml">environment.yml</a></li>
          <li>Install environment.yml: <pre>conda env create -f environment.yml</pre></li>
          <li>Close the terminal window</li>
        </ol>
      </article>
    </div>
  </div>
For more information, refer to <a href="http://docs.anaconda.com/anaconda/navigator/tutorials/manage-environments/">Managing environments</a> in the Anaconda documentation.
</div>


<div id="r"> {% comment %} Start of 'R' section. {% endcomment %}
  <h3>R</h3>

  <p>
    <a href="https://www.r-project.org">R</a> is a programming language
    that is especially powerful for data exploration, visualization, and
    statistical analysis. To interact with R, we use
    <a href="https://www.rstudio.com/">RStudio</a>.
  </p>
  <p>To install R and rstudio, use <a href="#anaconda">Anaconda navigator</a> and
  follow <a href="https://docs.anaconda.com/anaconda/navigator/tutorials/create-r-environment/">these instructions</a>
  to create a conda <b>R</b> environment called <b>esm-r-analysis</b>.
  </p>

</div> {% comment %} End of 'R' section. {% endcomment %}

<div id="r-libraries"> {% comment %} Start of 'R' section. {% endcomment %}
  <h3>Install additional R libraries</h3>

The following <pre>R</pre> packages are used in the lessons.

<ul>
<li><a href="https://cran.r-project.org/package=dplyr">dplyr</a></li>
<li><a href="https://cran.r-project.org/package=ggplot2">ggplot2</a></li>
<li><a href="https://cran.r-project.org/package=raster">raster</a></li>
<li><a href="https://cran.r-project.org/package=rgdal">rgdal</a></li>
<li><a href="https://cran.r-project.org/package=rasterVis">rasterVis</a></li>
<li><a href="https://cran.r-project.org/package=remotes">remotes</a></li>
<li><a href="https://cran.r-project.org/package=sf">sf</a></li>
<li><a href="https://cran.r-project.org/package=ncdf4">ncdf4</a></li>
<li><a href="https://cran.r-project.org/package=tmap">tmap</a></li>
<li><a href="https://cran.r-project.org/package=mapview">mapview</a></li>
<li><a href="https://cran.r-project.org/package=maps">maps</a></li>
<li><a href="https://cran.r-project.org/package=plotly">plotly</a></li>
<li><a href="https://cran.r-project.org/package=leaflet">leaflet</a></li>
<li><a href="https://cran.r-project.org/web/packages/ecmwfr/">ecmwfr</a></li>
</ul>

  Start RStudio with Anaconda Navigator and the newly created R environment. Then install the following packages:

  <pre>
  install.packages(c("installr","dplyr", "ggplot2", "raster", "rgdal", "rasterVis", "sf", "ncdf4", "tmap", "mapview", "maps", "plotly", "leaflet", "ecmwfr"))
  </pre>

</div>

{% include links.md %}