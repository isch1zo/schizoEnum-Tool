### بسم الله الغفور الرحيم

### ابرأ امام الله من اي استخدام لاي اداة من ادواتي لألحاق الضرر بالأخرين
# schizoEnum Tool

## schizoEnum.sh Tool is a web recon automation wrapper tool that includes many enumeration tools.
The tool needs to download the tools used in it. For the time being, you have to download the tools used by yourself and maybe at another time I will program a tool to download the tools and arrange them automatically

## The Idea:
first the tool gets the domain from user input. Then do subdomains enumeration for that domain using below tools:
1- subfinder
2- assetfinder
3- sublist3r
4- findomain
5- knockpy
6- massdns

Then grep all results and arranged to remove duplicates and save the final result in 'finaldomains.txt'

Next step is to get the alive domains and save them in 'alive.txt' file.

Then the tool will use 'alive.txt' to do two things:
1- get urls by waybackurls tool
2- screen shot all alive domains by using webscreenshot tool
