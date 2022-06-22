# Thrivecart-GTM-DataLayer-integration-change-GTM-ID-
Thrivecart GTM + DataLayer integration (change GTM ID)

#The following codes copy and paste in header section in Thrivecart All pages
<!-- Google Tag Manager -->
<script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
})(window,document,'script','dataLayer','GTM-XXXXXX');</script>
<!-- End Google Tag Manager -->

<script>
if(_thrive.offer){
var dataLayer = window.dataLayer || [];
dataLayer.push({
'event': _thrive.offer.type,
'ecommerce': {
'detail': {
'products': [{
'name': _thrive.offer.name,
'id': _thrive.offer.offer.id,
'price': _thrive.offer.price/100,
'category': _thrive.offer.type
}]
}
}
});
}
</script>

#Sources:
https://gist.github.com/measureschool/91b3f8d4a1c02ff5b611d9a8d652ebc5

https://measureschool.com/thrive-cart-tracking/

