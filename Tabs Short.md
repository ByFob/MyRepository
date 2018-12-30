# Tabs by WebMaster

<div class="wrapper">
    <div class="tabs">
        <span class="tab">Вкладка 1</span>
        <span class="tab">Вкладка 2</span>
        <span class="tab">Вкладка 3</span>        
    </div>
    <div class="tab_content">
        <div class="tab_item">Содержимое 1</div>
        <div class="tab_item">Содержимое 2</div>
        <div class="tab_item">Содержимое 3</div>
    </div>
</div>



$(".wrapper .tab").click(function() {
	$(".wrapper .tab").removeClass("active").eq($(this).index()).addClass("active");
	$(".tab_item").hide().eq($(this).index()).fadeIn()
}).eq(0).addClass("active");
