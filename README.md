## Requirements

The truncator requires [Nokogiri][4] to parse out the HTML string.

## Usage

If you're using Jekyll, add the only_first_p.rb file to your _plugins directory - this will give you the helper `only_first_p` as a [Liquid][3] filter. In your views, you can use this function in order to *show only first paragraph of page/post*

    page | only_first_p

## Default output

<p>
{first paragraph content}
</p><a class="readmore" href="{post-url}">Read more</a>

## Configuration

You can choose whether to output a 'Read more' link and the link text to use.

Update your _config.yml as required.

    # Only First P Plugin
    only_first_p:
        show_read_more_link: true
        read_more_link_text: 'Read more'

The above is the default configuration and will be used if nothing is specified. Modify as needed.

[3]:http://liquidmarkup.org
[4]:http://nokogiri.org/