---
layout: default
title: "The atomic web toolkit for pragmatists"
---

{% capture example_profile %}
<div class="card ~neutral !low md:flex max-w-lg">
  <div class="w-20 h-20 mx-auto mb-6 md:mr-6 flex-shrink-0">
    <img class="object-cover rounded-full" src="{{ '/assets/profile_image.png' | relative_url }}">
  </div>
  <div class="flex-grow text-center md:text-left">
    <p class="support">Senior Researcher</p>
    <h3 class="text-xl heading">Dr. Katya Hattenagh</h3>
    <p class="mt-2 mb-3">Katya studies the intersection of machine learning and differential topology.</p>
    <div>
      <span class="chip ~neutral mb-1">Discrete Math</span> <span class="chip ~neutral mb-1">Topology</span> <span
        class="chip ~neutral mb-1">Neural Nets</span>
    </div>
  </div>
</div>
{% endcapture %}

{% capture example_table %}
<table class="table">
  <thead>
    <tr>
      <th>Name</th>
      <th>Status</th>
      <th>Price</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Landinator 9000 <span class="badge ~neutral">New</span></td>
      <td><span class="chip ~positive">Completed</span></td>
      <td>$300</td>
    </tr>
    <tr>
      <td>Hammer</td>
      <td><span class="chip ~urge">Waiting</span></td>
      <td>$20</td>
    </tr>
    <tr>
      <td>Computer</td>
      <td><span class="chip ~info">Processing</span></td>
      <td>$500</td>
    </tr>
  </tbody>
</table>
{% endcapture %}

{% capture example_form %}
<form class="card ~neutral !low">
  <div class="mb-4">
    <label class="label" for="toolkit">Current job</label>
    <div class="select ~neutral !low my-1 max-w-xs">
      <select>
        <option>Teacher</option>
        <option>Engineer</option>
        <option>Firefighter</option>
        <option>Other</option>
      </select>
    </div>
    <p class="support">If you don't currently have a job, select 'other.'</p>
  </div>
  <div>
    <label class="label" for="toolkit">Favorite toolkit</label>
    <input id="toolkit" type="text" class="input ~critical !normal my-1 max-w-xs block" placeholder="At least 8 characters..."
      value="Not a17t">
    <p class="support ~critical">The correct answer is a17t!</p>
  </div>
</form>
{% endcapture %}

{% capture example_delete %}
<div class="card ~neutral !low p-0 max-w-sm">
  <div class="p-4">
    <h2 class="mb-1 text-lg heading">Just making sure!</h2>
    <p class="mb-3 text-base support">To confirm you'd like to delete this repository, please enter its name below.</p>
    <input class="input" type="text" placeholder="milesmcc/a17t">
  </div>
  <section class="section ~critical p-4">
    <span class="button ~critical !high">Delete</span>
    <span class="button ~neutral bg-transparent">Go Back</span>
  </section>
</div>
{% endcapture %}

<div class="items-center justify-between mb-24 md:flex md:mt-24">
  <section class="mt-6 mb-12 mr-6 md:w-6/12">
    <h2 class="text-lg heading md:text-3xl">
      a17t, <i>noun</i> <span class="text-neutral-400">(ey&#712;seven&#712;teen&#712;tee) &mdash;</span><br>
    </h2>
    <h1 class="mb-4 text-4xl heading md:text-5xl text-urge-600">
      atomic design toolkit
    </h1>
    <h3 class="mb-6 text-lg subheading md:text-xl font-primary">Build beautiful, unique interfaces
    without reinventing the wheel. Let a17t provide
      the core building blocks, then customize with ease.</h3>
    <div>
      <ul class="text-lg">
        <li class="portal ~urge active"><a href="#install">Start</a></li>
        <li class="portal"><a href="#design">Principles</a></li>
        <li class="portal"><a href="#concepts">Concepts</a></li>
      </ul>
    </div>
  </section>
  <section class="md:w-5/12">
    <img src="{{'/assets/main_code_demo.png'|relative_url}}" class="rounded" alt="a17t code demo">
  </section>
</div>

<hr class="h-12 sep">

<section class="md:flex">
  <div class="lg:w-9/12">
    <article class="md:flex">
      <aside class="self-start hidden w-3/12 mb-4 md:block mh-auto md:sticky md:pr-12 md:text-right" style="top: 2rem;">
        <p class="text-2xl heading text-urge-600">Overview</p>
      </aside>
      <div class="md:w-9/12 content">
        <h2>Core interface elements. <br> No opinions about anything else.</h2>
        <p>Some CSS frameworks come prepackaged with all sorts of components that are convenient
          at first but quickly become limiting. Utility frameworks like Tailwind are awesome, but
          can be difficult start using on their own.</p>
        <p>a17t tries to get the balance right. Instead of providing all-inclusive, opinionated components (like
          jumbotrons, navbars, and menus), a17t provides common single-class elements in a default (but easily
          customizable) style.
        </p>
      </div>
    </article>
    <hr class="h-16 sep">
    <article class="justify-end md:flex">
      <div class="md:w-9/12 md:max-w-full">
        {% include example.html code=example_form label=true classes="bg-neutral-100" %}
      </div>
    </article>
    <hr class="h-16 sep">
    <article class="md:flex" id="design">
      <aside class="self-start mb-4 md:w-3/12 mh-auto md:sticky md:pr-12 md:text-right" style="top: 2rem;">
        <p class="mb-8 text-3xl heading text-urge-600 md:text-2xl">Design Principles</p>
      </aside>
      <div class="md:w-9/12">
        <section class="grid-cols-2 gap-8 md:grid">
          <div class="mb-6">
            <span class="shield ~info float-right ml-1 mb-1">
              <span class="icon">
                <i class="fas fa-atom fa-lg"></i>
              </span>
            </span>
            <h4 class="mb-1 text-xl heading">Atomic &amp; flexible</h4>
            <p>a17t provides core, single-class interface elements and empowers you to assemble them your way. And
              everything is easily customizable using CSS variables, so you'll never need to settle for &ldquo;good
              enough.&rdquo;
            </p>
          </div>
          <div class="mb-6">
            <span class="float-right shield ~positive ml-1 mb-1">
              <span class="icon">
                <i class="fas fa-brain fa-lg"></i>
              </span>
            </span>
            <h4 class="mb-1 text-xl heading">Logical &amp; hierarchical</h4>
            <p>a17t encourages you to think in terms of intent and hierarchy by specifying elements in terms of tone
              and priority. As an added bonus, this makes refactoring and customization a breeze.</p>
          </div>
          <div class="mb-6">
            <span class="float-right shield ~critical ml-1 mb-1">
              <span class="icon">
                <i class="fas fa-feather fa-lg"></i>
              </span>
            </span>
            <h4 class="mb-1 text-xl heading">Lightweight &amp; modern</h4>
            <p>a17t has no dependencies. That means it's reliable, customizable,
              and can integrate with any JS stack. Just import a small pure CSS file and you're good to go.</p>
          </div>
          <div class="mb-6">
            <span class="float-right shield ~urge ml-1 mb-1">
              <span class="icon">
                <i class="fas fa-smile-beam fa-lg"></i>
              </span>
            </span>
            <h4 class="mb-1 text-xl heading">Pleasant &amp; accessible</h4>
            <p>a17t is designed to make every interaction a delight. In addition to its semantic markup, a17t is full
              of subtle animations and accessibility features that make it pleasing for everyone to use.</p>
          </div>
        </section>
      </div>
    </article>
    <hr class="h-16 sep">
    <article class="justify-end md:flex">
      <div class="md:w-9/12 md:max-w-full">
        {% include example.html code=example_profile label=true classes="bg-neutral-100" %}
      </div>
    </article>
    <hr class="h-16 sep">
    <article class="md:flex" id="concepts">
      <aside class="self-start mb-4 md:w-3/12 mh-auto md:sticky md:pr-12 md:text-right" style="top: 2rem;">
        <p class="mb-8 text-3xl heading text-urge-600 md:text-2xl">Concepts</p>
      </aside>
      <div class="md:w-9/12 content">
        <h2>Use tones to control color</h2>
        <p>There are six tones by default: neutral, positive, warning, critical, info, and urge. (Don't worry, these
          colors are all customizable.) Tones are specified using special class names that start with a tilde 
          (e.g., <code class="code">~positive</code>). To make a light green chip, for example, use <code class="code">chip
            ~positive</code>.</p>
        <h2>Use priorities to control prominence</h2>
        <p>There are three priorities &mdash; low, normal, and high. You can specify a
          priority by its class: an exclamation point followed by its name (e.g., <code class="code">!high</code> or
          <code class="code">!low</code>). Usually, priorities affect an elements' colors, but fallback to using elevation
          (communicated through drop shadow) when changing colors wouldn't look good.</p>
        <h2>Consider using with Tailwind</h2>
        <p>Because a17t only provides the core elements of your interface, like buttons and form inputs, you'll need a
          tool to stitch everything together. (a17t does not provide any grid utilities.) While you could do this using
          pure CSS, using a17t in conjunction with Tailwind makes for a very smooth and efficient development
          experience.</p>
      </div>
    </article>
    <hr class="h-16 sep">
    <article class="justify-end md:flex">
      <div class="md:w-9/12 md:max-w-full">
        {% include example.html label=true code=example_table %}
      </div>
    </article>
    <hr class="h-16 sep">
    <article class="md:flex">
      <aside class="self-start mb-4 md:w-3/12 mh-auto md:sticky md:pr-12 md:text-right" style="top: 2rem;">
        <p class="mb-8 text-3xl heading text-urge-600 md:text-2xl">More Benefits</p>
      </aside>
      <div class="md:w-9/12 content">
        <p><strong>Thoughtful typography</strong> &mdash; a17t is optimized for legibility. From headings to body text
          to labels, a17t tries to follow typographic best practices to ensure consistent, readable interfaces.</p>
        <p><strong>No margins</strong> &mdash; While most a17t elements have some kind of internal spacing, none have
          any external margin by default. This is intentional: spacing is not one-size-fits-all, so not having any makes
          a17t more flexible.</p>
        <p><strong>CSS variables</strong> &mdash; Unlike libraries built using preprocessing tools like Sass, a17t
          relies on CSS variables for customization. That means you can tweak it dynamically on the page without using
          any build tools.</p>
        <p><strong>Effortlessly responsive</strong> &mdash; All of a17t's elements are designed to look great on any
          kind of device. So as long as you build your layout responsively, a17t will automatically follow suit without
          any extra effort.</p>
      </div>
    </article>
    <hr class="h-16 sep">
    <article class="justify-end md:flex">
      <div class="md:w-9/12 md:max-w-full">
        {% include example.html code=example_delete label=true classes="bg-neutral-100" %}
      </div>
    </article>
    <hr class="h-16 sep">
    <article class="pb-12 md:flex" id="install">
      <aside class="self-start mb-4 md:w-3/12 mh-auto md:sticky md:pr-12 md:text-right" style="top: 2rem;">
        <p class="mb-8 text-3xl heading text-urge-600 md:text-2xl">Install</p>
      </aside>
      <div class="md:w-9/12">
        <p class="mb-2 label">Using NPM (recommended)</p>
        <div class="card ~neutral !high font-mono mb-4">
          npm install a17t
        </div>
        <p class="mb-2 content">Import a17t in your JavaScript using <code class="code">import 'a17t'</code> or into your preprocessed CSS using <code class="code">@import 'a17t';</code>. For more information about
          CSS-in-JS, see <a href="https://css-tricks.com/the-many-ways-to-include-css-in-javascript-applications/">
          this guide</a>. a17t's default export is simply its compiled CSS file, so you have no shortage of options
          to import it.</p>
        <p class="mb-6">Optionally use a17t's Tailwind distribution in your JavaScript with <code class="code">import 'a17t/dist/tailwind.css'</code> or in your CSS with <code class="code">@import 'a17t/dist/tailwind.css'</code>. The benefit of using a17t's Tailwind CSS distribution is that it uses the same CSS variables as a17t. That way, if you change your color scheme (for example), your Tailwind classes will change as well. (Note that the color names for a17t's Tailwind distribution match other a17t's naming system&mdash;e.g., the class for light grey text is `text-neutral-300`.)</p>
        <p class="mb-2 label">Using a CDN</p>
        <div class="card ~neutral !high font-mono mb-4 text-sm">
          &lt;link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/a17t@latest/dist/a17t.css"&gt;
        </div>
        <aside class="aside ~urge content">
          <p>
            <strong>Import a17t before Tailwind or other utility frameworks.</strong>
            That way, you'll easily be able to override a17t's defaults without fighting CSS's specificity logic.</p>
          <p>
            <strong>Use a CSS reset.</strong>
            To keep things modular and lightweight, a17t doesn't come with a CSS reset built-in. If you're not using
            Tailwind (which has a CSS reset built-in), make sure you use something like <a href="https://necolas.github.io/normalize.css/">Normalize.css</a>.
          </p>
          <p>
            <strong>Add <code class="code">~*</code> and <code class="code">!*</code> classes to your <a href="https://purgecss.com/safelisting.html">PurgeCSS class safelist</a>,
            if applicable.</strong> Because of an issue with PurgeCSS, it erroneously removes modifier classes that only set CSS variables (like <code class="code">~urge</code>
            and <code class="code">!low</code>). Add the following to your PurgeCSS config: <code class="code">safelistPatterns: [/^~/, /^!/]</code>.
          </p>
        </aside>
      </div>
    </article>
  </div>
  <div class="hidden pl-20 opacity-75 md:w-3/12 lg:block">
    {% include elements_list.html %}
  </div>
</section>

<hr class="sep">
