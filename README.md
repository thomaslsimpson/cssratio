Simple ratios for CSS.

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

