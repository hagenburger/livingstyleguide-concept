# LivingStyleGuide 2.0 Concepts

This is a **work-in-progress** repository to test upcoming features and syntax
enhancements of the [LivingStyleGuide Gem](http://livingstyleguide.org). The
code listed in here does not work. It exists to check consistency within all
planned features and get feedback by users before implementing the code.

I also wrote a blog post about the [plans for the LivingStyleGuide v2.0.0](http://www.hagenburger.net/BLOG/livingstyleguide-2.html). Those
influenced this repository. But while working on this, I made some small
improvements that differ from the blog post.


## Future Development

If you’re interested on updates and the progress of this, follow [@hagenburger](https://twitter.com/hagenburger)/[@LSGorg](https://twitter.com/LSGorg)
on Twitter or star the
[LivingStyleGuide repository](https://github.com/hagenburger/livingstyleguide).
I’m happy to get your feedback!


## Structure of this Repository

1. __[a_current-v1.0.x](tree/master/a_current-v1.0.x):__ The structure how
  it would look like with v1.0.x (current production ready code).
  * Uses YAML syntax for configuration (maybe hard to write if you’re not used
    to it by several Ruby projects)
  * Different syntax in config file and documentation files
  * Only one HTML file possible as output
  * Additional CSS for examples hard to integrate (in this example there is a
    popup (`position: absolute`) where the example lacks the height by default
2. __[b_new-v2.0.x](tree/master/b_new-v2.0.x):__ The same project,
  transferred to the new structure
  * LSG syntax is used for both—cofig file and documentation files
  * LSG syntax looks closer to CSS/SCSS/JavaScript/JSON and does not care about
    whitespace
  * Addition CSS for examples can be written in-line inside of the example
3. __[c_new-multiple-pages-v2.0.x](tree/master/c_new-multiple-pages-v2.0.x):__
  same example as above but additionally:
  * Style guide split up into several pages
  * One central config file
  * Possibility to include own filters
  * Possibility to use Ruby Gems (which may also define filters)
  * Use templates (eg Mustache) in examples and fill them with JSON data
  * Manually import documentation (don’t rely on Sass’ imports): This does not
    require including and parsing your whole Sass project anymore. You still may
    want to include colors and other partials to style the styleguide itself.
