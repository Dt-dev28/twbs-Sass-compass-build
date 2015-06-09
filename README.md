# twbs-Sass-compass-build
to replicate font glyphicon render issue on browsers

The repository is a new HTML build upon SASS version of bootstrap usign compass

there is an issue with the glyphicons, they are not rendering up , what is show is just a hollow rectangle like it does on font-missing

The initial set up of twbs-sass is done according to https://github.com/twbs/bootstrap-sass#b-compass-without-rails

The bootstrap import structure is the same  as per recoomendation

// Import Bootstrap Compass integration
    @import "bootstrap-compass";

// Import custom Bootstrap variables
    @import "bootstrap-variables";

// Import Bootstrap for Sass
    @import "bootstrap";
// Import custom styles
    @import "custom";

In config.rb
relative_assets = true  si uncommneted

So, it gives the proper relative URL as "../fonts/bootstrap"

But still , chrome logs the error : Failed to decode downloaded font: http://127.0.0.1:63895/fonts/bootstrap/glyphicons-halflings-regular.ttf?1433513350 
            firefox logs the error : downloadable font: incorrect file size in WOFF header (font-family: "Glyphicons Halflings" style:normal weight:normal stretch:normal src index:2) source: file:///D:/Web_design_development/RESOURCES%20n%20TUTS/TEST%20project/SASS/trial/bootstrap-SassProject%20-prouductionTest/fonts/bootstrap/glyphicons-halflings-regular.woff?1433513350 styles.css:371:12
downloadable font: rejected by sanitizer (font-family: "Glyphicons Halflings" style:normal weight:normal stretch:normal src index:2) source: file:///D:/Web_design_development/RESOURCES%20n%20TUTS/TEST%20project/SASS/trial/bootstrap-SassProject%20-prouductionTest/fonts/bootstrap/glyphicons-halflings-regular.woff?1433513350

PS: I am quite new to using the SASS version of bootstrap specially with compass framework.
    Searched stackoverflow and many other forums, didn't worked and hence created a repositroy to  look  over it, and get resolute on this matter.

Three cheers to the solver !!!     

