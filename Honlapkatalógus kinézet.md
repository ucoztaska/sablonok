# Honlapkatalógus kinézet

uCoz rendszerekben készített honlapkatalógusokhoz megfelelő kinézet. Az oldal címe és leírása mellett megtalálható az oldal ikonja és kisképe is.

Vezérlőpult >> Külalak vezérlése >> [honlapkatalógus alatt] Bejegyzések kinézete. A sablon tartalmát cseréljük le a a következőre: 

```html
<table border="0" cellpadding="0" cellspacing="0" width="100%" class="eBlock"><tr><td style="padding:3px;"><a href="$SITE_URL$" target="_blank"><img src="https://www.bitpixels.com/getthumbnail?code=91976&size=120&url=$SITE_DIRECT_URL$" title="$TITLE$" width="120" align="left" style="margin-right:5px;" /></a>  
<?if($MODER_PANEL$)?><div style="float:right">$MODER_PANEL$</div><?endif?>  
  <div class="eTitle" style="text-align:left;border:none;"><a target="_blank" href="$SITE_URL$"><img src="https://www.google.com/s2/favicons?domain=$SITE_DIRECT_URL$" width="16px" height="16px" align="left" style="margin-right:2px; margin-top:7px;" />$TITLE$</a></div><div class="eMessage" style="margin-top:4px;">$MESSAGE$</div></div>  
<div class="eDetails" style="clear:both;">  
<?if($RATING$)?><div style="float:right"><?$RSTARS$('12','/.s/img/stars/3/12.png','1','float')?></div><?endif?>  
<?if($CATEGORY_NAME$)?><span class="e-category"><span class="ed-value"><a href="$CATEGORY_URL$">$CATEGORY_NAME$</a></span></span><span class="ed-sep"> | </span><?endif?>  
<span class="e-redirects"><span class="ed-title">Látogatók:</span> <span class="ed-value">$REDIRECTS$</span></span>  
<?if($AUTHOR_NAME$)?><span class="ed-sep"> | </span> <span class="e-author"><span class="ed-title">Hozzáadta::</span> <span class="ed-value"><?if($AUTHOR_EMAIL_JS$)?><a href="$AUTHOR_EMAIL_JS$">$AUTHOR_NAME$</a><?else?>$AUTHOR_NAME$<?endif?></span></span><?endif?>  
<span class="ed-sep"> | </span> <span class="e-date"><span class="ed-title">Dátum:</span> <span title="$TIME$" class="ed-value">$DATE$</span></span>  
</div></td></tr></table>
```
