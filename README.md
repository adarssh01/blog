# Modern blog theme 

Modern blog theme is designed for use with Jekyll. Jekyll is a powerful static site generator that makes it easy to create and maintain a blog or personal website. With this theme, you'll be able to quickly set up a sleek and professional-looking blog that is fully customizable to suit your needs.



## Preview



**[View Live Preview](https://adarssh01.github.io/adarsh.github.io/)**

## Installation & Setup

### Using RubyGems

Jekyll is built with Ruby, so you will need to have Ruby installed on your computer. You can download the latest version of Ruby from the official website. Follow the instructions below for complete setup.

1. (Optional) Create a new Jekyll site: `jekyll new my-site`
2. Replace the current theme in your `Gemfile` with `gem "jekyll-theme-clean-blog"`.
3. Install the theme (run the command inside your site directory): `bundle install`
4. Replace the current theme in your `_config.yml` file with `theme: jekyll-theme-clean-blog`.
5. Build your site: `bundle exec jekyll serve`

Assuming there are no errors and the site is building properly, follow these steps next:

1. Create the following pages if they do not exist already (or change the extension of existing markdown files from `.md` to `.html`):

   * `index.html` - set to `layout: home`
   * `about.html` - set to `layout: page`
   * `contact.html` - set to `layout: page`
   * `posts/index.html` - set to `layout: page` (you will also need to create a `posts` directory)

2. Configure the `index.html` front matter. Example:

    ```markdown
    ---
    layout: home
    background: '/PATH_TO_IMAGE'
    ---
    ```

3. Configure the `about.html`, `contact.html`, and `posts/index.html` front matter. Example:

    ```markdown
    ---
    layout: page
    title: Page Title
    description: This is the page description.
    background: '/PATH_TO_IMAGE'
    ---
    ```
4. # Creating a new post
* Create a new markdown file in the _posts directory with the naming convention YYYY-MM-DD-title.md.
* At the top of the file, add the following front matter:

  For each post in the `_posts` directory, update the front matter. Example:

    ```markdown
    ---
    layout: post
    title: "Post Title"
    subtitle: "This is the post subtitle." (optional)
    date: YYYY-MM-DD HH:MM:SS
    background: '/PATH_TO_IMAGE'
    ---
    ```
    
* Write your post in markdown

    For reference, look at the [repository](https://github.com/adarssh01/adarsh.github.io) to see how the files are set up.



5. Build your site: `bundle exec jekyll serve`

### Using Core Files

When using the core files, the demo images, posts, and pages are all included with the download. After following the instructions below, you can then go and change the content of the pages and posts.

1. [Download](https://github.com/adarssh01/adarsh.github.io/archive/refs/heads/main.zip) or Clone the repository.
2. Update the following configuration settings in your `_config.yml` file:

    * `baseurl`
    * `url`
    * `title`
    * `email`
    * `description`
    * `author`
    * `twitter_username` (Optional)
    * `facebook_username` (Optional)
    * `github_username` (Optional)
    * `linkedin_username` (Optional)
    * `instagram_username` (Optional)

3. Build your site: `bundle exec jekyll serve`

## Bugs and Issues

Have a bug or an issue with this template? [Open a new issue](https://github.com/adarssh01/adarsh.github.io/issues) here on GitHub!

## About
The modern blog theme is designed for use with Jekyll, a powerful static site generator that makes it easy to create and maintain a blog or personal website. With this theme, you'll be able to quickly set up a sleek and professional-looking blog that is fully customizable to suit your needs.
The theme is built with the latest web technologies, including HTML, CSS, and JavaScript, and is fully responsive, ensuring that your site looks great on any device. 
 Additionally, it's made with Bootstrap, a widely used open-source front-end framework, which makes it easy to customize the look and feel of your site.

## Copyright and License

Copyright 2013-2021 Start Bootstrap LLC. Code released under the [MIT](https://github.com/StartBootstrap/startbootstrap-clean-blog-jekyll/blob/master/LICENSE) license.
