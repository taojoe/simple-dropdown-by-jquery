simple-dropdown-by-jquery
=========================

## Usage

see sample in the index.html

```html
	<div class="dropdown" style="margin-top:100px;">
	  <label>dropdown 2</label>
	  <ul>
		<li><a href="javascript:void(0);">aa</a></li>
		<li><a href="javascript:void(0);">aa</a></li>
	  </ul>
	</div>
<script>
$('.dropdown label').click(function(){
	var $ul=$(this).parent().children('ul');
	if($ul.is(':hidden')){
	    $ul.show();
	    setTimeout(function(){
	        $(document).one('click', function(){ $ul.hide();});
	    });
    }
});
</script>

```
