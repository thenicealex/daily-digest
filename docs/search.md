---
layout: default
title: Search
---

<div id="lang-zh" class="lang-section" markdown="0">
  <h1>搜索历史摘要</h1>
  <div class="search-wrap">
    <input type="text" id="search-input-zh" class="search-input" placeholder="输入关键词…" autocomplete="off" />
    <span class="search-clear" id="clear-zh">✕</span>
  </div>
  <ul id="results-zh" class="search-results"></ul>
  <p id="no-results-zh" class="no-results" style="display:none">没有找到相关内容</p>
</div>

<div id="lang-en" class="lang-section" markdown="0">
  <h1>Search Archive</h1>
  <div class="search-wrap">
    <input type="text" id="search-input-en" class="search-input" placeholder="Type to search…" autocomplete="off" />
    <span class="search-clear" id="clear-en">✕</span>
  </div>
  <ul id="results-en" class="search-results"></ul>
  <p id="no-results-en" class="no-results" style="display:none">No results found</p>
</div>

<script src="https://unpkg.com/simple-jekyll-search@1.10.0/dest/simple-jekyll-search.min.js"></script>
<script>
(function () {
  var dataUrl = '{{ "/search.json" | relative_url }}';
  var tmplZh = '<li><a href="{url}"><span class="search-date">{date}</span>{title}</a><p class="search-excerpt">{content}</p></li>';
  var tmplEn = tmplZh;

  function initSearch(inputId, resultsId, noResultsId, lang) {
    SimpleJekyllSearch({
      searchInput: document.getElementById(inputId),
      resultsContainer: document.getElementById(resultsId),
      json: dataUrl,
      searchResultTemplate: lang === 'zh' ? tmplZh : tmplEn,
      noResultsText: '',
      limit: 20,
      fuzzy: false,
      templateMiddleware: function (prop, value, template) {
        if (prop === 'content') return value.slice(0, 120);
        return value;
      },
      filter: function (item) { return item.lang === lang; },
      success: function () {},
    });

    var input = document.getElementById(inputId);
    var noResults = document.getElementById(noResultsId);
    var results = document.getElementById(resultsId);
    var clear = document.getElementById('clear-' + lang);

    input.addEventListener('input', function () {
      clear.style.display = input.value ? 'inline' : 'none';
      setTimeout(function () {
        noResults.style.display = (input.value && results.children.length === 0) ? 'block' : 'none';
      }, 100);
    });

    clear.addEventListener('click', function () {
      input.value = '';
      input.dispatchEvent(new Event('input'));
      results.innerHTML = '';
      clear.style.display = 'none';
      noResults.style.display = 'none';
      input.focus();
    });
  }

  document.addEventListener('DOMContentLoaded', function () {
    initSearch('search-input-zh', 'results-zh', 'no-results-zh', 'zh');
    initSearch('search-input-en', 'results-en', 'no-results-en', 'en');
  });
})();
</script>
