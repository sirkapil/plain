---
layout: default
title: Search
permalink: /search/
---
<div>

    <h2><a href="{{ site.url }}{{ page.url }}">Search</a></h2>
    <section>
		
    <form> <input type="text" id="search-input" placeholder="What are you looking for ?" />
    </form> </section>

</div>

<div class="search-results" id="results-container"></div>

<!-- Script pointing to jekyll-search.js -->
<script src="{{ site.url }}/trio/js/jekyll-search.min.js" type="text/javascript"></script>

<script type="text/javascript">
  SimpleJekyllSearch({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    json: '{{ site.url }}/search.json',
    searchResultTemplate: '<div class="single-search-result"><h2><a href="{url}" title="{desc}">{title}</a></h2><p>{snippet}</p><p class="date">{date}</p></div>',
    noResultsText: 'No results found',
    limit: 20,
    fuzzy: false
    // exclude: ['search']
})
</script>
