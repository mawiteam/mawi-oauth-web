# Mawi OAuth client

The project created to allow third-party applications access Mawi users data(Integrate Mawi Solutions API in your system)

## Getting Started

To start working with Mawi OAuth client you need to contact Mawi Solutions CTO via email to request integration. CTO's email - artem@mawi.band

### 1. Prerequisites

To start working you need to receive next things from Mawi Team :
1) URL - web-page address
2) URL for API endpoints - Request access to API documentation(updae/revoke tokens etc.)
3) Client ID - your application ID
4) Client Secret - unique token for your application to authorize requests

### 2. Installing and Deployment

Cross-domain pop-up built with **zoid**, to use it on your page load scripts [URL]/js/zoid.min.js and [URL]/js/component.js,
add "placeholder" DOM-node with proper id: ```<div id="mawi-login" style="display: none;"></div>``` (without display: none zoid will set width and height of "placeholder" div to the values of the pop-up), then use   
```
ZoidLogin({
      username: 'YOUR-USERNAME',
      password: 'YOUR-PASSWORD',
      onLogin: function (response) {
        /*your handling of response data, such as accesToken, status, etc.*/
      }
    }).render('#mawi-login');
```
to open pop-up (use onclick action, most browsers will block pop-up without this requirement).
Use ```onLogin``` callback as a function with ```response``` argument, ```response``` is an object from API call request of Mawi User Authorization. 

## 3. Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds
* [Zoid](https://github.com/krakenjs/zoid) - Cross-domain pop-up component

## 4. Authors

* **Artem Malynovskyi** - *Initial work* - [artemmalynovskyi](https://github.com/artemmalynovskyi)
* **Kostyantin Kurynni** - *Initial work* - [artemmalynovskyi](https://github.com/artemmalynovskyi)


## 5. License

Will be provided soon

## 6. Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
