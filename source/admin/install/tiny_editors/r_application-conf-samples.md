# Sample application.conf {#application-conf-samples .reference}

A sample configuration for the Tiny Editor Services.

The following shows the configuration for the server connections.example.com. The configuration assumes the default ports are used and that WebSphere is configured with a trust store that will allow communication with external sites. This configuration will enable the spelling, link-checking, and media embedding services. The media embedding service has been configured with the details of many common OEmbed services to enable embedded content.

```
ephox {
  allowed-origins {
    origins = [
      "http://connections.example.com",
      "https://connections.example.com",

      "http://connections.example.com:9081",
      "https://connections.example.com:9444"
    ]
  }
  embed {
    custom = [
      # flickr
      {
        endpoint = "https://www.flickr.com/services/oembed.json/"
        schemes = [
          "http://www.flickr.com/photos/*",
          "https://www.flickr.com/photos/*",
          "http://www.flickr.com/photos/*/foo/",
          "https://www.flickr.com/photos/*/foo/",
          "http://*.flickr.com/photos/*",
          "https://*.flickr.com/photos/*"
        ]
      },
      # youtube
      {
        endpoint = "https://www.youtube.com/oembed"
        schemes = [
          "http://youtu.be/*",
          "https://youtu.be/*",
          "http://www.youtu.be/*",
          "https://www.youtu.be/*",
          "http://youtube.com/*",
          "https://youtube.com/*",
          "http://www.youtube.com/*",
          "https://www.youtube.com/*",
          "http://m.youtube.com/*",
          "https://m.youtube.com/*"
        ]
      },
      # NY Times
      {
        endpoint = "https://www.nytimes.com/svc/oembed/json/"
        schemes = [
          "http://www.nytimes.com/*",
          "https://www.nytimes.com/*"
        ]
      },
      # Daily Motion
      {
        endpoint = "http://www.dailymotion.com/services/oembed"
        schemes = [
          "http://www.dailymotion.com/video/*"
          "https://www.dailymotion.com/video/*"
          "http://www.dailymotion.com/embed/video/*"
          "https://www.dailymotion.com/embed/video/*"
        ]
      },
      # Soundcloud
      {
        endpoint = "http://soundcloud.com/oembed"
        schemes = [
          "http://soundcloud.com/*",
          "https://soundcloud.com/*",
          "http://api.soundcloud.com/tracks/*",
          "https://api.soundcloud.com/tracks/*"
        ]
      },
      # Facebook post
      {
        endpoint = "https://www.facebook.com/plugins/post/oembed.json/"
        schemes = [
          "http://*.facebook.com/permalink.php*",
          "https://*.facebook.com/permalink.php*",
          "http://*.facebook.com/photo.php*",
          "https://*.facebook.com/photo.php*",
          "http://*.facebook.com/*/photos/*",
          "https://*.facebook.com/*/photos/*",
          "http://*.facebook.com/*/posts/*",
          "https://*.facebook.com/*/posts/*",
          "http://*.facebook.com/*/activity/*",
          "https://*.facebook.com/*/activity/*",
          "http://*.facebook.com/notes/*",
          "https://*.facebook.com/media/set/*"
        ]
      },
      # Facebook Video
      {
        endpoint = "https://www.facebook.com/plugins/video/oembed.json/"
        schemes = [
          "http://www.facebook.com/video*",
          "https://www.facebook.com/video*",
          "http://www.facebook.com/*/videos/*",
          "https://www.facebook.com/*/videos/*",
          "http://business.facebook.com/video*",
          "https://business.facebook.com/video*",
          "http://business.facebook.com/*/videos/*",
          "https://business.facebook.com/*/videos/*"
        ]
      },
      # Facebook Page
      {
        endpoint = "https://www.facebook.com/plugins/page/oembed.json/"
        schemes = [
          "http://www.facebook.com/*",
          "https://www.facebook.com/*",
          "http://m.facebook.com/*",
          "https://m.facebook.com/*"
        ]
      },
      # Spotify
      {
        endpoint = "https://embed.spotify.com/oembed/"
        schemes = [
          "http://spotify.com/*",
          "https://spotify.com/*",
          "http://open.spotify.com/*",
          "https://open.spotify.com/*",
          "http://embed.spotify.com/*",
          "https://embed.spotify.com/*",
          "http://play.spotify.com/*",
          "https://play.spotify.com/*"
        ]
      },
      # Vine
      {
        endpoint = "https://vine.co/oembed.json"
        schemes = [
          "http://vine.co/v/*",
          "https://vine.co/v/*"
        ]
      },
      # Hulu
      {
        endpoint = "http://www.hulu.com/api/oembed.json",
        schemes = [
          "http://www.hulu.com/watch/*",
          "https://www.hulu.com/watch/*"
        ]
      },
      # Vimeo
      {
        endpoint = "http://vimeo.com/api/oembed.json",
        schemes = [
          "http://vimeo.com/*",
          "https://vimeo.com/*",
          "http://www.vimeo.com/*",
          "https://www.vimeo.com/*"
        ]
      },
      # CollegeHumor
      {
        endpoint = "http://www.collegehumor.com/oembed.json"
        schemes = [
          "http://www.collegehumor.com/video/*",
          "https://www.collegehumor.com/video/*"
        ]
      },
      # SmugMug
      {
        endpoint = "http://api.smugmug.com/services/oembed/"
        schemes = [
          "http://*.smugmug.com/*",
          "https://*.smugmug.com/*"
        ]
      },
      # Slideshare
      {
        endpoint = "http://www.slideshare.net/api/oembed/2"
        schemes = [
          "http://*.slideshare.net/*"
        ]
      },
      # Twitter timelines
      {
        endpoint = "https://publish.twitter.com/oembed?i=timeline"
        schemes = [
          "http://twitter.com/*/timelines/*",
          "https://twitter.com/*/timelines/*",
          "http://twitter.com/*/lists/*",
          "https://twitter.com/*/lists/*",
          "http://twitter.com/*/likes",
          "https://twitter.com/*/likes"
        ]
      },
      # Twitter Users
      {
        endpoint = "https://publish.twitter.com/oembed?i=user"
        schemes = [
          "http://twitter.com/*",
          "https://twitter.com/*"
        ]
      },
      # Getty Images
      {
        endpoint = "http://embed.gettyimages.com/oembed"
        schemes = [
          "http://gty.im/*",
          "https://gty.im/*"
        ]
      },
      # Wordpress
      {
        endpoint = "https://public-api.wordpress.com/oembed/1.0/?for=ephox"
        schemes = [
          "http://*.wordpress.com/*",
          "https://*.wordpress.com/*"
        ]
      },
      # Twitch
      {
        endpoint = "https://api.twitch.tv/v4/oembed"
        schemes = [
          "http://www.twitch.tv/*",
          "https://www.twitch.tv/*"
        ]
      },
      # Meetup
      {
        endpoint = "https://api.meetup.com/oembed"
        schemes = [
          "http://www.meetup.com/*",
          "https://www.meetup.com/*",
          "http://meetup.com/*",
          "https://meetup.com/*",
          "http://meetu.ps/*",
          "https://meetu.ps/*"
        ]
      },
      # Spotify
      {
        endpoint = "https://embed.spotify.com/oembed/"
        schemes = [
          "http://open.spotify.com/*",
          "https://open.spotify.com/*",
          "http://play.spotify.com/*",
          "https://play.spotify.com/*"
        ]
      },
      # Tech crunch
      {
        endpoint = "http://public-api.wordpress.com/oembed/1.0/?for=ephox"
        schemes = [
          "http://techcrunch.com/*",
          "https://techcrunch.com/*"
        ]
      },
      # Dotsub
      {
        endpoint = "https://dotsub.com/services/oembed"
        schemes = [
          "http://dotsub.com/view/*",
          "https://dotsub.com/view/*"
        ]
      },
      # Speaker deck
      {
        endpoint = "https://speakerdeck.com/oembed.json"
        schemes = [
          "http://speakerdeck.com/*/*",
          "https://speakerdeck.com/*/*"
        ]
      },
      # Tumblr
      {
        endpoint = "https://www.tumblr.com/oembed/1.0"
        schemes = [
          "http://*.tumblr.com/post/*",
          "https://*.tumblr.com/post/*"
        ]
      },
      # Adobe Stock
      {
        endpoint = "https://stock.adobe.com/oembed"
        schemes = [
          "http://stock.adobe.com/*",
          "https://stock.adobe.com/*"
        ]
      },
      # Code pen
      {
        endpoint = "https://codepen.io/api/oembed"
        schemes = [
          "http://codepen.io/*/pen/*",
          "https://codepen.io/*/pen/*"
        ]
      },
      # 500px
      {
        endpoint = "https://500px.com/oembed"
        schemes = [
          "http://500px.com/photo/*",
          "https://500px.com/photo/*"
        ]
      }
    ]
  }
}
```

**Parent topic:**[Common tasks, concepts and reference information](../../install/tiny_editors/r_appendix.md)

**Related information**  


[Tiny Editor Services configuration](../../install/tiny_editors/c_application-conf.md)

[Configuring the application.conf for the Tiny Editors Services](../../install/tiny_editors/t_01-setup_02-services_01-appconf_00-summary.md)

[../../admin/install/tiny\_editors/t\_01-setup\_02-services\_01-appconf\_01-create-an-application-conf-1.md](../../admin/install/tiny_editors/t_01-setup_02-services_01-appconf_01-create-an-application-conf-1.md)

[Disable SSL certificate validation for testing](../../install/tiny_editors/t_disable-certificate-validation-for-testing.md)

