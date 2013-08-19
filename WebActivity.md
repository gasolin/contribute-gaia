# Homescreen

    "activities": {
      "save-bookmark": {
        "filters": {
          "type": "url",
          "url": { "required":true, "pattern":"https?:.{1,16384}" }
        },
        "disposition": "inline",
        "href": "/save-bookmark.html",
        "returnValue": true
      }
    }

# Bluetooth

    "activities": {
      "share": {
        "disposition": "inline",
        "returnValue": true,
        "href": "/transfer.html"
      }
    },

# Browser

    "activities": {
      "view": {
        "filters": {
          "type": "url",
          "url": {
            "required":true, "pattern":"https?:.{1,16384}", "patternFlags":"i"
          }
        }
      }
    }

# Camera

    "activities": {
      "record": {
        "filters": {
          "type": ["photos", "videos"]
         },
        "disposition": "window"
      },
      "pick": {
        "filters": {
          "type": ["image/*", "image/jpeg", "video/*", "video/3gpp"]
         },
        "returnValue": true,
        "disposition": "inline",
        "href": "/index.html#pick"
      }
    },
  
# Communication

    "activities": {
      "pick": {
        "filters": {
          "type": {
            "required": true,
            "value": ["webcontacts/contact","webcontacts/email","webcontacts/tel"]
          }
         },
        "disposition": "inline",
        "href": "/contacts/index.html?pick",
        "returnValue": true
      },
      "open": {
      "filters": {
        "type": "webcontacts/contact"
      },
      "disposition": "inline",
      "href": "/contacts/index.html?open",
      "returnValue": true
    },
    "new": {
      "filters": {
        "type": "webcontacts/contact"
      },
      "disposition": "inline",
      "href": "/contacts/index.html?new",
      "returnValue": true
    },
    "update": {
      "filters": {
        "type": "webcontacts/contact"
      },
      "disposition": "inline",
      "href": "/contacts/index.html?update",
      "returnValue": true
    },
    "dial": {
      "filters": {
        "type": "webtelephony/number",
        "number": { "pattern":"[\\d\\s+#*().-]{0,50}" }
      },
      "href": "/dialer/index.html#keyboard-view",
      "disposition": "window"
    }
    },
  
# CostControl

    "activities": {
    "costcontrol/balance": {
      "filters": {
       },
      "disposition": "window"
    },
    "costcontrol/telephony": {
      "filters": {
       },
      "disposition": "window"
    },
    "costcontrol/data_usage": {
      "filters": {
       },
      "disposition": "window"
    }
    }
  
# Email

    "activities": {
    "new": {
      "filters": {
        "type": "mail"
      },
      "disposition": "window"
    },
    "share": {
      "filters": {
        "type": "image/*"
       },
      "disposition": "window",
      "returnValue": true
    },
    "view": {
      "filters": {
        "type": "url",
        "url": { "required":true, "pattern":"mailto:.{1,16384}" }
      }
    }
    },
  
# Gallery

    "activities": {
    "browse": {
      "filters": {
        "type": "photos"
       },
      "disposition": "window"
    },
    "pick": {
      "filters": {
        "type": ["image/*", "image/jpeg", "image/png"]
       },
      "disposition": "inline",
      "returnValue": true,
      "href": "/index.html#pick"
    },
    "open": {
      "filters": {
        "type": ["image/jpeg", "image/png", "image/gif", "image/bmp"]
       },
      "disposition": "inline",
      "returnValue": true,
      "href": "/open.html"
    }
    },
  
# Music 

    "activities": {
    "pick": {
      "filters": {
        "type": ["audio/*", "audio/mpeg", "audio/ogg", "audio/mp4"]
       },
      "disposition": "inline",
      "returnValue": true,
      "href": "/index.html#pick"
    },
    "open": {
      "filters": {
        "type": ["audio/mpeg", "audio/ogg", "audio/mp4", "audio/amr"]
       },
      "disposition": "inline",
      "returnValue": true,
      "href": "/open.html"
    }
    }
  

# PDF.js

    "activities": {
    "view" : {
      "filters": {
        "type": "application/pdf"
      },
      "disposition": "inline",
      "href": "/content/web/viewer.html",
      "returnValue": true
    }
    },

# Settings

    "activities": {
    "configure": {
      "filters": {
        "target": "device"
       },
      "disposition": "window"
    }
    },
  

# SMS

    "activities": {
    "new": {
      "filters": {
        "type": "websms/sms",
        "number": {
          "pattern":"[\\w\\s+#*().-]{0,50}"
        }
       },
      "disposition": "window"
    },
    "share": {
      "filters": {
        "type": ["image/*", "audio/*", "video/*"],
        "number": 1
       },
      "disposition": "window",
      "returnValue": true
    }
    },
  
# Video

    "activities": {
    "pick": {
      "filters": {
        "type": ["video/*", "video/webm", "video/mp4", "video/3gpp", "video/ogg"]
       },
      "disposition": "inline",
      "returnValue": true,
      "href": "/index.html#pick"
    },
    "view" : {
      "filters": {
        "type": ["video/webm", "video/mp4", "video/3gpp", "video/ogg"]
      },
      "href": "view.html",
      "disposition": "inline",
      "returnValue": true
    },
    "open" : {
      "filters": {
        "type": ["video/webm", "video/mp4", "video/3gpp", "video/ogg"]
      },
      "href": "view.html",
      "disposition": "inline",
      "returnValue": true
    }
    }
  
# Wallpaper

    "activities": {
    "pick": {
      "filters": {
        "type": ["image/*", "image/jpeg"],
        "width": 320,
        "height": 480
       },
      "disposition": "inline",
      "returnValue": true,
      "href": "/pick.html"
    },
    "share": {
      "filters": {
        "type": "image/*",
        "number": 1
       },
      "disposition": "inline",
      "returnValue": true,
      "href": "/share.html"
    }
    },
  
  
