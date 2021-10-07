Explore this project at:

https://cipher387.github.io/osintmap/

![Worldwide OSINT Map](https://github.com/cipher387/osintmap/blob/main/osintmap.jpg)


<h1>What if you want to make a copy of the map with other points?</h1>

1. Go to https://developer.tech.yandex.ru/services/ and get the API-key for Yandex Maps API (for non-commercial use only).

2. When filling out the form, be sure to specify the site where you will use the map. The key will work only on the URL that is specified in the form. If you are going to put it on Github Pages, specify an address like https://cipher387.github.io/ (replace cipher387 with your username)

3. Fork (or download to you device) this repository and type your API-key in index.html</br> ![API Key](https://github.com/cipher387/osintmap/blob/main/apikey.jpg)

4. If you want to publish your map in Github Pages, just go to Settings->Pages and publish it! </br> ![API Key](https://github.com/cipher387/osintmap/blob/main/Githubpages.jpg)

5. About how to configure the map and add elements to it very clearly and intelligibly written in Yandex Maps Javascript API documentation https://yandex.com/dev/maps/jsbox/2.1/?from=jsapi

6. If you want just add some placemark, use this code example:</br>
```javascript
           .add(new ymaps.Placemark([53.709807, 27.953389], {
               balloonContentHeader: 'Belarus',
               balloonContent: 'Cadastral map</br><a href="https://map.nca.by/">map.nca.by</a></br>Business registry</br><a href="https://tsouz.belgiss.by/#!/tsouz/certifs">tsouz.belgiss.by</a>'
              }, {
               preset: 'islands#governmentCircleIcon',
               iconColor: '#ff0000'
            }))    
  
