# Huomioita

## Webdevaajan vala

Aina console auki devatessa. Siellä on paljon elämää helpottavia toimintoja.

## Lomakkeet

### input

`<input>` elementit tarvitsee aina `name` attribuutin.

Ei toimi:
```html
<label for="example">Esimerkki</label>
<input type="text" id="example" />
```

Toimii:
```html
<label for="example">Esimerkki</label>
<input type="text" id="example" name="example" />
```

Name attribuutin perusteella lomakkeen tiedot lähetetään avain-arvo pareina palvelimelle.

Lomake lähettää suurinpiirtein tämän kaltaista dataa palvelimelle:

```
username: windows95man
name: pelle peloton
password: windows3.11rules
email: man@windows.com
```

Jos name attribuutti puuttuu, lomake vastaanotetaan puutteellisena. Esim jos username ja name on unohtunut, lähtee lomake palvelimelle tälläisena:

```
password: windows3.11rules
email: man@windows.com
```


### form

Muistetaan `<form>` tagissa `action` ja `method` attribuutit.


## Selainten erot

Kuten huomattiin, chrome, firefox, safari kaikki käyttäytyy hieman eri tavalla, vaikka samaa standardia hyödyntävät. CSS:n puolella eroavaisuuksia voi pienentää css resetin / normalize css:n avulla. Tätä ei sen kummemmin käyty läpi, googlesta löytyy.
