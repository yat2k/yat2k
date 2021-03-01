<h3>Intro</h3>  
Yo! Its me!! Yathin!! But you can call me yat :p<br>
I'm an Information Science student at The National Institute of Engineering, Mysuru :computer:<br>    
I'm a front end developer :p but slowly transitioning into becoming a fullstack dev :D<br>
I also love making Discord Bots and learn something new everytime :sunny:<br>
![counter](https://enzqf6vglvco8wv.m.pipedream.net)


<h3>Languages and Tools<h3>    
<img align="left" alt="Visual Studio Code" width="26px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/visual-studio-code/visual-studio-code.png" style="max-width:100%;">
<img align="left" alt="HTML5" width="26px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/html/html.png" style="max-width:100%;">
<img align="left" alt="CSS3" width="26px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/css/css.png" style="max-width:100%;">
<img align="left" alt="JavaScript" width="26px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/javascript/javascript.png" style="max-width:100%;">
<img align="left" alt="C++" width="26px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/cpp/cpp.png" style="max-width:100%;">
<img align="left" alt="Python" width="26px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" style="max-width:100%;">
<img align="left" alt="C" width="26px" src="https://logodix.com/logo/640491.png" style="max-width:100%;">
<img align="left" alt="C" width="26px" src="https://logodix.com/logo/840708.png" style="max-width:100%;">
  
async(events,steps)=>{  
  const axios = require("axios")

// Retrieve existing counter and increment for this view
// See https://docs.pipedream.com/workflows/steps/code/state/
const counter = $checkpoint + 1 || 1

// Use shields.io to generate a badge with our counter as the message
const { data } = await axios({
  url: `https://img.shields.io/static/v1?label=Profile-Views&message=${counter}&color=green`,
})

// Save the incremented counter back to state
$checkpoint = counter

// See https://docs.pipedream.com/workflows/steps/triggers/#customizing-the-http-response
$respond({
  status: 200,
  headers: {
    'Content-Type': 'image/svg+xml',
    'Cache-Control': 'max-age=0, no-cache, no-store, must-revalidate'
  },
  body: data,
}) 

}
