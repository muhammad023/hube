# hube
import requests

def video_yuklab_ber(link):
    url = "https://instagram-downloader-download-instagram-videos-stories.p.rapidapi.com/index"
    
    querystring = {"url":link}
    
    headers = {
      "X-RapidAPI-Key": "82d214d06amsh1a8779fec34649ep1ab62fjsn9de378a7509e",
      "X-RapidAPI-Host": "instagram-downloader-download-instagram-videos-stories.p.rapidapi.com"
    }
    
    response = requests.get(url, headers=headers, params=querystring)
    
    return response.json()
