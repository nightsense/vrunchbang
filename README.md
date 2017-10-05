<h1 id="vrunchbang">vrunchbang</h1>

<p>A vim theme inspired by the <a href="https://distrowatch.com/table.php?distribution=crunchbang">CrunchBang</a> Linux distribution (now <a href="https://www.bunsenlabs.org/">BunsenLabs</a>).</p>

<h2 id="screenshots">screenshots</h2>

<table>
<tr></tr><tr><td align="center"><strong>vrunchbang-<br />light</strong></td>
<td align="center"><img src="/img/screenshot-vrunchbang-light.png" alt="screenshot of the vrunchbang-light vim theme" width="288" /> <img src="/img/screenshot-vrunchbang-dark.png" alt="screenshot of the vrunchbang-dark vim theme" width="288" /></td>
<td align="center"><strong>vrunchbang-<br />dark</strong></td></tr>
</table>

<h2 id="setup">setup</h2>

<h3 id="installation">installation</h3>

<p>While themes can be installed manually (by placing a <a href="https://github.com/nightsense/vrunchbang/tree/master/colors">theme file</a> in <code class="highlighter-rouge">~/.vim/colors/</code>), a <strong>plugin helper</strong> is recommended.</p>

<p>If you don’t have a preferred helper, consider trying <a href="https://github.com/junegunn/vim-plug">vim-plug</a>, which can be installed with:</p>

<div class="highlighter-rouge"><pre class="highlight"><code>curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
</code></pre>
</div>

<p>To install vrunchbang via vim-plug, add the following to the top of your <code class="highlighter-rouge">vimrc</code>:</p>

<div class="highlighter-rouge"><pre class="highlight"><code>call plug#begin('~/.vim/plugged')
Plug 'nightsense/vrunchbang'
call plug#end()
</code></pre>
</div>

<p>Then restart vim and run <code class="highlighter-rouge">PlugUpdate</code> (from the vim command line).</p>

<h3 id="activation">activation</h3>

<p>To activate the vrunchbang theme, add one of the following lines to your <code class="highlighter-rouge">vimrc</code>:</p>

<ul>
  <li><code class="highlighter-rouge">colorscheme vrunchbang-light</code></li>
  <li><code class="highlighter-rouge">colorscheme vrunchbang-dark</code></li>
</ul>

<p>Note that the <code class="highlighter-rouge">background</code> setting doesn’t affect this theme.</p>

<blockquote>
  <p>To assign themes to specific intervals of the day, try the <a href="https://github.com/nightsense/night-and-day">night-and-day</a> plugin.</p>
</blockquote>

<h2 id="terminal-vim">terminal vim</h2>

<p>See the <a href="https://github.com/nightsense/nightshell">nightshell</a> repository, which allows vrunchbang to be used in a variety of terminal applications.</p>

<h2 id="design">design</h2>

<h3 id="palette">palette</h3>

<p>vrunchbang consists of 16 colours:</p>

<ul>
  <li>8 theme-distinct <strong>base colours</strong>, which meet the <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast.html#visual-audio-contrast-contrast-73-head">3:1 ISO standard</a> for text/background contrast ratio</li>
  <li>a hand-tuned selection of 8 <strong>accent colours</strong>, common to the nightsense theme family, for syntax highlighting
    <ul>
      <li>hue selection was made at the coarse scale of 1/12 (30°) colour wheel intervals, followed by adjustment on a fine scale of 1/12 subintervals</li>
      <li>value and saturation were manually tuned for light backgrounds, then saturation was lowered for dark backgrounds</li>
      <li>again, ISO contrast ratio was observed</li>
    </ul>
  </li>
</ul>

<table>
  <thead>
    <tr>
      <th style="text-align: right">base colours</th>
      <th style="text-align: center">light-background accents</th>
      <th style="text-align: left">dark-background accents</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: right"><img src="http://www.colorhexa.com/191d1f.png" height="24" width="42" /> <code class="highlighter-rouge">191d1f</code> </td>
      <td style="text-align: center"><img src="http://www.colorhexa.com/ff453f.png" height="24" width="42" /> <code class="highlighter-rouge">ff453f</code> </td>
      <td style="text-align: left"><img src="http://www.colorhexa.com/ff5a54.png" height="24" width="42" /> <code class="highlighter-rouge">ff5a54</code></td>
    </tr>
    <tr>
      <td style="text-align: right"><img src="http://www.colorhexa.com/282e30.png" height="24" width="42" /> <code class="highlighter-rouge">282e30</code> </td>
      <td style="text-align: center"><img src="http://www.colorhexa.com/eb6d13.png" height="24" width="42" /> <code class="highlighter-rouge">eb6d13</code> </td>
      <td style="text-align: left"><img src="http://www.colorhexa.com/eb8f4e.png" height="24" width="42" /> <code class="highlighter-rouge">eb8f4e</code></td>
    </tr>
    <tr>
      <td style="text-align: right"><img src="http://www.colorhexa.com/444e52.png" height="24" width="42" /> <code class="highlighter-rouge">444e52</code> </td>
      <td style="text-align: center"><img src="http://www.colorhexa.com/ffdb00.png" height="24" width="42" /> <code class="highlighter-rouge">ffdb00</code> </td>
      <td style="text-align: left"><img src="http://www.colorhexa.com/ebd43b.png" height="24" width="42" /> <code class="highlighter-rouge">ebd43b</code></td>
    </tr>
    <tr>
      <td style="text-align: right"><img src="http://www.colorhexa.com/5d6b70.png" height="24" width="42" /> <code class="highlighter-rouge">5d6b70</code> </td>
      <td style="text-align: center"><img src="http://www.colorhexa.com/289e37.png" height="24" width="42" /> <code class="highlighter-rouge">289e37</code> </td>
      <td style="text-align: left"><img src="http://www.colorhexa.com/5c9e65.png" height="24" width="42" /> <code class="highlighter-rouge">5c9e65</code></td>
    </tr>
    <tr>
      <td style="text-align: right"><img src="http://www.colorhexa.com/999999.png" height="24" width="42" /> <code class="highlighter-rouge">999999</code> </td>
      <td style="text-align: center"><img src="http://www.colorhexa.com/1b9e93.png" height="24" width="42" /> <code class="highlighter-rouge">1b9e93</code> </td>
      <td style="text-align: left"><img src="http://www.colorhexa.com/5c9e99.png" height="24" width="42" /> <code class="highlighter-rouge">5c9e99</code></td>
    </tr>
    <tr>
      <td style="text-align: right"><img src="http://www.colorhexa.com/bfbfbf.png" height="24" width="42" /> <code class="highlighter-rouge">bfbfbf</code> </td>
      <td style="text-align: center"><img src="http://www.colorhexa.com/3292c9.png" height="24" width="42" /> <code class="highlighter-rouge">3292c9</code> </td>
      <td style="text-align: left"><img src="http://www.colorhexa.com/75aac9.png" height="24" width="42" /> <code class="highlighter-rouge">75aac9</code></td>
    </tr>
    <tr>
      <td style="text-align: right"><img src="http://www.colorhexa.com/e8e8e8.png" height="24" width="42" /> <code class="highlighter-rouge">e8e8e8</code> </td>
      <td style="text-align: center"><img src="http://www.colorhexa.com/8a54c9.png" height="24" width="42" /> <code class="highlighter-rouge">8a54c9</code> </td>
      <td style="text-align: left"><img src="http://www.colorhexa.com/a687c9.png" height="24" width="42" /> <code class="highlighter-rouge">a687c9</code></td>
    </tr>
    <tr>
      <td style="text-align: right"><img src="http://www.colorhexa.com/ffffff.png" height="24" width="42" /> <code class="highlighter-rouge">ffffff</code> </td>
      <td style="text-align: center"><img src="http://www.colorhexa.com/e05e95.png" height="24" width="42" /> <code class="highlighter-rouge">e05e95</code> </td>
      <td style="text-align: left"><img src="http://www.colorhexa.com/e082a9.png" height="24" width="42" /> <code class="highlighter-rouge">e082a9</code></td>
    </tr>
  </tbody>
</table>

<h3 id="syntax-highlighting-logic">syntax highlighting logic</h3>

<p><img src="http://www.colorhexa.com/ff453f.png" height="24" width="42" />
<strong>Red</strong>, the colour of alarm, is used for <strong>warning elements</strong>, including error messages, misspellings, and diff deletions.</p>

<p><img src="http://www.colorhexa.com/eb6d13.png" height="24" width="42" />
<strong>Orange</strong> is the colour of fire, which serves as a preliminary to many practical activities. Orange is therefore used for <strong>preliminary elements</strong>, such as preprocessor commands (which prepare data to be handled by another program), incremental searching (that is, a search term in the process of being typed), titles, and miscapitalized words.</p>

<p><img src="http://www.colorhexa.com/ffdb00.png" height="24" width="42" />
<strong>Yellow</strong>, the classic highlighting colour, is applied to elements that are not warnings yet should draw attention with high visibility. These <strong>highlighted elements</strong> include search results, task tags (<code class="highlighter-rouge">TODO</code>, <code class="highlighter-rouge">FIXME</code>…), and diff changes.</p>

<p><img src="http://www.colorhexa.com/289e37.png" height="24" width="42" />
<strong>Green</strong>, the colour that says “go ahead, proceed with the task at hand”, is used for positive <strong>action elements</strong>, such as statements (if/then, while/do, case…), mode indicators (insert, visual…), vim user prompts, and diff additions.</p>

<p><img src="http://www.colorhexa.com/1b9e93.png" height="24" width="42" />
<strong>Teal</strong> is named after the “common teal”, a kind of duck, thus connecting this colour with the concept of “species”, which is a means of classifying life into very specific types. Teal is therefore used for specifying <strong>object types</strong>, such as data type (boolean, integer, string…) or storage class (static, volatile…), as well as mislocalized words (that is, words that are not misspelled but of the wrong type, namely a foreign type).</p>

<p><img src="http://www.colorhexa.com/3292c9.png" height="24" width="42" />
<strong>Blue</strong>, a colour of calm stability, is used for <strong>constants</strong>, which come in the form of boolean values, integers, floating-point numbers, characters, and strings.</p>

<p><img src="http://www.colorhexa.com/8a54c9.png" height="24" width="42" />
<strong>Purple</strong>, often associated with rare purple dyes historically produced for special works of art, is used for <strong>special text</strong>, including special characters (standalone or within syntax units), vim tags, and debugging statements. Rarely-used words are also marked, allowing the writer to consider whether such a specially uncommon word is appropriate.</p>

<p><img src="http://www.colorhexa.com/e05e95.png" height="24" width="42" />
<strong>Pink</strong>, the colour of spring blossoms, is used for <strong>object names</strong>, including the names of variables and functions. To code is to bring countless objects blossoming into existence as one types their names.</p>
