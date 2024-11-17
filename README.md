# tuxi-fixes
i donwloaded tuxi and had an error, then i fixed it and am publishing it for somebody else that could not use it 


Introduction to Tuxi
Tuxi is a command-line tool designed to simplify the search and viewing of information directly from the terminal. With a straightforward and intuitive interface, Tuxi enables users to perform web searches quickly and efficiently, utilizing a set of commands that streamline access to relevant content. It is especially useful for developers and tech enthusiasts who prefer working in the terminal and want to integrate web searches into their workflows.

One of Tuxi's main features is its ability to display search results in an organized manner, allowing users to easily navigate through options. Additionally, it can be configured to use different search engines, providing flexibility and customization.

If you're interested in trying out Tuxi or contributing to its development, you can find the source code and more information in the official GitHub repository:

Official Tuxi GitHub Repository
https://github.com/Bugswriter/tuxi

Conclusion
Tuxi is an excellent addition for anyone looking to optimize their web searches directly from the terminal, combining the efficiency of command-line operations with the wealth of information available online. Give it a try and see how it can enhance your productivity!



## installing tuxi itself and its deps
    
    $ sudo curl -sL "https://raw.githubusercontent.com/Bugswriter/tuxi/main/tuxi" -o /usr/local/bin/tuxi
    $ sudo chmod +x /usr/local/bin/tuxi
    more info in https://github.com/Bugswriter/tuxi



## real stuff. you can save it as alias or local bins , you rule

    #short response
    ~/tuxi/tuxi -s "which is the most big animal on earth" > /dev/null 2>&1 ; cat /home/$USER/.cache/tuxi/$(ls -lt created /home/$USER/.cache/tuxi/ | awk '{print $7}'| tac | sed -n '1p') | sed -n 's/.*<div class="BNeawe s3v9rd AP7Wnd">\([^<]*\)<\/div>.*/\1/p'
    
    #not short response
    cat /home/$USER/.cache/tuxi/$(ls -lt created /home/$USER/.cache/tuxi/ | awk '{print $7}'| tac | sed -n '1p') | awk -F'x3' '{for(i=2; i<NF;i+=2) print $i}' | sed -n '/^e[^/]/p' | sed 's/^.\(.*\).$/\1/' | awk 'NF {print; last=$0; next} {if (last) print ""; last=""}'  | sed -n '/More results/{n; p; n; p;}'


## expecteds responses 

    Far bigger than any dinosaur, the blue whale is the largest known animal to have ever lived. An adult blue whale can grow to a massive 30m ...

and
    
    blue whale
    
    120 tons (109 metric tons)
    

    
