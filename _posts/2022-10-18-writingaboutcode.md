---
keywords: fastai
title: Javascript code ( explaining )
toc: true
Badges: true
comments: false
author: Eli gilmour
Categories: [fastpages,javascript]
nb_path: _notebooks/2022-10-18-writingaboutcode.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-10-18-writingaboutcode.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>This code is creating an HTML table</p>
<ul>
<li>tr<ul>
<li>creating a row</li>
</ul>
</li>
<li>th<ul>
<li>creating an header</li>
</ul>
</li>
<li>table<ul>
<li>creating the shape of the table</li>
</ul>
</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-javascript"><pre><span></span><span class="c">&lt;!--</span> <span class="nx">HTML</span> <span class="nx">table</span> <span class="nx">fragment</span> <span class="k">for</span> <span class="nx">page</span> <span class="o">--&gt;</span>
<span class="o">&lt;</span><span class="nx">table</span><span class="o">&gt;</span>
  <span class="o">&lt;</span><span class="nx">thead</span><span class="o">&gt;</span>
  <span class="o">&lt;</span><span class="nx">tr</span><span class="o">&gt;</span>
    <span class="o">&lt;</span><span class="nx">th</span><span class="o">&gt;</span><span class="nx">Time</span><span class="o">&lt;</span><span class="err">/th&gt;</span>
    <span class="o">&lt;</span><span class="nx">th</span><span class="o">&gt;</span><span class="nx">All</span><span class="o">-</span><span class="nx">time</span> <span class="nx">Cases</span><span class="o">&lt;</span><span class="err">/th&gt;</span>
    <span class="o">&lt;</span><span class="nx">th</span><span class="o">&gt;</span><span class="nx">Recorded</span> <span class="nx">Deaths</span><span class="o">&lt;</span><span class="err">/th&gt;</span>
    <span class="o">&lt;</span><span class="nx">th</span><span class="o">&gt;</span><span class="nx">Active</span> <span class="nx">Cases</span><span class="o">&lt;</span><span class="err">/th&gt;</span>
  <span class="o">&lt;</span><span class="err">/tr&gt;</span>
  <span class="o">&lt;</span><span class="err">/thead&gt;</span>
  <span class="o">&lt;</span><span class="nx">tbody</span><span class="o">&gt;</span>
    <span class="o">&lt;</span><span class="nx">td</span> <span class="nx">id</span><span class="o">=</span><span class="s2">&quot;time&quot;</span><span class="o">&gt;&lt;</span><span class="err">/td&gt;</span>
    <span class="o">&lt;</span><span class="nx">td</span> <span class="nx">id</span><span class="o">=</span><span class="s2">&quot;total_cases&quot;</span><span class="o">&gt;&lt;</span><span class="err">/td&gt;</span>
    <span class="o">&lt;</span><span class="nx">td</span> <span class="nx">id</span><span class="o">=</span><span class="s2">&quot;total_deaths&quot;</span><span class="o">&gt;&lt;</span><span class="err">/td&gt;</span>
    <span class="o">&lt;</span><span class="nx">td</span> <span class="nx">id</span><span class="o">=</span><span class="s2">&quot;active_cases&quot;</span><span class="o">&gt;&lt;</span><span class="err">/td&gt;</span>
  <span class="o">&lt;</span><span class="err">/tbody&gt;</span>
<span class="o">&lt;</span><span class="err">/table&gt;</span>

<span class="o">&lt;</span><span class="nx">table</span><span class="o">&gt;</span>
  <span class="o">&lt;</span><span class="nx">thead</span><span class="o">&gt;</span>
  <span class="o">&lt;</span><span class="nx">tr</span><span class="o">&gt;</span>
    <span class="o">&lt;</span><span class="nx">th</span><span class="o">&gt;</span><span class="nx">Country</span><span class="o">&lt;</span><span class="err">/th&gt;</span>
    <span class="o">&lt;</span><span class="nx">th</span><span class="o">&gt;</span><span class="nx">All</span><span class="o">-</span><span class="nx">time</span> <span class="nx">Cases</span><span class="o">&lt;</span><span class="err">/th&gt;</span>
    <span class="o">&lt;</span><span class="nx">th</span><span class="o">&gt;</span><span class="nx">Recorded</span> <span class="nx">Deaths</span><span class="o">&lt;</span><span class="err">/th&gt;</span>
    <span class="o">&lt;</span><span class="nx">th</span><span class="o">&gt;</span><span class="nx">Active</span> <span class="nx">Cases</span><span class="o">&lt;</span><span class="err">/th&gt;</span>
  <span class="o">&lt;</span><span class="err">/tr&gt;</span>
  <span class="o">&lt;</span><span class="err">/thead&gt;</span>
  <span class="o">&lt;</span><span class="nx">tbody</span> <span class="nx">id</span><span class="o">=</span><span class="s2">&quot;result&quot;</span><span class="o">&gt;</span>
    <span class="c">&lt;!--</span> <span class="nx">generated</span> <span class="nx">rows</span> <span class="o">--&gt;</span>
  <span class="o">&lt;</span><span class="err">/tbody&gt;</span>
<span class="o">&lt;</span><span class="err">/table&gt;</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<ul>
<li>This code block is how it fetches the data for the covid cases from the api which is being taken from the backend.</li>
<li>The URl is where you access the api to use the data collected.</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-javascript"><pre><span></span><span class="c">&lt;!--</span> <span class="nx">Script</span> <span class="nx">is</span> <span class="nx">layed</span> <span class="nx">out</span> <span class="k">in</span> <span class="nx">a</span> <span class="nx">sequence</span> <span class="p">(</span><span class="nx">no</span> <span class="kd">function</span><span class="p">)</span> <span class="nx">and</span> <span class="nx">will</span> <span class="nx">execute</span> <span class="nx">when</span> <span class="nx">page</span> <span class="nx">is</span> <span class="nx">loaded</span> <span class="o">--&gt;</span>
<span class="o">&lt;</span><span class="nx">script</span><span class="o">&gt;</span>
  <span class="c1">// prepare HTML result container for new output</span>
  <span class="kr">const</span> <span class="nx">resultContainer</span> <span class="o">=</span> <span class="nb">document</span><span class="p">.</span><span class="nx">getElementById</span><span class="p">(</span><span class="s2">&quot;result&quot;</span><span class="p">);</span>

  <span class="c1">// prepare fetch options</span>
  <span class="kr">const</span> <span class="nx">url</span> <span class="o">=</span> <span class="s2">&quot;https://flask.nighthawkcodingsociety.com/api/covid/&quot;</span><span class="p">;</span>
  <span class="kr">const</span> <span class="nx">headers</span> <span class="o">=</span> <span class="p">{</span>
    <span class="nx">method</span><span class="o">:</span> <span class="s1">&#39;GET&#39;</span><span class="p">,</span> <span class="c1">// *GET, POST, PUT, DELETE, etc.</span>
    <span class="nx">mode</span><span class="o">:</span> <span class="s1">&#39;cors&#39;</span><span class="p">,</span> <span class="c1">// no-cors, *cors, same-origin</span>
    <span class="nx">cache</span><span class="o">:</span> <span class="s1">&#39;default&#39;</span><span class="p">,</span> <span class="c1">// *default, no-cache, reload, force-cache, only-if-cached</span>
    <span class="nx">credentials</span><span class="o">:</span> <span class="s1">&#39;omit&#39;</span><span class="p">,</span> <span class="c1">// include, *same-origin, omit</span>
    <span class="nx">headers</span><span class="o">:</span> <span class="p">{</span>
      <span class="s1">&#39;Content-Type&#39;</span><span class="o">:</span> <span class="s1">&#39;application/json&#39;</span>
      <span class="c1">// &#39;Content-Type&#39;: &#39;application/x-www-form-urlencoded&#39;,</span>
    <span class="p">},</span>
  <span class="p">};</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<ul>
<li>The code block is telling us how we get the data of the covid cases and then formatting it in a row and column. </li>
<li>It formats the countries name, cases, deaths, active cases in a row using the api.</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-javascript"><pre><span></span><span class="c1">// fetch the API</span>
 <span class="nx">fetch</span><span class="p">(</span><span class="nx">url</span><span class="p">,</span> <span class="nx">headers</span><span class="p">)</span>
 <span class="c1">// response is a RESTful &quot;promise&quot; on any successful fetch</span>
 <span class="p">.</span><span class="nx">then</span><span class="p">(</span><span class="nx">response</span> <span class="p">=&gt;</span> <span class="p">{</span>
   <span class="c1">// check for response errors</span>
   <span class="k">if</span> <span class="p">(</span><span class="nx">response</span><span class="p">.</span><span class="nx">status</span> <span class="o">!==</span> <span class="mf">200</span><span class="p">)</span> <span class="p">{</span>
       <span class="kr">const</span> <span class="nx">errorMsg</span> <span class="o">=</span> <span class="s1">&#39;Database response error: &#39;</span> <span class="o">+</span> <span class="nx">response</span><span class="p">.</span><span class="nx">status</span><span class="p">;</span>
       <span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="nx">errorMsg</span><span class="p">);</span>
       <span class="kr">const</span> <span class="nx">tr</span> <span class="o">=</span> <span class="nb">document</span><span class="p">.</span><span class="nx">createElement</span><span class="p">(</span><span class="s2">&quot;tr&quot;</span><span class="p">);</span>
       <span class="kr">const</span> <span class="nx">td</span> <span class="o">=</span> <span class="nb">document</span><span class="p">.</span><span class="nx">createElement</span><span class="p">(</span><span class="s2">&quot;td&quot;</span><span class="p">);</span>
       <span class="nx">td</span><span class="p">.</span><span class="nx">innerHTML</span> <span class="o">=</span> <span class="nx">errorMsg</span><span class="p">;</span>
       <span class="nx">tr</span><span class="p">.</span><span class="nx">appendChild</span><span class="p">(</span><span class="nx">td</span><span class="p">);</span>
       <span class="nx">resultContainer</span><span class="p">.</span><span class="nx">appendChild</span><span class="p">(</span><span class="nx">tr</span><span class="p">);</span>
       <span class="k">return</span><span class="p">;</span>
   <span class="p">}</span>
   <span class="c1">// valid response will have json data</span>
   <span class="nx">response</span><span class="p">.</span><span class="nx">json</span><span class="p">().</span><span class="nx">then</span><span class="p">(</span><span class="nx">data</span> <span class="p">=&gt;</span> <span class="p">{</span>
       <span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="nx">data</span><span class="p">);</span>
       <span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="nx">data</span><span class="p">.</span><span class="nx">world_total</span><span class="p">)</span>

       <span class="c1">// World Data</span>
       <span class="nb">document</span><span class="p">.</span><span class="nx">getElementById</span><span class="p">(</span><span class="s2">&quot;time&quot;</span><span class="p">).</span><span class="nx">innerHTML</span> <span class="o">=</span> <span class="nx">data</span><span class="p">.</span><span class="nx">world_total</span><span class="p">.</span><span class="nx">statistic_taken_at</span><span class="p">;</span>
       <span class="nb">document</span><span class="p">.</span><span class="nx">getElementById</span><span class="p">(</span><span class="s2">&quot;total_cases&quot;</span><span class="p">).</span><span class="nx">innerHTML</span> <span class="o">=</span> <span class="nx">data</span><span class="p">.</span><span class="nx">world_total</span><span class="p">.</span><span class="nx">total_cases</span><span class="p">;</span>
       <span class="nb">document</span><span class="p">.</span><span class="nx">getElementById</span><span class="p">(</span><span class="s2">&quot;total_deaths&quot;</span><span class="p">).</span><span class="nx">innerHTML</span> <span class="o">=</span> <span class="nx">data</span><span class="p">.</span><span class="nx">world_total</span><span class="p">.</span><span class="nx">total_deaths</span><span class="p">;</span>
       <span class="nb">document</span><span class="p">.</span><span class="nx">getElementById</span><span class="p">(</span><span class="s2">&quot;active_cases&quot;</span><span class="p">).</span><span class="nx">innerHTML</span> <span class="o">=</span> <span class="nx">data</span><span class="p">.</span><span class="nx">world_total</span><span class="p">.</span><span class="nx">active_cases</span><span class="p">;</span>

       <span class="c1">// Country data</span>
       <span class="k">for</span> <span class="p">(</span><span class="kr">const</span> <span class="nx">row</span> <span class="k">of</span> <span class="nx">data</span><span class="p">.</span><span class="nx">countries_stat</span><span class="p">)</span> <span class="p">{</span>
         <span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="nx">row</span><span class="p">);</span>

         <span class="c1">// tr for each row</span>
         <span class="kr">const</span> <span class="nx">tr</span> <span class="o">=</span> <span class="nb">document</span><span class="p">.</span><span class="nx">createElement</span><span class="p">(</span><span class="s2">&quot;tr&quot;</span><span class="p">);</span>
         <span class="c1">// td for each column</span>
         <span class="kr">const</span> <span class="nx">name</span> <span class="o">=</span> <span class="nb">document</span><span class="p">.</span><span class="nx">createElement</span><span class="p">(</span><span class="s2">&quot;td&quot;</span><span class="p">);</span>
         <span class="kr">const</span> <span class="nx">cases</span> <span class="o">=</span> <span class="nb">document</span><span class="p">.</span><span class="nx">createElement</span><span class="p">(</span><span class="s2">&quot;td&quot;</span><span class="p">);</span>
         <span class="kr">const</span> <span class="nx">deaths</span> <span class="o">=</span> <span class="nb">document</span><span class="p">.</span><span class="nx">createElement</span><span class="p">(</span><span class="s2">&quot;td&quot;</span><span class="p">);</span>
         <span class="kr">const</span> <span class="nx">active</span> <span class="o">=</span> <span class="nb">document</span><span class="p">.</span><span class="nx">createElement</span><span class="p">(</span><span class="s2">&quot;td&quot;</span><span class="p">);</span>

         <span class="c1">// data is specific to the API</span>
         <span class="nx">name</span><span class="p">.</span><span class="nx">innerHTML</span> <span class="o">=</span> <span class="nx">row</span><span class="p">.</span><span class="nx">country_name</span><span class="p">;</span>
         <span class="nx">cases</span><span class="p">.</span><span class="nx">innerHTML</span> <span class="o">=</span> <span class="nx">row</span><span class="p">.</span><span class="nx">cases</span><span class="p">;</span> 
         <span class="nx">deaths</span><span class="p">.</span><span class="nx">innerHTML</span> <span class="o">=</span> <span class="nx">row</span><span class="p">.</span><span class="nx">deaths</span><span class="p">;</span> 
         <span class="nx">active</span><span class="p">.</span><span class="nx">innerHTML</span> <span class="o">=</span> <span class="nx">row</span><span class="p">.</span><span class="nx">active_cases</span><span class="p">;</span> 

         <span class="c1">// this builds td&#39;s into tr</span>
         <span class="nx">tr</span><span class="p">.</span><span class="nx">appendChild</span><span class="p">(</span><span class="nx">name</span><span class="p">);</span>
         <span class="nx">tr</span><span class="p">.</span><span class="nx">appendChild</span><span class="p">(</span><span class="nx">cases</span><span class="p">);</span>
         <span class="nx">tr</span><span class="p">.</span><span class="nx">appendChild</span><span class="p">(</span><span class="nx">deaths</span><span class="p">);</span>
         <span class="nx">tr</span><span class="p">.</span><span class="nx">appendChild</span><span class="p">(</span><span class="nx">active</span><span class="p">);</span>

         <span class="c1">// add HTML to container</span>
         <span class="nx">resultContainer</span><span class="p">.</span><span class="nx">appendChild</span><span class="p">(</span><span class="nx">tr</span><span class="p">);</span>
       <span class="p">}</span>
   <span class="p">})</span>
<span class="p">})</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<ul>
<li>The code block below shows how the code catches fetch errors when the server is blocked.</li>
<li>So if tr or td has an error, the code will detect the error.</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-javascript"><pre><span></span><span class="c1">// catch fetch errors (ie ACCESS to server blocked)</span>
<span class="p">.</span><span class="k">catch</span><span class="p">(</span><span class="nx">err</span> <span class="p">=&gt;</span> <span class="p">{</span>
    <span class="nx">console</span><span class="p">.</span><span class="nx">error</span><span class="p">(</span><span class="nx">err</span><span class="p">);</span>
    <span class="kr">const</span> <span class="nx">tr</span> <span class="o">=</span> <span class="nb">document</span><span class="p">.</span><span class="nx">createElement</span><span class="p">(</span><span class="s2">&quot;tr&quot;</span><span class="p">);</span>
    <span class="kr">const</span> <span class="nx">td</span> <span class="o">=</span> <span class="nb">document</span><span class="p">.</span><span class="nx">createElement</span><span class="p">(</span><span class="s2">&quot;td&quot;</span><span class="p">);</span>
    <span class="nx">td</span><span class="p">.</span><span class="nx">innerHTML</span> <span class="o">=</span> <span class="nx">err</span><span class="p">;</span>
    <span class="nx">tr</span><span class="p">.</span><span class="nx">appendChild</span><span class="p">(</span><span class="nx">td</span><span class="p">);</span>
    <span class="nx">resultContainer</span><span class="p">.</span><span class="nx">appendChild</span><span class="p">(</span><span class="nx">tr</span><span class="p">);</span>
  <span class="p">});</span>
<span class="o">&lt;</span><span class="err">/script&gt;</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

</div>
 

