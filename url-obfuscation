import os
import time
url=''
def display_message(message):
    print(message)
    time.sleep(3)
    os.system('cls' if os.name == 'nt' else 'clear')
display_message('dash URL Obfuscator 🎭')
display_message('dash lives forever')
display_message('https://t.me/dash027')
display_message('Welcome User 😊')
open_redirect=[ '--- URLS with Redirection Notice ---\n',
                'https://www.google.com/url?q=',  
                'https://google.com/url?q='     ,
                'https://facebook.com/l.php?u=',

                '\n--- URLS with No Redirection Warnings ---\n',

                'https://via.hypothes.is/' ,
                'http://vk.com/away.php?to=',
                'https://googleweblight.com/i?u=' ,
                'https://l.wl.co/l?u=',
                'https://tor2web.onionsearchengine.com/index.php?q=',
                'https://proxy.torgateway.com/index.php?q=',  
                'https://onionengine.com/url.php?u=', 
                'http://raspe.id.au/bypass/miniProxy.php?', 
                'https://www.awin1.com/cread.php?awinmid=6798&awinaffid=673201&ued=',
                'https://www.anrdoezrs.net/click-6361382-15020510?url=',
                'https://www.digit.in/flipkart/intermediate?url=',
                'https://adclick.g.doubleclick.net/pcs/click?url=',
                'https://shop-links.co/link?url=',

                '\n--- ONION URLs ---\n',

                'http://haystak5njsmn2hqkewecpaxetahtwhsbsa64jom2k22z5afxhnpxfid.onion/redir.php?url=',
                'http://zgphrnyp45suenks3jcscwvc5zllyk3vz4izzw67puwlzabw4wvwufid.onion/url.php?u=',  

                '\n--- Tor Onion URL Redirection ---\n',

                'https://ahmia.fi/search/search/redirect?redirect_url=',     
                'http://juhanurmihxlp77nkq76byazcldy2hlmovfu2epvl5ankdibsot4csyd.onion/search/search/redirect?redirect_url='
                ]


def get_url():
    print('\nInput your URL: ', end='') 
    global url
    tmp = input()
    if tmp.startswith('http://') or tmp.startswith('https://'):
        url = tmp
    else:
        url = 'http://' + tmp


def file_w():
    with open('url_obfuscated.txt', 'w') as f:
        for i in open_redirect:
            if '---' in i:
                f.write(i)
            else:
                f.write(f'{i}{url}\n')
def http_basic_auth():
    custom_url = [
        'https://accounts.google.com+signin=secure+v2+identifier=passive@',
        'https://facebook.com+login=secure+settings=private@',
        'https://instagram.com+accounts=login+settings=private@',
        'https://linkedin.com+accounts=securelogin+settings=private@',
        'https://github.com+login=secure+settings=private@'
    ]            
    with open('url_obfuscated.txt', 'a+') as f:
        f.write('\n--- Custom HTTP BASIC AUTH URLS [ Don\'t work in Firefox ] ---\n')
        for i in custom_url:
            if url.startswith('https://'):
                f.write(i + url[8:] + '\n')
            elif url.startswith('http://'):
                f.write(i + url[7:] + '\n')
get_url()
file_w()
http_basic_auth()

x = input(f'\n{os.getcwd()}/url_obfuscated.txt Generated!!!\n\nPress Enter to continue...')
