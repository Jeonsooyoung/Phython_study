# 2 BUILDING A JOB SCRAPPER

# 2.0 What is Web Scrapping     
- What is Web Scrapping
: 웹상의 데이터를 추출하는 것을 이야기함

- Scrapping : 
url 에서 제목과 상단 이미지를 가져와서 화면에 보여줌 

* 활용 예시
내가 새 휴대폰을 구입하고 싶을 때, 
파이썬 스크립트를 통해서 웹사이트 내 휴대폰 정보를 불러올 수 있음,
할인 상품/할인률/최저가 정보 등등 정보 추출 가능
그외에도 리뷰를 비교, 제품 색인,영화를 리뷰하는 등등
사용 가능


# 2.1 What are We Building      
- 프로젝트 목표 : 이번 프로젝트에서 파이썬 개발 일자리에 대한 정보를 크롤링함. (Indeed/stackoverflow)

- 최종 결과물 : indeed/stackoverflow 에서 python 검색시, 나오는 검색 결과를 불러온 후, 가져온 모든 데이터를 엑셀 시트로 옮김

# 2.2 Navigating with Python      
- import urllib : 파이썬에서 제공하는 라이브러리
- python request : 파이썬에서 요청을 만드는 기능을 모아 놓은 것 (import requests)<br>
ex) indeed_result = request.get("https://www.indeed.com/jobs?q=python&limit=50")
requests 패키지 사용하여 파이썬을 통해서 페이지의 URL 을 가져옴 

- HTML 가져오기
ex) print(indeed_result.text)

- 페이지 숫자 가져오기
 : beautiful soup을 통해서 페이지 숫자 추출


# 2.3 Extracting Indeed Pages      
- beautiful soup 통해서 page 숫자 추출    
<code>
from bs4 import BeautifulSoup

indeed_result = requests.get("https://indeed.com/jobs?q=python&limit=50")

indeed_soup = BeautifulSoup(indeed_result.text,"html.parset")

print(indeed_soup)

pagination = indeed_soup.find("div",{"class":"pagination"})
print(pagination)
</code>


# 2.4 Extracting Indeed Pages part Two      
<code>
from bs4 import BeautifulSoup

indeed_result = requests.get("https://indeed.com/jobs?q=python&limit=50")

indeed_soup = BeautifulSoup(indeed_result.text,"html.parset")

print(indeed_soup)

pagination = indeed_soup.find("div",{"class":"pagination"})
print(pagination)

links = pagination.find_all("a")
pages = []
print(links)

- 모든 anchor의 span을 찾기
for link in links : 
    print(link.find("span"))
    pages.append(link.find("span"))

max_page = pages[0:-1]

</code>

# 2.5 Requesting Each Page      
from bs4 import BeautifulSoup

#재사용 가능하도록 정리#
<code>
LIMIT = 50
indeed_URL = requests.get(f"https://indeed.com/jobs?q=python&limit={LIMIT}")

def extract_indeed_pages () : 
    result = requests.get(indeed_URL)

    soup = BeautifulSoup(result.text,"html.parser")

    print(soup)

    pagination = soup.find("div",{"class":"pagination"})
    print(pagination)

    links = pagination.find_all("a")
    pages = []
    print(links)

    /*  모든 anchor의 span을 찾기 */
    for link in links : 
        print(link.find("span"))
        pages.append(link.find("span"))

    max_page = pages[0:-1]
    return max_page

def extract_indeed_jobs (last_page) : 
    jobs = []
    for page in range(last_page)
        #print(f"&start={page*LIMIT}")#
        result = requests.get(f"{URL}&start={page*LIMIT}")
        print(result.status_code)
        soup = BeautifulSoup(result.text,"html.parser")
        results = soup.find_all("div",{"class":"jobsearch-SerpJobCard"})
        print(results)
        for result in results : 
            title = result.find("div",{"class":"title"}).find("a")
    return jobs

</code>


# 2.6 Extracting Titles      
# 2.7 Extracting Companies      
# 2.8 Extracting Locations and Finishing up      
# 2.9 StackOverflow Pages      
# 2.10 StackOverflow extract jobs      
# 2.11 StackOverflow extract job      
# 2.12 StackOverflow extract job part Two      
# 2.13 StackOverflow Finish      
# 2.14 What is CSV      
# 2.15 Saving to CSV      
# 2.16 OMG THIS IS AWESOME     


