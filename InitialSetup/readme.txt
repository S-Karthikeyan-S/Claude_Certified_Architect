Since claude api has a price we are using googleapi since its free. We are running the code with anthropic SDK using Google api\\
by using LITELLM proxy to use google api key with Anthropic SDK

first lets download the litellm to provide us the proxy server: 
 Run 
pip install litellm[proxy]
pip install anthropic litellm


In your terminal provide the apikey:
$env:GEMINI_API_KEY="your_API_key"

to print and check the api key:
$env:GEMINI_API_KEY    -> This command will print the api key which u have setitup

to start the proxy server in your local machine run the below command in the terminal:
litellm --model gemini/gemini-2.5-flash --port 8000

to connect with the yaml file use the below command : 
litellm --config config.yaml --port 8000

to close the connection:
ctrl + c
