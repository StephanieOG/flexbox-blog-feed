![Stephanie O'Gay Garcia](https://www.stephanieogaygarcia.com/hubfs/Logos/StephanieOGayGarcia-PoppinsLogo-1.png "Stephanie O'Gay Garcia")


# Flexbox Blog Feed

This is a simple flexbox card layout that displays the most recent posts from a blog or blog tag/topic. It is intended to be use on pages that are not the blog to showcase blog content, typically a homepage or a company page. 

Preview a live demo of the module here: https://www.stephanieogaygarcia.com/hubspot-custom-module-demo-flexbox-blog-feed

![Demo Preview](https://github.com/StephanieOG/flexbox-blog-feed/blob/master/screenshots/flexbox-blog-feed-demo.png?raw=true "Demo Preview")

## Fields
In the module basic module, there are only three fields: 

- Choose Blog (Blog field)
- Use posts from a specific tag/topic? (Boolean field)
- Tag (tag field)

![Module Preview](https://github.com/StephanieOG/flexbox-blog-feed/blob/master/screenshots/flexbox-blog-feed-module-preview.png?raw=true "Module Preview")

## Customisations

### Number of posts
You can decrease or increase the number of posts to be displayed by updating the number_of_posts value. If you do so, you may want to also update the flex-basis width in the CSS (note that this changes in the media queries below).

### Content displayed
When using this module with clients, I've often added in additional boolean fields that lets them choose what they want to display (e.g. so they can hide the author, date or summary). For example, if you create the boolean field "Display Summary", you could copy the snippet for that field and wrap it around the summary: 

         {% if module.content.display_summary %}
          <div class="blog-post-summary">{{ post.post_summary }}</div>
         {% endif %}  

### Styling
The module currently has minimal styling but can be customised using the CSS classes for each element.  
