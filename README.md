# \<splash-screen\>

Splash Screen element for Polymer v2 


#### Important

This element DOES NOT works with Polymer 1.x 

The 1.x version will be available soon

#### How to Use

Here is how to use the `<splash-screen>` element

`````
<splash-screen align="middle" show="true" background-style="#432" destroy="false">
    <img src="images/manifest/icon-48x48.png" class="center-aligned" slot="logo" alt="">
    <div slot="content">

        <!---Your custom html--->
    </div>

</splash-screen>
`````

#### Element Properties
##### `show` - `Boolean`

This is a boolean flag to cancel the splashcreen activity. Default `true`


##### `destroy` - `Boolean`

If you are planning to reuse the splashcreen, set this flag as `false`. Otherwise the element is destroyed. Default `false`


##### `background-style` - `String`

This flag accepts both hex strings, `url()` & default material color variables. Default `white`

##### `align` - `String`

This flag allows you to position your content of splashscreen in different positions. Here are the allowed values
- ###### middle `default`
- ###### middle-left
- ###### middle-right
- ###### top-left
- ###### top-right
- ###### top-middle
- ###### top-left
- ###### top-right


#### Slot properties

`<splash-screen>` element is composed using specific slots inside the element. Here are the slot names allowed
- `logo` - To set the logo image
- `content` - Here you can set the content that follows the logo

#### Viewing Your Element

```
$ polymer serve
```

#### Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.


#### Future work
- Add a slot for introducing custom dynamic background like `<canvas>` based animations
- Add custom animation behaviour to entire splash screen content (logo and content)
- Introduce spinner slots with custom positioning


#### Licence
##### Apache License 2.0
