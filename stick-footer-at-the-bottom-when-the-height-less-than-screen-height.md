```
<script>
function setSectionHeight() {
        if(document.body.offsetHeight < window.innerHeight) {
          var viewPortHeight = Math.max(document.documentElement.clientHeight, window.innerHeight || 0);
          document.getElementsByTagName('section')[0].style.height = viewPortHeight - document.getElementsByTagName('header')[0].clientHeight - document.getElementsByTagName('footer')[0].clientHeight + 'px';
        }
    }
    window.addEventListener('resize', setSectionHeight);
    setSectionHeight();
</script>
```
