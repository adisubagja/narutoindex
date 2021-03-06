

# Naruto Index
Combining the power of [Cloudflare Workers](https://workers.cloudflare.com/) and [Google Drive](https://www.google.com/drive/) will allow you to index you files on the browser on Cloudflare Workers.    

[go2index/index.js](https://github.com/thomasshelbybot/narutoindex/tree/master/go2index) is the content of the Workers script.  

This theme's goindex is currently based on [yanzai/goindex](https://github.com/yanzai/goindex/)

## Features

- [x] 🗂 Multi drive switching
- [x] 🔐 Http Basic Auth
- [x] 🎨 Grid view mode(File Preview)
- [x] 🎯 Paging load
- [x] 🌐 I18n(multi-language)
- [x] 🛠 Html render 
- [x] 🖥 Video Online(mp4,mkv,webm,flv,m3u8)
- [x] 🚀 Faster speed

## TODO

- [ ] More file format preview
- [ ] Let goindex be more than just a directory index

## Quick Deployment

1. Open https://narutoindex.glitch.me  
2. Auth and get the code  
3. Deploy the code to [Cloudflare Workers](https://www.cloudflare.com/)

## Deployment  

1. Open [Google Drive API](https://console.developers.google.com/apis/api/drive.googleapis.com/overview)
2. Create a [OAuth client ID](https://console.developers.google.com/apis/credentials/oauthclient)
3. Install [rclone](https://rclone.org/downloads/) software locally
4. Get `refresh_token ` with `rclone`
5. Download `index.js` in https://github.com/thomasshelbybot/narutoindex/tree/master/go2index and replace `client_id`,`client_secret`,`refresh_token` for what you just got.
6. Deploy the code to [Cloudflare Workers](https://www.cloudflare.com/)

> If you write a good article and want to share it with others, please submit Issues and I will post the link here.

## Logs

### 2020-5-20

- Program changed to SPA(single page application)

- Add page level cache(The browser does not refresh and load in seconds after backward, and Mac users have a better experience of using touch pad)
- Add http basic auth(Each drive letter can be configured with a user name and password separately, which can protect all sub files and sub folders under the drive)
- Add  grid view mode(File preview)
- Add paging load
- Add  i18n
- Add html render 
- Add render folder/file description
- Add optional configuration
- Support quick deployment
- Support PDF Online preview
- Replace text editor
- Solve the problem of URL encoding
- Solve other known problems

### 2020-4-29

- Support multi disk switching
- Add version detection
- Optimize search results
- Optimize page display

## About

At the beginning of this project, it was just to satisfy my personal perception and experience development. When this project reaped the first start, the first fork and the first issues, and then everyone began to make suggestions, I had the power to update. Thank you very much for your support. Now we have version 2.0.

## Lisense

[MIT](LICENSE)

