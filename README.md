# Relogio Digital
Relógio criado com html5, css e js.
Responsivo.

## Modelo Javascript

```javascript
    const horas = document.getElementById('horas');
    const minutos = document.getElementById('minutos');
    const segundos = document.getElementById('segundos');

    const relogio = setInterval(() => {
        let datadeHoje = new Date();
        let hora = datadeHoje.getHours();
        let minuto = datadeHoje.getMinutes();
        let segundo = datadeHoje.getSeconds();

        if (hora < 10) hora = '0' + hora;
        if (minuto < 10) minuto = '0' + minuto;
        if (segundo < 10) segundo = '0' + segundo;

        horas.textContent = hora;
        minutos.textContent = minuto;
        segundos.textContent = segundo;
})
```

## Captura de Tela

![CapturadeTela](https://github.com/luannsct/RelogioDigital/assets/34097627/bd345f5f-e43f-4d1d-acf9-ac5df23c2a95)

