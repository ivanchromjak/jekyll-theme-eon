---
title:                  Theme Docs
width:                  small
navbar:
  sticky:               false
  scroll_up:            true
  animation:            true
  transparent:          true
  transparent_color:    light
header:
  layout:               center # Options: left, center, 1-1, 1-2, 1-3 or 2-3
  background_image:     header-8.jpg
  background_overlay:   "rgba(0, 0, 0, 0.5)"
  color:                light
  header_size:         large
  heading_size:         medium
  parallax:             true
---

{% include toc.html %}

## Theme installation
{: .uk-heading-divider}

Install the dependencies with [Bundler](http://bundler.io/):

```bash
bundle install
```

Run the following to generate your site:
```bash
bundle exec jekyll serve
```

You can find more on [Deployment Methods](https://jekyllrb.com/docs/deployment-methods/) page on Jekyll website.

## Basic theme setup
{: .uk-heading-divider}

### Site URL
The base hostname and protocol for your site. If you’re hosting with GitHub Pages this will be something like `url: "https://username.github.io"` or `url: "https://mydomain.com"` if you have a custom domain name.

```yaml
url:                    "https://eon.jekyll.plus"
```

### Site base URL
If you want to host your site in a subfolder (eg: /blog) set it as `baseurl: "/blog"`.


### Site and author details
Add your site and author details in `_config.yml`:

```yaml
title:                  Eon
description:            Multipurpose Jekyll theme.

# Default author settings
author:
  name:                 Pete Seth
  avatar:               avatar-tom.png
  title:                Support     
```

### Update favicon
You can find the current favicon (favicon.png) inside the theme `/uploads/` directory, just replace it with your new favicon.

### Update logo
The theme uses two logo files one dark for display on light backgrounds and one light logo for display on dark backgrounds. If you don't intent to use dark navigation backgrounds you dont need to upload the light logo.
Add your logo image files to `/uploads/` directory, then specify the logo files in `_config.yml`:

```yaml
logo:                   logo-dark.svg
logo_light:             logo-light.svg
```
If logo image files are not set, the site title text is displayed instead.

## Navigation
{: .uk-heading-divider}

### Main navigation bar
There are two navigation bar layouts `default` or `center`, the default layout offers left, center or right aligned navigation with logo on the left, the center layout display logo in the center and navigation link on the left and right. 

Set navbar layout options in `_config.yml`, these setting can be overridden on per page basis in page front matter:

```yaml
navbar:
  layout:               default   # Options: default, center
  color:                dark      # Text color, Options: dark or light
  animation:            true
  sticky:               true
  search:               false
  scroll_up:            true
  transparent:          true
  transparent_color:    light  
```


Set in the main navigation links in `_data/base/navbar.yml`:

```yaml
left:
  - title: About
    url: /about/
center:
  - title: About
    url: /about/
right:
  - title: About
    url: /about/
```

To display a link as a button use:
```yaml
- title: Contact
  url: /contact/
  button: success
```

All available button styles:
```yaml
- title: Changelog
  url: /contact/
  button: default

- title: Contact
  url: /contact/
  button: primary

- title: Changelog
  url: /contact/
  button: secondary

- title: Contact
  url: /contact/
  button: danger

- title: Changelog
  url: /contact/
  button: success

- title: Contact
  url: /contact/
  button: warning

- title: Changelog
  url: /contact/
  button: primary-outline

- title: Contact
  url: /contact/
  button: danger-outline

- title: Changelog
  url: /contact/
  button: success-outline

- title: Contact
  url: /contact/
  button: warning-outline
```

### Mobile navigation
Set in the mobile navigation links in `_data/base/mobile.yml`:

```yaml
- title: About
  url: /about/
```

## Header
Page headers offer numerous content, layout and styling options.

#### Background options
Set header background color, image, video and overlar color:
```yaml
header:
  background_color:     "#1B33BF"
  background_image:     working-space.jpg
  background_align:     center-center # Image position, Options: center-center, top-center, bottom-center, center-right, center-left
  background_video:     working-space.mp4
  background_overlay:   "rgba(0, 0, 0, 0.5)"
```
Upload images and videos to `/uploads/` directory.

#### Content options
```yaml
header:
  layout:               1-1           # Options: left, center, 1-1, 1-2, 1-3 or 2-3. Left, right options display this pages title and subtitle. 1-1, 1-2, 1-3 or 2-3 options display content of block file/s.
  color:                light         # Content font color, Options: light, dark
  header_size:         large         # Content top and bottom padding, Options: small, medium, large
  heading_size:         medium        # Title size, Options: small, medium, large
  height:               full          # Enable viewport height, Options: full
  parallax:             true          # Enable content parallax, Options: true
  container:            small         # Content width, Options: expand, small, xsmall
  content:                            # Source block file for first column if layout set to 1-1, 1-2, 1-3 or 2-3
    block:              header-one    # Reference block file e.g. for _blocks/header-one.md enter header-one
  content-2:                          # Source block file for second column if layout is set to 1-1, 1-2, 1-3 or 2-3
    block:              header-two    # Reference block file e.g. for _blocks/header-two.md enter header-two 
    title:              false         # Do not display block title, Options: false
```

## Footer
{: .uk-heading-divider}

Edit footer layout, background color style and copyright notice in `_config.yml`:
```yaml
footer:           
  style:                secondary     # default, muted, primary, secondary
  layout:               columns       # center or columns
  copyright:            Made by a <a href="https://mysite.com/">human</a>.
```

Set in the footer navigation links in `_data/base/mobile.yml`. There are two footer layouts `center` or `columns`, the layout is set in `_config.yml`. Set the footer links under the chosen footer layout variable:

The center layout has one horizontal navigation:
```yaml
center:
  - title: Services
    url: /services/
```

The columns layout offers multiple (up to six) columns of navigation links:
```yaml
columns:
  - title: COLUMN ONE
    links:
      - title: Marketing Tools
        url: /#
      - title: Presentations
        url: /#
      - title: Professionals
  - title: COLUMN TWO
    links:
      - title: Small Businesses
        url: /#
      - title: Photographers
        url: /#
      - title: Restaurants
```

## Page layouts and sidebars

#### Page container width
Width of the page content, the following page widths are available:
- `full` suitable when adding full browser width sections to a page
- `expand` full browser width with horizontal padding
- `small` small container
- `xsmall` extra small container

Set page width by adding the following to page front matter block:
```yml
width:                full
```

#### Sidebars
Add sidebar to a page by adding the following to page front matter block:
Set page width by adding the following to page front matter block:
```yml
sidebar: 
  right:              sidebar-left
  left:               sidebar-right
```

Sidebar widgets are defied in `_data/base/sidebar.yml` data file, the following widget are available:
```yml
sidebar-left:

  - widget:           latest        # Display list of latest posts
    type:             posts         # Post type: posts
    count:            15            # Number of posts to display
    title:            Latest Posts

  - widget:           author        # Display user information
    author:           john          # User variable from _config.yml 'authors' setting

  - widget:           tagged        # Display list of posts by tag
    type:             posts         # Post type: posts
    primary:
      title:          Product news
      tag:            news          # Display post tagged with 'news' tag
    secondary:                      # Optional second tab
      title:          Editor picks
      tag:            pick          # Display post tagged with 'pick' tag

  - widget:           navigation    # Navigation links widget
    nav:
    - title:          Pages         
      links:
        - title:      Portfolio
          url:        /portfolio/
        - title:      Blog
          url:        /blog/

  - widget:           block         # Display contents of a block file
    block:            block-1       # Block _blocks/block-1.md file to display
    title:            Content of a block
```

## Sections
Section is a wrapper arround piece of included content that allows setting custom backgrounds and layout options. Section options are defined as attributed in include, for example:

Image include without a section wrapper:
{% raw %}
```yml
{% include image.html 
  src="portfolio-4-header.jpg"
  alt="Some alt title"
%}
```
{% endraw %}

Image include with a section wrapper, includes all options for demonstration:
{% raw %}
```yml
{% include image.html 
  src="portfolio-4-header.jpg"
  alt="Some alt title"
  section_size="medium"
  section_padding_remove="top"
  section_title="Section title" 
  section_subtitle="Section subtitle" 
  section_header_align="center"
  section_header_color="#fff"
  section_background="primary" 
  section_image="image-3.jpg"
  section_image_align="center-center"
  section_video="video-3.mp4"
  section_overlay="rgba(0, 0, 0, 0.5)"
  section_container="small"
  section_content_align="center"
  section_content_color="light"
%}
```
{% endraw %}

#### Attributes

| Attribute | Description | Choices |
| --- | --- | --- |
| section_size | Section size (top and bottom padding) required to enable section | xsmall, small, medium, large, xlarge |
| section_title | Optional section title | string |
| section_subtitle | Optional section subtitle | string |
| section_header_align | Aligns section title and subtitle | left, center, right |
| section_header_color | Section title and subtitle font color | light, hex or rgb color value |
| section_background | Section background color | muted, primary, secondary, hex or rgb color value |
| section_image | Background image | Image file name (upload image to `/uploads/` directory), external image URL |
| section_image_align | Background image position | center-center, top-center, bottom-center, center-right, center-left |
| section_video | Background video | MP4 file name, (upload video to `/uploads/` directory), external video URL|
| section_overlay | Background overlay color | rgba color value |
| section_container | Content container width | expand, small, xsmall |
| section_content_align | Content alignment | left, center, right |
| section_content_color | Content font color | light, hex or rgb color value |

## Introduction to blocks

Theme uses blocks as source of content for many includes. Blocks is a Jekyll collection with its posts in `_blocks` directory. Some includes such as call to action will pull content only from one block post e.g.:
{% raw %}
```yml
{% include cta.html 
  block="cta-2"
%}
```
{% endraw %}
The above include references `cta-2` as block source, this displays contents of `_blocks/cta-2.md` file.

Other includes such as gallery, cards or sliders display contents of multiple block posts ordered by file name e.g.:
{% raw %}
```yml
{% include cards.html 
  block="feature" 
%}
```
{% endraw %}
The above include references `feature` as block source, this displays contents of all files that have `feature` as a part of their filename:
```yml
_blocks/
    feature-1.md
    feature-2.md
    feature-3.md
    feature-4.md
    feature-5.md
    feature-6.md
```
All the above files would display as cards (one file per card) ordered from 1 to 6.

## Cards
Use the following include to add cards to a page:

{% raw %}
```yml
{% include cards.html 
  block="home-card" 
  media="top" 
  card_style="default"
  grid="1-2"
%}
```
{% endraw %}

#### Attributes

| Attribute | Description | Choices |
| --- | --- | --- |
| block | Block posts to display | block file name without extension e.g. to display `home-card-1.md` and `home-card-2.md` as cards, reference `block="home-card"` |
| media | Alignment of media (image or icon) | left, top, right |
| card_style | Card style | default, primary, secondary, leave blank for borderless style |
| grid | Display cards in columns | 1-2, 1-3, 1-4, 1-5, 1-6 |
| gutter | Spacing between columns | small, medium, large, collapse, leave blank for default |

Example of card block post with image media, upload the image to `/uploads/` directory:
```yml
---
title: Are of brief house annoyed
image: card-2.jpeg
---

Suspendisse quis turpis quis, semper consequat vehicula dolor consequat quam, ac consequat posuere leo dapibus.
```

Example of card block post with icon media, use one of the icons from `_includes/icons/` directory or add your own:
```yml
---
title: Navbar
icon: ios-navigation-toolbar-top.svg
---

Fixed or sticky navbar with left, center and right aligned navigation.
```

## Image
Use the following include to add an image to a page:
{% raw %}
```yml
{% include image.html 
	src="alexander-read.jpg"
  alt="Alt for image"
  align="right"
  caption="Caption example"
  lightbox="true"
%}
```
{% endraw %}

#### Attributes

| Attribute | Description | Choices |
| --- | --- | --- |
| src | Image file source | image file name, upload the image to `/uploads/` directory or external image URL |
| alt | Image alt text | string |
| align | Align within text | left, right |
| caption | Image caption | string |
| lightbox | Display image in popup lightbox on a click | true |

## Slider
Use the following include to add a slider to a page:
{% raw %}
```yml
{% include slider.html 
  block="slider-home" 
  color="light"
  display_title="false"
  autoplay="true"
  sets="true"
  grid="1-3"
  gutter="large"
  navigation="outside"
  dotnav="true"
  card_style="default"
%}
```
{% endraw %}

#### Attributes

| Attribute | Description | Choices |
| --- | --- | --- |
| block | Block posts to display | block file name without extension |
| color | Enable light font color for dark content | light |
| display_title | Disable slide title | false |
| autoplay | Auto slide slider | true |
| sets | Slide slides in sets | true |
| navigation | Display navigation outside of slides | outside |
| dotnav | Enable dot navigation | true |
| grid | Display slides in columns | 1-1, 1-2, 1-3, 1-4, 1-5, 1-6 |
| gutter | Spacing between columns | small, medium, large, collapse, leave blank for default |
| card_style | Display slides as card style | default, primary, secondary, leave blank for borderless style |
| media | Alignment of card media (image or icon) if card_style attribute used | left, top, right |

Example of slide block post, upload the image to `/uploads/` directory:
```yml
---
title: Are of brief house annoyed
image: card-2.jpeg
---
```






{% raw %}
```yml

```
{% endraw %}




## Creating your first post in Jekyll
{: .uk-heading-divider}

To create a new post, you can create a new markdown file inside the `_posts` directory by following the recommended file naming format:
```
YEAR-MONTH-DAY-title.MARKUP
```
Where `YEAR` is a four-digit number, `MONTH` and `DAY` are both two-digit numbers, and `MARKUP` is the file extension representing the format used in the file. For example, the following are examples of valid post filenames:

```
2011-12-31-new-years-eve-is-awesome.md
2012-09-12-how-to-write-a-blog.md
```

Post requires front matter, everything in between the first and second --- are part of the YAML Front Matter, and everything after the second --- will be rendered with Markdown and show up as “Content”.
The following is a post file with different configurations you can add as example:

```yaml
---
layout: post
title: How To Travel On Low Budget
---
```

You can rebuild the site in many different ways, but the most common way is to run `bundle exec jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To keep things more organized, add post images to `/uploads/` directory.

## Creating FAQ posts
{: .uk-heading-divider}

Create new FAQ post entries in `_faqs` folder, similar to creating posts, but with following front matter settings:

```yml
---
title: Do you provide customer support?
categories: [presale]
---
```

## Enabling comments (via Disqus)
{: .uk-heading-divider}

Optionally, if you have a Disqus account, you can tell Jekyll to use it to show a comments section below each post. To enable it, add the following lines to your Jekyll site:

```yaml
disqus:
    shortname: my_disqus_shortname
```

You can find out more about Disqus' shortnames [here](https://help.disqus.com/customer/portal/articles/466208).

Comments are enabled by default and will only appear in production, i.e., `JEKYLL_ENV=production`. If you don't want to display comments for a particular post you can disable them by adding `comments: false` to that post's YAML Front Matter.

## Adding media to post content
{: .uk-heading-divider}

### Adding images
To add an image to a post or page use the following codes:
Local image from `/uploads/` directory:
{% raw %}
```yaml
{% include image.html src="girl.jpg" alt="Alt for image" caption="Girl on a rock" %}
```
{% endraw %}

External wide image with lightbox:
{% raw %}
```yaml
{% include image.html src="https://source.unsplash.com/TT-ROxWj9nA.jpg" lightbox="true" alt="Alt for image" caption="Image in lightbox" %}
```
{% endraw %}

Uploads folder location can be changed in `_config.yml`.

### Slideshow

{% raw %}
```yaml
{% include slideshow.html gallery="slideshow-1" %}
```
{% endraw %}

The `gallery` attribute refers to a folder inside your `uploads` folder, all images in `slideshow-1` folder will be displyed in slideshow. Uploads folder location can be changed in `_config.yml`.

### Responsive Videos
Embed local videos:
```html
<video controls playsinline uk-video="automute: true">
    <source src="http://www.quirksmode.org/html5/videos/big_buck_bunny.mp4" type="video/mp4">
    <source src="http://www.quirksmode.org/html5/videos/big_buck_bunny.ogv" type="video/ogg">
</video>
```
Embed YouTube videos:
```html
<iframe src="http://www.youtube.com/embed/YE7VzlLtp-4?autoplay=0&amp;showinfo=0&amp;rel=0&amp;modestbranding=1&amp;playsinline=1" width="600" height="340" frameborder="0" allowfullscreen uk-responsive uk-video="automute: true"></iframe>
```

## Adding alerts to content
{: .uk-heading-divider}

There are four alert styles:

{% include alert.html style="primary" text="Cras at dolor eget urna varius faucibus tempus in elit." %}

{% include alert.html style="success" text="Cras at dolor eget urna varius faucibus tempus in elit." %}

{% include alert.html style="warning" text="Cras at dolor eget urna varius faucibus tempus in elit." %}

{% include alert.html style="danger" text="Cras at dolor eget urna varius faucibus tempus in elit." %}

Add alerts to a post using the following includes:

{% raw %}
```yaml
{% include alert.html style="primary" text="Cras at dolor eget urna varius faucibus tempus in elit." %}

{% include alert.html style="success" text="Cras at dolor eget urna varius faucibus tempus in elit." %}

{% include alert.html style="warning" text="Cras at dolor eget urna varius faucibus tempus in elit." %}

{% include alert.html style="danger" text="Cras at dolor eget urna varius faucibus tempus in elit." %}
```
{% endraw %}

## Page header
{: .uk-heading-divider}

To add a hero header to a page add the following to a YAML Front Matter:

{% raw %}
```yaml
---
title: Page title
subtitle: Page subtitle optional
width: full
navbar:
  sticky: true
  scroll_up: true
  animation: true
  transparent: true
  transparent_color: light
header:
  layout: 1-1 # Options: left, center, 1-1, 1-2, 1-3 or 2-3
  background_color: "#1B33BF"
  background_image: Working-Space.jpg
  background_video: Working-Space.mp4
  background_align: center-center
  background_overlay: "rgba(0, 0, 0, 0.5)"
  color: light
  header_size: large
  heading_size: medium
  height: full
  parallax: true
  container:
    block: header-home
    # title: false
---
```
{% endraw %}

## Frequently asked questions section
{: .uk-heading-divider}

Create FAQ post in `_faqs` folder (categories are optional):
```yml
---
title: Do you provide customer support?
categories: [presale]
---
```

To add the following to a page:
{% raw %}
```yaml
{% include faqs.html 
  multiple="true" 
  title="Frequently asked questions" 
  category="presale"
%}
```
{% endraw %}

Specifying category is optional, if not defined all FAQ posts will be displayed. To display multiple FAQs at the same time without one collapsing when the other one is opened, add the `multiple="true"` attribute.

## Call to action
{: .uk-heading-divider}

To add the following to a page:
{% raw %}
```yaml
{% include cta.html 
  section_size="large"
  section_image="header-9.jpeg"
  section_overlay="rgba(0, 0, 0, 0.5)"
  section_container="small"
  section_content_align="center"
  section_content_color="light"
  layout="1"
  block="cta-4"
%}
```
{% endraw %}

## Contact form (via FormSpree)
{: .uk-heading-divider}

Submit the form and confirm your email address at [FormSpree](https://formspree.io/). Then add the following include to a page, replacing the email address:

{% raw %}
```yaml
{% include 
  formspree.html 
  email="my_name@gmail.com" 
  redirect="/thanks/" 
  name="true" 
  subject="true" 
%}
```
{% endraw %}


## Google Analytics
{: .uk-heading-divider}

To enable Google Anaytics, add the following lines to your Jekyll site:

```yaml
  google_analytics: UA-NNNNNNNN-N
```

Google Analytics will only appear in production, i.e., `JEKYLL_ENV=production`

## Displaying mailchimp newsletter sign up form on a blog post
{: .uk-heading-divider}

Add the following code in `_congig.yml`:
```yaml
mailchimp:
  form_action:    "https://mycompany.us8.list-manage.com/subscribe/post?u=2e56c13452bd&amp;id=e682645464"
  hidden_name:    "b_2e56c1231057fjsd4fd_e685657"

# Defaults
defaults:
  # _posts
  - scope:
      path: ""
      type: posts
    values:
      mailchimp: true
```

Get the values for `form_action` and `hidden_name` from your mailchimp embed form:

Get `form_action` value from:

```
<form action="https://mycompany.us8.list-manage.com/subscribe/post?u=2e56c12fcd37e5dab02bd&amp;id=e6e94847464" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
```

Get `hidden_name` value from:
```
<input type="text" name="b_2e56c123105fcd37e5dab02bd_e68475657" tabindex="-1" value="">
```

## Translation
{: .uk-heading-divider}

Set your language code in `_config.yml`:
```yml
lang: en
```
Theme strings can be translated in `_data/base/translation.yml`, copy the current English translation and paste it bellow the Eglish translation, then replace `en` with you language code that you set in `_config.yml` and translate the strings.

```yml
en:
  previous:                   "Previous"
  next:                       "Next"
  related_articles:           "Related Articles"
  related_posts:              "Related Posts"
  read_more:                  "Read more"
  by:                         "By"
  share_twitter:              "Share on Twitter"
  share_facebook:             "Share on Facebook"
  search_placeholder:         "Search for answers"
  search_no_results:          "No results found"
  mobile_nav_site:            "Menu"
  contact_name:               "Name"
  contact_email:              "Email"
  contact_subject:            "Subject"
  contact_message:            "Message"
  contact_send:               "Send"
```

## Customization
{: .uk-heading-divider}

To modify the primary color, open `/_sass/theme/variables.scss` and replace the color values e.g.:

```scss
$global-primary-background:                   #05c896;
```

Further style customisation can be done in the following files:
```
/_sass/theme/mixins.scss
/_sass/theme/variables.scss
/assets/css/main.scss
```

## Development
{: .uk-heading-divider}

### Build process
Install [UIkit](https://getuikit.com/) font end framework dependency via Npm:
```bash
npm install
```
Enable live browser reload with the following:
```bash
bundle exec jekyll s --livereload
```

Use the following commands to compile js scripts:
```bash
npm run dev
```
Compile and minify:
```bash
npm run build
```

### Hooks
There are two hook inlude files that simplify adding content or scripts in the theme locations:
- `_includes/hook-head.html`
- `_includes/hook-pre-closing-body.html`

## Contacting support
{: .uk-heading-divider}

Customer support is provided through our Envato item page [contact form](https://themeforest.net/user/pressapps) for up to six months from the purchase date and is provided Monday to Friday during the business week. We aim to answer all support requests daily, most are handled within 24h.

## Sources and credits
{: .uk-heading-divider}

- Google analytics [https://www.google.com/analytics/](https://www.google.com/analytics/)
- Google maps [https://www.google.com/maps](https://www.google.com/maps)
- UIkit front end framework [https://getuikit.com/](https://getuikit.com/)
- Jekyll CML [https://jekyllrb.com/](https://jekyllrb.com/)