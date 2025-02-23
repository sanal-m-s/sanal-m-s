import webbrowser
import os
import sys

def open_links():
    links = [
        "https://sanalms.vercel.app/",
        "https://twitter.com/sanal80469020",
        "https://linkedin.com/in/sanal-m-s-a75b77276",
        "https://instagram.com/__.sanal.__",
        "https://www.youtube.com/c/sanal9584",
        "https://www.buymeacoffee.com/sanalms"
    ]
    for link in links:
        try:
            webbrowser.open(link)
        except Exception as e:
            print(f"Failed to open {link}: {e}")

def display_info():
    about_me = {
        "Name": "Sanal M S",
        "Profession": "Frontend Developer | UI/UX Designer | Tech Enthusiast",
        "Education": "Master's in Computer Applications",
        "Skills": ["HTML", "CSS", "JavaScript", "React", "Tailwind", "Bootstrap", "Java", "Python", "PHP", "MySQL", "MongoDB", "Android Studio", "Figma", "Photoshop", "Illustrator"],
        "Hobbies": ["Web Design", "Creating YouTube Videos", "Mobile App Development"]
    }
    
    print("🔥 About Me 🔥")
    for key, value in about_me.items():
        if isinstance(value, list):
            print(f"{key}: {', '.join(value)}")
        else:
            print(f"{key}: {value}")

def show_github_stats():
    github_links = [
        "https://github-readme-stats.vercel.app/api?username=sanal-m-s&show_icons=true&theme=tokyonight",
        "https://github-readme-stats.vercel.app/api/top-langs/?username=sanal-m-s&layout=compact&theme=tokyonight",
        "https://github-profile-trophy.vercel.app/?username=sanal-m-s&theme=onedark",
        "https://github-readme-activity-graph.cyclic.app/graph?username=sanal-m-s&theme=tokyonight"
    ]
    
    print("\n🚀 GitHub Stats 🚀")
    for stat in github_links:
        try:
            webbrowser.open(stat)
        except Exception as e:
            print(f"Failed to open {stat}: {e}")

def show_random_quote():
    try:
        webbrowser.open("https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical")
    except Exception as e:
        print(f"Failed to open quote API: {e}")

def show_spotify():
    try:
        webbrowser.open("https://spotify-github-profile.vercel.app/api/view?uid=your_spotify_id&cover_image=true&theme=default&show_offline=false&background_color=121212")
    except Exception as e:
        print(f"Failed to open Spotify API: {e}")

if __name__ == "__main__":
    display_info()
    open_links()
    show_github_stats()
    show_random_quote()
    show_spotify()
