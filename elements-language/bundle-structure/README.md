---
description: An Element is a bundled folder
---

# Bundle Structure

Elements require a specific directory structure in order to work correctly, these are called Bundles in macOS.

Element bundles are directory hierarchies, with the top-level directory having a name that ends with a `.rwdevpack` extension.

The Pro version of RapidWeaver Elements is required to build and develop Elements.

### Dev Pack Bundle Structure

The following outlines the folder structure supported by elements — Only **bold items are required** for a basic Element to function inside of RapidWeaver.

{% hint style="info" %}
An Element pack can contain multiple Elements, each Element should be placed in the "elements" folder inside the main bundle.
{% endhint %}

* **HelloWorld.rwdevpack** (bundle)
* **elements** (folder)
* info.json
  * **com.realmac.elementpack.helloworld** (folder)
    * [hooks.js](broken-reference)
    * [**icon.icns**](icons.md)
    * icon-dark.icns
    * [**info.json**](info.json.md)
    * paletteIcon.png
    * paletteIcon-dark.png
    * [properties.json](broken-reference)
    * assets (folder)
      * page (folder)
    * **templates** (folder)
      * **each** (folder)
        * **index.html**
        * styles.css
      * [include](../templates/includes.md) (folder)
        * extra.html
      * page (folder)
        * page.html
  * com.realmac.elementpack.foobar (folder)
  * shared (folder)
    * assets (folder)
    * hooks (folder)
    * templates (folder)

Here's a Finder window showing a standard Element folder structure on macOS Ventura.

<figure><img src="../../.gitbook/assets/CleanShot 2023-05-31 at 14.08.03@2x.png" alt=""><figcaption><p>Finder window showing the layout of a typical Element.</p></figcaption></figure>

And the same Element being edited in [Visual Studio Code](https://code.visualstudio.com).

<figure><img src="../../.gitbook/assets/CleanShot 2023-05-31 at 14.26.45@2x.png" alt=""><figcaption><p>Editing an Element in Visual Studio Code</p></figcaption></figure>

### Dev Pack with Multiple Elements

An Element pack can have multiple addons inside of it, here's an example of that structure:

**WebWorld.rwdevpack** (bundle)

* **elements** (folder)
  * [**info.json**](info.json.md)
  * **com.realmac.elementpack.helloworld** (folder)
  * **com.realmac.elementpack.goodbyeworld** (folder)

