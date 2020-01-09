# 智能博物馆PRD文档
### 项目概括：兼具导航，讲解，参展路线推荐的智能软件
| 发布日期   | 2019/12/03   |
| ---------- | ------------ |
| 项目名称   | 智能博物馆 |
| 项目状态   | 完成      |
| 项目负责人 | 黄琪琪       |

# 一、 产品定位：
博物馆本身承担着社会教育功能，如何更好的发挥社会教育功能，目前博物馆所需的就是提高博物馆的服务水平，讲解水平，还有展品的质量。API让我们可以从服务和讲解入手，更好发挥博物馆的社会教育功能。所以我们要打造一款具有推荐、语音功能、图片识别的智能app。
* 目标市场：
主要针对那些比较老旧的博物馆或者是还没有进行智慧化的博物馆帮助他们用最快的方式和相对较低的价格转型升级。
* 市场需求：
在大多数二三线或者是四线城市的博物馆都是比较老旧且设施不齐全的，所以这些博物馆是需要一些较为廉价和适应性较强的项目产品对其进行转型升级来满足当地对博物馆的教育需求。

# 二、同类产品竞争分析
我们的产品与智慧博物馆主要的差别在于智慧博物馆是一个借助物联网和云计算技术实现的智能的新兴博物馆。而我们的产品是相对于博物馆本身比较独立的，它本身投入的成本就较为低廉不像智慧博物馆那样是以创建博物馆的生态形同为基础的。所以我们的项目可以根据不同的博物馆情况进行有目的有规划的适应性更改。更强的适应性和弹性使得我们的产品受众的博物馆会更加的多。

# 三、加值宣言
让用户选择几个想要观览的展品，调用应用机器算法从而计算出用户的个人喜好，为推荐一条专属的游览路线。调用语音合成实现语音导航，可以为用户提供更好的游览服务，也更加的有趣，让用户在感兴趣的前提下去探索去学习。

* 调用百度图像识别API：用户将允许拍照的展品通过拍照上传，（如不能拍照的展品可以输入名字），系统分析图片，然后将得到的结果通过语音的方式为用户讲解，有趣的讲解将会更好的让用户对藏品知识的学习。

* 调用百度语音识别API： 提供长语音转化成文字的功能，博文关的讲解员讲解可以转换成文字，为听力障碍者提供文字功能，让他们能和其他人一样得到讲解元的服务，更好了解博物馆的展示。

* 调用百度语音合成API：帮助视觉障碍者提供朗读功能，提供语音问答功能。也为其他人提供了解放双手的可能。通过导览小程序，使用语音合成技术为访客提供多种发音人的朗读功能与多种语言模式，获得更极致的阅读体验。支持多种参数配置，可根据场景需求对发音人的语速、音调、音量进行灵活设置，满足个性化需求。

* 调用图灵机器人API智能问答API：利用知识图谱理解用户搜索语义，并给出正确答案。也有简单的对话功能。
* 调用高德地图API，为用户提供前往展馆的路线。并且可以让用户清楚所在的位置。
# 四、核心价值
* 语音合成：使用语音合成技术为访客提供多种发音人的朗读功能与多种语言模式，支持多种参数配置，可根据场景需求对发音人的语速、音调、音量进行灵活设置，满足个性化需求。

* 图像识别：使用图像识别技术，让用户在不知道展品是什么的情况下，使用图像识别获得展品介绍。
* 导航功能：使用高德地图API为用户提供导航服务，用户使用手机即可知道各个展品的具体位置。

# 五、用户痛点分析
明确的指标：设计AR导览员小程序给博物馆用
 
* （1）：博物馆工作人员有限，不能即使的为每一个游览者提供有效的服务，服务的缺失影响了游客的体验，也影响了游客享受博物馆的社会教育功能。很多时候，游客会在博物馆迷路，同时也不能得到有效的知识讲解。
 
* （2）：博物馆场地复杂，展品繁多，如果用户想将全部展品游览且消化是一件很难得事情。没有目的的在博物馆逛可能会降低游客的游览效率，不能形成系统的知识学习。
 
* （3）：展品静静的躺在展台等待着前来欣赏的人，但是很多来博物馆游览的游客并没有很高的文化修养，所以来博物馆也是她们进修的一个方式，但是博物馆的讲解一般以文字和讲解员为主，但是文字缺乏生动性，不能达到很强的教育效果；讲解员也水平参差不齐，同时博物馆资金限制，不能再每一个展区，每一个展品之前都有讲解员，因而很多希望来博物馆接受社会教育的人却不能得到有效的教育。

# 六、功能详情与整合功能
## 使用操作说明：
* 通过语音查找想要参观的展品位置与信息：将用户的语音精准识别为文字（，再通过语音合成将用户所查找的展品的位置与信息
* 通过语音反馈给用户；提供导航服务，用户实现不用跳转app即可获得前往展品的最佳路线；
* 通过上传展品的照片来获得展品的信息：在博物馆展品图库中搜索与用户上传图片相同及相近的展品，然后将得到的结果通过语音合成反馈给用户；
* 通过线上参观，甚至不用到达博物馆，都可以得到所有展品信息。如果前来，调用高德api实现馆内参观。

# 七、产品原型
[产品原型](http://nicekiki.gitee.io/museum_prototype)（建议用Google Chrome打开）
## 1.语音问答：
![语音问答](https://images.gitee.com/uploads/images/2020/0109/215930_ecc1379a_1648193.png "屏幕截图.png")
 ![调用的api](https://images.gitee.com/uploads/images/2020/0109/215549_9ba1d298_1648193.png "屏幕截图.png")
## 2.拍一拍
[拍一拍]（https://github.com/KIKINICE/museum/blob/master/%E6%8B%8D%E4%B8%80%E6%8B%8D.png)

## 3.智能浏览
![智能浏览](https://images.gitee.com/uploads/images/2020/0109/220331_25fb6cc0_1648193.png "屏幕截图.png")
# API使用水平：
## 1.调用Azure API key 进行图像识别
```
import requests
import os
import sys
# If you are using a Jupyter notebook, uncomment the following line.
# %matplotlib inline
import matplotlib.pyplot as plt
import json
from PIL import Image
from io import BytesIO

# Add your Computer Vision subscription key and endpoint to your environment variables.
if 'COMPUTER_VISION_SUBSCRIPTION_KEY' in os.environ:
    subscription_key = os.environ['COMPUTER_VISION_SUBSCRIPTION_KEY']
else:
    print("\nSet the COMPUTER_VISION_SUBSCRIPTION_KEY environment variable.\n**Restart your shell or IDE for changes to take effect.**")
    sys.exit()

if 'COMPUTER_VISION_ENDPOINT' in os.environ:
    endpoint = os.environ['COMPUTER_VISION_ENDPOINT']

analyze_url = endpoint + "vision/v2.0/analyze"

# Set image_url to the URL of an image that you want to analyze.
image_url = "[https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=1754667609](https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=1754667609),3961441332&fm=26&gp=0.jpg"

headers = {'Ocp-Apim-Subscription-Key': subscription_key}
params = {'visualFeatures': 'Categories,Description,Color'}
data = {'url': image_url}
response = requests.post(analyze_url, headers=headers,
                         params=params, json=data)
response.raise_for_status()

# The 'analysis' object contains various fields that describe the image. The most
# relevant caption for the image is obtained from the 'description' property.
analysis = response.json()
print(json.dumps(response.json()))
image_caption = analysis["description"]["captions"][0]["text"].capitalize()

# Display the image and overlay it with the caption.
image = Image.open(BytesIO(requests.get(image_url).content))
plt.imshow(image)
plt.axis("off")
_ = plt.title(image_caption, size="x-large", y=-0.1)
plt.show()
```
## 2.调用高德地图api
```
import requests
from PIL import Image
from io import BytesIO
key_kiki = '03e820a955f427fbcb22b85faf6afca2'
def walking(origin,destination)->dict:
    url = '[https://restapi.amap.com/v3/direction/walking?parameters](https://restapi.amap.com/v3/direction/walking?parameters)'
    params={
        'key':key_kiki,
        'origin':origin,
        'destination':destination,
        'output':'json'
    }
    response = requests.get(url,params=params)
    data = response.json()
    return data
walking('116.481038,39.989543','116.434546,39.91816')
```
## 3.调用百度语言合成API
```
import requests
import base64
from aip import AipSpeech

""" 你的 APPID AK SK """
APP_ID = '2fa1c821284f4129939860f55751657c'
API_KEY = 'c473c6db-f83b-ba9a-6a54-9dc7eea7225d'
SECRET_KEY = 'lSzTRUvqGHsq5Pd42XaH8VhEXB7IcRXk'

client = AipSpeech(APP_ID, API_KEY, SECRET_KEY)


# In[7]:


# coding=utf-8
import sys
import json

IS_PY3 = sys.version_info.major == 3
if IS_PY3:
    from urllib.request import urlopen
    from urllib.request import Request
    from urllib.error import URLError
    from urllib.parse import urlencode
    from urllib.parse import quote_plus
else:
    import urllib2
    from urllib import quote_plus
    from urllib2 import urlopen
    from urllib2 import Request
    from urllib2 import URLError
    from urllib import urlencode

API_KEY = '4E1BG9lTnlSeIf1NQFlrSq6h'
SECRET_KEY = '544ca4657ba8002e3dea3ac2f5fdd241'

TEXT = "去五号展馆"
PER = 4
# 语速，取值0-15，默认为5中语速
SPD = 3
# 音调，取值0-15，默认为5中语调
PIT = 5
# 音量，取值0-9，默认为5中音量
VOL = 5
# 下载的文件格式, 3：mp3(default) 4： pcm-16k 5： pcm-8k 6. wav
AUE = 3

FORMATS = {3: "mp3", 4: "pcm", 5: "pcm", 6: "wav"}
FORMAT = FORMATS[AUE]

CUID = "123456PYTHON"

TTS_URL = '[http://tsn.baidu.com/text2audio](http://tsn.baidu.com/text2audio)'


class DemoError(Exception):
    pass


"""  TOKEN start """

TOKEN_URL = '[http://openapi.baidu.com/oauth/2.0/token](http://openapi.baidu.com/oauth/2.0/token)'
SCOPE = 'audio_tts_post'  


def fetch_token():
    print("fetch token begin")
    params = {'grant_type': 'client_credentials',
              'client_id': API_KEY,
              'client_secret': SECRET_KEY}
    post_data = urlencode(params)
    if (IS_PY3):
        post_data = post_data.encode('utf-8')
    req = Request(TOKEN_URL, post_data)
    try:
        f = urlopen(req, timeout=5)
        result_str = f.read()
    except URLError as err:
        print('token http response http code : ' + str(err.code))
        result_str = err.read()
    if (IS_PY3):
        result_str = result_str.decode()

    print(result_str)
    result = json.loads(result_str)
    print(result)
    if ('access_token' in result.keys() and 'scope' in result.keys()):
        if not SCOPE in result['scope'].split(' '):
            raise DemoError('scope is not correct')
        print('SUCCESS WITH TOKEN: %s ; EXPIRES IN SECONDS: %s' % (result['access_token'], result['expires_in']))
        return result['access_token']
    else:
        raise DemoError('MAYBE API_KEY or SECRET_KEY not correct: access_token or scope not found in token response')


"""  TOKEN end """

if __name__ == '__main__':
    token = fetch_token()
    tex = quote_plus(TEXT)  # 此处TEXT需要两次urlencode
    print(tex)
    params = {'tok': token, 'tex': tex, 'per': PER, 'spd': SPD, 'pit': PIT, 'vol': VOL, 'aue': AUE, 'cuid': CUID,
              'lan': 'zh', 'ctp': 1}  # lan ctp 固定参数

    data = urlencode(params)
    print('test on Web Browser' + TTS_URL + '?' + data)

    req = Request(TTS_URL, data.encode('utf-8'))
    has_error = False
    try:
        f = urlopen(req)
        result_str = f.read()

        headers = dict((name.lower(), value) for name, value in f.headers.items())

        has_error = ('content-type' not in headers.keys() or headers['content-type'].find('audio/') < 0)
    except  URLError as err:
        print('asr http response http code : ' + str(err.code))
        result_str = err.read()
        has_error = True

    save_file = "error.txt" if has_error else 'result.' + FORMAT
    with open(save_file, 'wb') as of:
        of.write(result_str)

    if has_error:
        if (IS_PY3):
            result_str = str(result_str, 'utf-8')
        print("tts api  error:" + result_str)

    print("result saved as :" + save_file)
```
## 4.调用百度语音识别API
```
from aip import AipSpeech

""" 你的 APPID AK SK """
APP_ID = '2fa1c821284f4129939860f55751657c'
API_KEY = '03hu0vBRBqsZHBYNPaY1dELP'
SECRET_KEY = 'VuZDlIupGaoxPBFFCATDCI6kTdQ8dzZT'

client = AipSpeech(APP_ID, API_KEY, SECRET_KEY
import sys
import json

IS_PY3 = sys.version_info.major == 3
if IS_PY3:
    from urllib.request import urlopen
    from urllib.request import Request
    from urllib.error import URLError
    from urllib.parse import urlencode
    from urllib.parse import quote_plus
else:
    import urllib2
    from urllib import quote_plus
    from urllib2 import urlopen
    from urllib2 import Request
    from urllib2 import URLError
    from urllib import urlencode

API_KEY = '03hu0vBRBqsZHBYNPaY1dELP'
SECRET_KEY = 'VuZDlIupGaoxPBFFCATDCI6kTdQ8dzZT'

TEXT = "apple"

PER = 4
# 语速，取值0-15，默认为5中语速
SPD = 5
# 音调，取值0-15，默认为5中语调
PIT = 5
# 音量，取值0-9，默认为5中音量
VOL = 5
# 下载的文件格式, 3：mp3(default) 4： pcm-16k 5： pcm-8k 6. wav
AUE = 3

FORMATS = {3: "mp3", 4: "pcm", 5: "pcm", 6: "wav"}
FORMAT = FORMATS[AUE]

CUID = "123456PYTHON"

TTS_URL = '[http://tsn.baidu.com/text2audio](http://tsn.baidu.com/text2audio)'


class DemoError(Exception):
    pass


"""  TOKEN start """

TOKEN_URL = '[http://openapi.baidu.com/oauth/2.0/token](http://openapi.baidu.com/oauth/2.0/token)'
SCOPE = 'audio_tts_post'  # 有此scope表示有tts能力，没有请在网页里勾选


def fetch_token():
    print("fetch token begin")
    params = {'grant_type': 'client_credentials',
              'client_id': API_KEY,
              'client_secret': SECRET_KEY}
    post_data = urlencode(params)
    if (IS_PY3):
        post_data = post_data.encode('utf-8')
    req = Request(TOKEN_URL, post_data)
    try:
        f = urlopen(req, timeout=5)
        result_str = f.read()
    except URLError as err:
        print('token http response http code : ' + str(err.code))
        result_str = err.read()
    if (IS_PY3):
        result_str = result_str.decode()

    print(result_str)
    result = json.loads(result_str)
    print(result)
    if ('access_token' in result.keys() and 'scope' in result.keys()):
        if not SCOPE in result['scope'].split(' '):
            raise DemoError('scope is not correct')
        print('SUCCESS WITH TOKEN: %s ; EXPIRES IN SECONDS: %s' % (result['access_token'], result['expires_in']))
        return result['access_token']
    else:
        raise DemoError('MAYBE API_KEY or SECRET_KEY not correct: access_token or scope not found in token response')


"""  TOKEN end """

if __name__ == '__main__':
    token = fetch_token()
    tex = quote_plus(TEXT)  # 此处TEXT需要两次urlencode
    print(tex)
    params = {'tok': token, 'tex': tex, 'per': PER, 'spd': SPD, 'pit': PIT, 'vol': VOL, 'aue': AUE, 'cuid': CUID,
              'lan': 'zh', 'ctp': 1}  # lan ctp 固定参数

    data = urlencode(params)
    print('test on Web Browser' + TTS_URL + '?' + data)

    req = Request(TTS_URL, data.encode('utf-8'))
    has_error = False
    try:
        f = urlopen(req)
        result_str = f.read()

        headers = dict((name.lower(), value) for name, value in f.headers.items())

        has_error = ('content-type' not in headers.keys() or headers['content-type'].find('audio/') < 0)
    except  URLError as err:
        print('asr http response http code : ' + str(err.code))
        result_str = err.read()
        has_error = True

    save_file = "error.txt" if has_error else 'result.' + FORMAT
    with open(save_file, 'wb') as of:
        of.write(result_str)

    if has_error:
        if (IS_PY3):
            result_str = str(result_str, 'utf-8')
        print("tts api  error:" + result_str)

    print("result saved as :" + save_file)
```
## 5.调用图灵机器人API
```
import json
import urllib.request
while 1:
    try:
        api_url = "[http://openapi.tuling123.com/openapi/api/v2](http://openapi.tuling123.com/openapi/api/v2)"
        text_input = input('我：')
        if text_input == 'exit':
            break
        req = {
            "reqType": 0,  # 输入类型 0-文本, 1-图片, 2-音频
            "perception":  # 信息参数
            {
                "inputText":  # 文本信息
                {
                    "text": text_input
                },

                "selfInfo":  # 用户参数
                {
                    "location":
                    {
                        "city": "深圳",  # 所在城市
                        "province": "广东",  # 省份
                        "street": "红花岭路"  # 街道
                    }
                }
            },
            "userInfo":
            {
                "apiKey": "347b39ee228b4b109dae7270cc08d3c8",  
                "userId": "0001"  # 用户唯一标识(随便填, 非密钥)
            }
        }
        # print(req)
        # 将字典格式的req编码为utf8
        req = json.dumps(req).encode('utf8')
        # print(req)
        http_post = urllib.request.Request(api_url, data=req, headers={'content-type': 'application/json'})
        response = urllib.request.urlopen(http_post)
        response_str = response.read().decode('utf8')
        # print(response_str)
        response_dic = json.loads(response_str)
        # print(response_dic)
        intent_code = response_dic['intent']['code']
        results_text = response_dic['results'][0]['values']['text']
        print('机器人1号：', results_text)
        # print('code：' + str(intent_code))
    except KeyError:
        print('好的~')
```
###　代码下载链接：
[代码下载](https://github.com/KIKINICE/museum/blob/master/%E4%BB%A3%E7%A0%81%E4%B8%8B%E8%BD%BD.ipynb)

# 八、使用比较分析 

|      | 图灵机器人api                                                                                                                                                        | 青云智能聊天API                                                                                            |
| ---- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| 功能 | 语义理解 开放域聊天准确率81.64%，垂域技能准确率96.34%  知识图谱 千万级实体及关系知识，支持逻辑与关系的知识推理  多轮对话 开放域聊天与垂域技能超过5轮的上下文对话能力 | 支持功能：天气、翻译、藏头诗、笑话、歌词、计算、域名信息/备案/收录查询、IP查询、手机号码归属、人工智能聊天 |
| 体验 | 流畅自然 领先的增强学习模型，让机器人聊天对话更接近真人  情感交互 23类情绪识别及多维情感表达，让机器人更拟人化  记忆系统 通过深度记忆系统与用户画像，让机器人更懂你  | 功能少，无法通畅交流，体验感差                                                                             |



# 九、使用风险分析
>  风险通常是指由于当事者主观上不能控制的一些因素的影响，使得实际结果与当事者的事先估计有较大的背离而带来的损害。风险分析是找出行动方案的不确定性（主观上无法控制）因素，分析其环境状况和对方案的敏感程度；估计有关数据，包括行动方案的费用，在不同情况下得到的收益以及不确定性因素各种机遇的概率，计算各种风险情况下的效果；
* api无法调用的风险，key使用次数的限制，无法使用产品api
* api出现错误的风险
* 用户上传错误数据，导致api分析结果不显示的风险。

# 十、关于其他——成本效益分析
* 售前技术支持：销售给博物馆遇到无法解答的产品技术问题时，售前技术支持给予帮助。
* 售后技术支持：帮助博物馆诊断并解决其在使用产品过程中出现的有明显症状的，可能由产品导致的技术问题。
* 方法：技术支持有电话技术支持、上门服务技术支持等 。包括两方面内容，一是进行技术上的维护，二是进行服务上的沟通。
成本
* 新产品方案产生的效益
（1）降低人工成本（减少所需的人力物力）
（2）节省人员培训时间（讲解员需培训后才能上岗，而该软件则无需培训）
（3）可提供专属的定制化游览路线，带给用户更好的观览体验
（4）提高博物馆的服务水平，更好的发挥博物馆的社会教育功能
（5）博物馆可以容纳的观览人数增加，同时可以吸引更多游客前来






