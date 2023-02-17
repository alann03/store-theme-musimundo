# Musimundo Store

<Musimundo Store> **Musimundo Store** es una imitación de la tienda [Musimundo](https://www.musimundo.com/), la cual fue creada con fines educativos utilizando la plataforma de desarrollo [VTEX IO](https://developers.vtex.com/docs/guides/welcome).

## Vista Previa

![Imagen Home](/assets/img/home-image.png)

## Configuración

### Paso 1 - Configuraciones básicas

Accede a la guía de [configuración básica](https://developers.vtex.com/docs/guides/vtex-io-documentation-2-basic-development-setup-in-vtex-io) de VTEX IO y sigue los pasos indicados. Al finalizar la configuración, debe tener instalada la interfaz de línea de comandos de VTEX ([Toolbelt](https://uxwriting.vtex.com/docs/text-patterns/toolbelt-cli/)) junto con un espacio de trabajo de desarrollador en el que puede trabajar.

### Paso 2 - Clonar el repositorio

Clona esta [plantilla](https://github.com/alann03/store-theme-musimundo) ← a tus archivos locales para poder empezar a trabajar en ella de manera efectiva. Luego, acceda al directorio del repositorio usando su terminal.

### Paso 3 - Editar el archivo Manifest.json

Una vez en el directorio del repositorio, es hora de editar el archivo `manifest.json`. Una vez dentro del archivo, debe reemplazar los valores del `vendor` y el `name`. El `vendor` es el nombre de la cuenta en la que está trabajando y `name` es cualquier nombre que desee para su tema. Por ejemplo:

```json
{
  "vendor": "store",
  "name": "store-theme"
}
```

### Paso 4 - Instalar las aplicaciones requeridas

Se deben instalar las siguientes aplicaciones:

- [VTEX Mega Menu](https://github.com/vtex-apps/mega-menu)

  ```bash
  vtex install vtex.mega-menu@2.x
  ```

- [VTEX Wish List](https://github.com/vtex-apps/wishlist)

  ```bash
  vtex install vtex.wish-list
  ```

### Paso 5 - Desinstalar cualquier tema existente

Al ejecutar el comando `vtex ls` puede verificar si algún tema está instalado.

```bash
 vtex ls
```

Es común tener instalado un vtex.store-theme cuando inicia el proceso de desarrollo de la tienda. Por lo tanto, si lo encuentra en la lista de aplicaciones, copie su nombre y versión, y utilícelo junto con el comando `vtex uninstall`. Por ejemplo:

```bash
 vtex uninstall vtex.store-theme@0.0.1
```

### Paso 6- Ejecutar y obtener una vista previa de su tienda

Ha llegado el momento de cargar todos los cambios que realizó en sus archivos locales a la plataforma. Para eso, use el comando `vtex link`.

```bash
vtex link
```

Si el proceso se ejecuta sin ningún error, deberá visualizar por consola el mensaje "_`App linked successfully`_".

Luego debe ejecutar el comando `vtex browse` para poder visualizar su tienda en el navegador.

```bash
vtex browse
```

Esto le permitirá ver los cambios aplicados en tiempo real, a través de la cuenta y el espacio de trabajo en el que está trabajando.

## Dependencias

```json
 "dependencies": {
    "vtex.store": "2.x",
    "vtex.store-header": "2.x",
    "vtex.product-summary": "2.x",
    "vtex.store-footer": "2.x",
    "vtex.store-components": "3.x",
    "vtex.styleguide": "9.x",
    "vtex.slider": "0.x",
    "vtex.carousel": "2.x",
    "vtex.shelf": "1.x",
    "vtex.menu": "2.x",
    "vtex.minicart": "2.x",
    "vtex.product-details": "1.x",
    "vtex.product-kit": "1.x",
    "vtex.search-result": "3.x",
    "vtex.login": "2.x",
    "vtex.my-account": "1.x",
    "vtex.flex-layout": "0.x",
    "vtex.rich-text": "0.x",
    "vtex.store-drawer": "0.x",
    "vtex.locale-switcher": "0.x",
    "vtex.product-quantity": "1.x",
    "vtex.product-identifier": "0.x",
    "vtex.product-specification-badges": "0.x",
    "vtex.product-review-interfaces": "1.x",
    "vtex.telemarketing": "2.x",
    "vtex.order-placed": "2.x",
    "vtex.stack-layout": "0.x",
    "vtex.tab-layout": "0.x",
    "vtex.responsive-layout": "0.x",
    "vtex.slider-layout": "0.x",
    "vtex.iframe": "0.x",
    "vtex.breadcrumb": "1.x",
    "vtex.sticky-layout": "0.x",
    "vtex.add-to-cart-button": "0.x",
    "vtex.store-image": "0.x",
    "vtex.modal-layout": "0.x",
    "vtex.product-price": "1.x",
    "vtex.overlay-layout": "0.x",
    "vtex.store-icons": "0.x",
    "vtex.store-link": "0.x",
    "vtex.checkout-summary": "0.x",
    "vtex.disclosure-layout": "1.x",
    "vtex.store-form": "0.x",
    "vtex.product-list": "0.x"
  }
```

```json
"peerDependencies": {
  "vtex.mega-menu": "2.x",
  "vtex.wish-list": "1.x"
}
```

### Aplicaciones customizadas

En esta tienda se realizaron los siguientes componentes customizados, que también deben incluirse en las dependencias.

```json
{
  "itgloberspartnercl.whatsapp-button": "0.x",
  "itgloberspartnercl.bullets-diagramation": "0.x",
  "itgloberspartnercl.add-to-cart-info": "0.x",
  "itgloberspartnercl.custom-department-search": "0.x",
  "itgloberspartnercl.pdf-reader": "0.x",
  "itgloberspartnercl.quick-order": "0.x",
  "itgloberspartnercl.special-diagramation": "0.x"
}
```

## Documentación a tener en cuenta

- [GitFlow](https://www.atlassian.com/es/git/tutorials/comparing-workflows/gitflow-workflow)

- [SemanticCommit](https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716)

## Colaboradores

- **Alan Agustín Huismann**
