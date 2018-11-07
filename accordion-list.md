```
<script>
    (function () {
        var allPanels = $('.accordion .answer-content').hide();
        $('.accordion .answer > a').click(function() {
            if($(this).next().hasClass('show')) {
                $(this).next().removeClass('show');
                $(this).next().slideUp(350);
            } else {
                allPanels.removeClass('show');
                allPanels.slideUp(350);
                $(this).parent().find('.answer-content').toggleClass('show');
                $(this).parent().find('.answer-content').slideToggle(350);
            }
            return false;
        })
    })(jQuery);
</script>
```
