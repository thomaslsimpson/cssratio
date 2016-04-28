Simple ratios for CSS.

Ever wish you could just get your DIV's to be a locked ratio and stay that way. Well now you can!

You just specify the right class and the width (which can come from fixed sizes or a percentage) and the 
height of the container will be automatically set to maintain the correct ratio you selected.

You can poke aroudn in the code to find the start and stop points or change them.

And before you tell me, I do infact know that 1-2, 2-4, 3-6, and such are the same. I don't care
and you shouldn't worry either. I would rather put in a few extra characters and dodge the complaints
from non-math people. 

*If YOU would like to remove the duplicates in your own, it is simple enough: just make sure that 
you only output values where:  `max(w,h) / min(w,h)` is a whole number.*

Examples
========
```
<div class='SOMETHING-WITH-WIDTH'> <!-- this outside div should have a width specifier -->
	<div class='ratio-wrapper-WIDE-HIGH'> <!-- WIDE and HIGH are ratios from 1 to 16 e.g. '3-4' -->
		<div class='ration-wrapper-inner'> <!-- required -->
			<div>Content</div>
		</div>
	</div>
</div>
```

This is a simple was to set up fixed ration divs.


```
<div style='width:100px'> 
	<div class='ratio-wrapper-2-1'> 
		<div class='ration-wrapper-inner'> 
			<div>This will set itself to 50px</div>
		</div>
	</div>
</div>

<div style='width:50%'> 
	<div class='ratio-wrapper-2-1'> 
		<div class='ration-wrapper-inner'> 
			<div>This div will maintain the 2 to 1 ratio.</div>
		</div>
	</div>
</div>

```

