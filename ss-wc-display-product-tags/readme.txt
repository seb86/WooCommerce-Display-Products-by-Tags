=== WooCommerce Display Products by Tags ===
Contributors:         sebsstudio, sebd86
Donate link:          http://www.sebastiendumont.com/donation/
Tags:                 woocommerce, products, tags, taxonomy, filter
Requires at least:    4.2
Tested up to:         4.2.2
Stable tag:           1.0.0
License:              GPLv2 or later
License URI:          http://www.gnu.org/licenses/gpl-2.0.html

Display WooCommerce products by tags using a shortcode.

== Description ==
This shortcode is much like the product category shortcode. The attributes are the same also, the only difference is that you can display WooCommerce products by product tags instead.

= Contributing and reporting bugs =
You can contribute code to this plugin via GitHub: https://github.com/Sebs-Studio/WooCommerce-Display-Products-by-Tags

= Support =
Use the WordPress.org forums for [community support](https://wordpress.org/support/plugin/woocommerce-display-products-by-tags). If you spot a bug, you can of course log it on [Github](https://github.com/Sebs-Studio/WooCommerce-Display-Products-by-Tags/issues) instead where I can act upon it more efficiently.

Please consider making a [donation](http://www.sebastiendumont.com/donation/) or [write a review](https://wordpress.org/support/view/plugin-reviews/woocommerce-customer-notes-to-completed-order-emails?rate=5#postform).

**More information**

- Other [WordPress plugins](http://profiles.wordpress.org/sebsstudio/) by [Sebs Studio](http://www.sebs-studio.com/)
- Contact Sebastien on Twitter: [@sebsstudio](http://twitter.com/sebsstudio)
- If you're a developer yourself, follow or contribute to the [WooCommerce Display Products by Tags plugin on GitHub](https://github.com/Sebs-Studio/WooCommerce-Display-Products-by-Tags)

== Installation ==
Installing "WooCommerce Display Products by Tags" can be done either by searching for "WooCommerce Display Products by Tags" via the "Plugins > Add New" screen in your WordPress dashboard, or by using the following steps:

1. Download the plugin via WordPress.org
2. Upload the ZIP file through the 'Plugins > Add New > Upload' screen in your WordPress dashboard.
3. Activate the plugin through the 'Plugins' menu in WordPress.

== Frequently Asked Questions ==

= Q.1 How do I display products by tags? =

A.1 Simple add this shortcode with the product tags you wish to filter by. e.g. ```[product_tag tags="shoes,socks"]```

= Q.2 What are the attributes? =

A.2 You can use the following attributes.
`
array(
  'per_page' => '12',
  'columns'  => '4',
  'orderby'  => 'title',
  'order'    => 'asc',
  'tags'     => '',  // Product Tag Slugs
  'operator' => 'IN' // Possible values are 'IN', 'NOT IN', 'AND'.
)
`

= Q.3 Can I place content before and after the product loop? =

A.3 Yes, there are two action hooks you can use.

`add_action( 'ss_wc_shortcode_before_product_tag_loop', 'your_function_name' );`

`add_action( 'ss_wc_shortcode_after_product_tag_loop', 'your_function_name' );`

== Changelog ==

= 1.0.0 : 15th June 2015 =
* Initial version
