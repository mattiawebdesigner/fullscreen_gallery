# fullscreen_gallery

Galleria fotografica gestita con jQuery. <br />
Per il corretto funzionamento della galleria va incluso jQuery.


La galleria si suddivide in due parti:

<ul>
  <li><strong>Parte 1: </strong> Gestisce l'elenco delle foto dell'album visualizzando anche il titolo e la descrizione. Se si clicca su una delle foto viene apero lo slideshow a tutto schermo.</li>
  <li><strong>Parte 2: </strong> Slideshow fullscreen
</ul>

<h3>Esempio d'uso</h3>

index.html
```` 
<!-- Elenco delle foto -->
<div id="album" class="gallery-index">
    <h1>Titolo dell'album</h1>
    
    <p class="description">
        Descrizione dell'album
    </p>
    
    <div class="container">
        <div class="row">
            <div data-image-position="0" class="foto col col-sm-5 col-md-3 col-lg-2"
                 style="background-image: url(<path_immagine>)">
            </div>
            <div data-image-position="1" class="foto col col-sm-5 col-md-3 col-lg-2"
                 style="background-image: url(<path_immagine>)">
            </div>
            <div data-image-position="2" class="foto col col-sm-5 col-md-3 col-lg-2"
                 style="background-image: url(<path_immagine>)">
            </div>
        </div>
    </div>
</div>

<!-- Slideshow -->
<div id="gallery" class="fullscreen">
    <div class="close">
        <i class="fas fa-times"></i>
    </div>
    
    <div class="wrap">
        <div class="relative">
            <div class="prev"><i class="fas fa-arrow-circle-left"></i></div>
            <div class="image" data-image-position="0" data-show="false">
                <div class="img-box">
                    <div class="img">
                        <img src="<path_immagine>" />
                    </div>
                </div>
                
                <div class="container-info">
                    <div class="description">
                        Descrizione dell'immagine
                    </div>
                </div>
            </div>
            
            <div class="image" data-image-position="1" data-show="false">
                <div class="img-box">
                    <div class="img">
                        <img src="<path_immagine>" />
                    </div>
                </div>
                
                <div class="container-info">
                    <div class="description">
                        Descrizione dell'immagine
                    </div>
                </div>
            </div>
            
            <div class="image" data-image-position="2" data-show="false">
                <div class="img-box">
                    <div class="img">
                        <img src="<path_immagine>" />
                    </div>
                </div>
                
                <div class="container-info">
                    <div class="description">
                        Descrizione dell'immagine
                    </div>
                </div>
            </div>
            <div class="next"><i class="fas fa-arrow-circle-right"></i></div>
        </div>
    </div>
</div>

<script type="text/javascript">
   jQuery("#gallery").fullscreen_gallery();
</scrip>
````





















