---


---

<h3 id="tartalomjegyzék">Tartalomjegyzék</h3>
<ul>
<li><a href="#id">id</a></li>
<li><a href="#name">name</a></li>
<li><a href="#description">description</a></li>
<li><a href="#price">price</a></li>
<li><a href="#images">images</a></li>
<li><a href="#category">category</a></li>
<li><a href="#discount_price">discount_price</a></li>
<li><a href="#attributes">attributes</a></li>
<li><a href="#delivery_cost">delivery_cost</a></li>
<li><a href="#p%C3%A9lda-xml">Példa xml</a></li>
</ul>
<h2 id="id">id</h2>
<pre class=" language-xml"><code class="prism  language-xml"><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>id</span><span class="token punctuation">&gt;</span></span>ABC123<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>id</span><span class="token punctuation">&gt;</span></span>
</code></pre>
<p>Ezt az azonosítót a saját webáruházából kell megadnia, hogy később betudja azonosítani melyik terméket rendelték meg illetve al terméket tudjon hozzáadni.<br>
Fontos, hogy egyedi azonosító legyen tehát ne ismétlődjön kétszer ugyanaz az azonosító.</p>
<h2 id="name">name</h2>
<pre class=" language-xml"><code class="prism  language-xml"><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>name</span><span class="token punctuation">&gt;</span></span>Fali polc<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>name</span><span class="token punctuation">&gt;</span></span>
</code></pre>
<p>Termék neve.</p>
<h2 id="description">description</h2>
<pre class=" language-xml"><code class="prism  language-xml"><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>description</span><span class="token punctuation">&gt;</span></span>Modern fali polc Stilista® márkájú termék sorozatból<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>description</span><span class="token punctuation">&gt;</span></span>
</code></pre>
<p>Termék leírása.</p>
<h2 id="price">price</h2>
<pre class=" language-xml"><code class="prism  language-xml"><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>price</span><span class="token punctuation">&gt;</span></span>12000<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>price</span><span class="token punctuation">&gt;</span></span>
</code></pre>
<p>Termék bruttó forintban értendő ára.</p>
<h2 id="discount_price">discount_price</h2>
<pre class=" language-xml"><code class="prism  language-xml"><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>discount_price</span><span class="token punctuation">&gt;</span></span>10000<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>discount_price</span><span class="token punctuation">&gt;</span></span>
</code></pre>
<p>Termék forintban értendő akciós ára.<br>
Ha a termékre nincs érvényes leárazás akkor a mezőt nem kell megadni.</p>
<h2 id="images">images</h2>
<pre class=" language-xml"><code class="prism  language-xml"><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>images</span><span class="token punctuation">&gt;</span></span>
   <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>image</span><span class="token punctuation">&gt;</span></span>https://example.com/image1.png<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>image</span><span class="token punctuation">&gt;</span></span>
   <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>image</span><span class="token punctuation">&gt;</span></span>https://example.com/image2.png<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>image</span><span class="token punctuation">&gt;</span></span>
   <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>image</span><span class="token punctuation">&gt;</span></span>https://example.com/image3.png<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>image</span><span class="token punctuation">&gt;</span></span>
<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>images</span><span class="token punctuation">&gt;</span></span>
</code></pre>
<p>A termékekhez való képeket itt lehet megadni.<br>
Minden képet külön <code>image</code> tag közé kell tenni.</p>
<h2 id="category">category</h2>
<pre class=" language-xml"><code class="prism  language-xml"><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>category</span><span class="token punctuation">&gt;</span></span>Bútor &gt; Nappali &gt; Fali polc<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>category</span><span class="token punctuation">&gt;</span></span>
</code></pre>
<p>A terméket itt kell besorolni egy kategória alá.</p>
<h2 id="attributes">attributes</h2>
<pre class=" language-xml"><code class="prism  language-xml"><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>attributes</span><span class="token punctuation">&gt;</span></span>
   <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>attribute</span><span class="token punctuation">&gt;</span></span>
      <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>name</span><span class="token punctuation">&gt;</span></span>Szín<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>name</span><span class="token punctuation">&gt;</span></span>
      <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>value</span><span class="token punctuation">&gt;</span></span>zöld<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>value</span><span class="token punctuation">&gt;</span></span>
   <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>attribute</span><span class="token punctuation">&gt;</span></span>
   <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>attribute</span><span class="token punctuation">&gt;</span></span>
      <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>name</span><span class="token punctuation">&gt;</span></span><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>name</span><span class="token punctuation">&gt;</span></span>
      <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>value</span><span class="token punctuation">&gt;</span></span>zöld<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>value</span><span class="token punctuation">&gt;</span></span>
   <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>attribute</span><span class="token punctuation">&gt;</span></span>
<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>attributes</span><span class="token punctuation">&gt;</span></span>
</code></pre>
<p>A termékekre vonatkozó tulajdonságok.</p>
<h2 id="delivery_cost">delivery_cost</h2>
<pre class=" language-xml"><code class="prism  language-xml"><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>delivery_cost</span><span class="token punctuation">&gt;</span></span>3000<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>delivery_cost</span><span class="token punctuation">&gt;</span></span>
</code></pre>
<p>A termék szállítási költsége.<br>
Az ár forintban értendő.</p>
<h2 id="példa-xml">Példa xml</h2>
<pre class=" language-xml"><code class="prism  language-xml"><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>products</span><span class="token punctuation">&gt;</span></span>
    <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>product</span><span class="token punctuation">&gt;</span></span>
        <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>product_id</span><span class="token punctuation">&gt;</span></span>ABC123<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>product_id</span><span class="token punctuation">&gt;</span></span>
        <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>name</span><span class="token punctuation">&gt;</span></span>Fali polc<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>name</span><span class="token punctuation">&gt;</span></span>
        <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>price</span><span class="token punctuation">&gt;</span></span>12500<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>price</span><span class="token punctuation">&gt;</span></span>
        <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>discount_price</span><span class="token punctuation">&gt;</span></span>10000<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>discount_price</span><span class="token punctuation">&gt;</span></span>
        <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>images</span><span class="token punctuation">&gt;</span></span>
            <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>image</span><span class="token punctuation">&gt;</span></span>https://example.com/image1.png<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>image</span><span class="token punctuation">&gt;</span></span>
            <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>image</span><span class="token punctuation">&gt;</span></span>https://example.com/image2.png<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>image</span><span class="token punctuation">&gt;</span></span>
            <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>image</span><span class="token punctuation">&gt;</span></span>https://example.com/image3.png<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>image</span><span class="token punctuation">&gt;</span></span>
        <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>images</span><span class="token punctuation">&gt;</span></span>
        <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>category</span><span class="token punctuation">&gt;</span></span>Bútor &gt; Nappali &gt; Fali polc<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>category</span><span class="token punctuation">&gt;</span></span>
        <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>attributes</span><span class="token punctuation">&gt;</span></span>
           <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>attribute</span><span class="token punctuation">&gt;</span></span>
                <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>name</span><span class="token punctuation">&gt;</span></span>Szín<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>name</span><span class="token punctuation">&gt;</span></span>
                <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>value</span><span class="token punctuation">&gt;</span></span>zöld<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>value</span><span class="token punctuation">&gt;</span></span>
            <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>attribute</span><span class="token punctuation">&gt;</span></span>
            <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>attribute</span><span class="token punctuation">&gt;</span></span>
                <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>name</span><span class="token punctuation">&gt;</span></span>Anyag<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>name</span><span class="token punctuation">&gt;</span></span>
                <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>value</span><span class="token punctuation">&gt;</span></span>MDF<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>value</span><span class="token punctuation">&gt;</span></span>
            <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>attribute</span><span class="token punctuation">&gt;</span></span>
        <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>attributes</span><span class="token punctuation">&gt;</span></span>
        <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>description</span><span class="token punctuation">&gt;</span></span>Modern fali polc Stilista® márkájú termék sorozatból VOLATO köszönhetően a lebegtető hatásnak gyönyörű kelléke lesz a szobának. Polc szélessége 3,8 cm és max. teherbírása 10 kg függően a fal anyagától, amelyre a polc el lesz helyezve.<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>description</span><span class="token punctuation">&gt;</span></span>
       <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>delivery_cost</span><span class="token punctuation">&gt;</span></span>3000<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>delivery_cost</span><span class="token punctuation">&gt;</span></span>
    <span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>product</span><span class="token punctuation">&gt;</span></span>
<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>products</span><span class="token punctuation">&gt;</span></span>
</code></pre>

