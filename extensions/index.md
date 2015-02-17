---
title: Open Badges Extensions
subtitle: Community-developed additions to the Open Badges Standard
show_sidebar: true
layout: page
---

## {{ page.title }}
Extensions are community developed contributions to the Open Badges Standard. Any issuer may define and publish them to include new types of metadata in badges. Any other issuer may use the same extensions to publish similar information in a mutually recognizable way.

### [Open Badges Community Extensions](#CommunityExtensions)
Submit your published extensions to this page with a pull request on [GitHub](https://github.com/openbadges/openbadges/specification/extensions/index.md), following the existing format of the page.


# Extension Example:

### <a name="ExampleExtension"></a> Example Extension Name
This is a definition of an example extension. If it were a real extension, it would describe the purpose of adding it to a badge object. If you follow the link [#ExampleExtension](#ExampleExtension), you'll get to this paragraph. This is the IRI (Internationalized Resource Identifier) to use for implementations of this exension, included below as the compact IRI `extension:ExampleExtension`. See the [context](./exampleExtension/context.json) and [schema](./exampleExtension/schema.json) files that form the machine-readable core of this extension.

Property     | Type        | Value Description
-------------|-------------|---------
**@context** | context IRI | [http://standard.openbadges.org/extensions/exampleExtension/context.json](./exampleExtension/context.json)
**@type**    | type IRI array |`['extension', 'extension:exampleExtension']`
**exampleProperty** | string | Any text the implementer likes.

**Extendable Badge Objects:**
Assertion, BadgeClass, Issuer

**Example implementation:**
{% highlight json %}
{ 
  "extension:ExampleExtension": {
    "@context":"http://standard.openbadges.org/extensions/exampleExtension/context.json",
    "@type": ["extension", "extension:ExampleExtension"],
    "exampleProperty": "I'm a property, short and sweet."
  }
}
{% endhighlight %}


# Community Extensions: