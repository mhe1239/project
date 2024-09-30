import random as r
import time

value = ("가위", "주먹", "보")

print("=" * 30)
print("""AI와 함께하는 가위바위보 대결장에 오신것을 환영합니다.
Welcome""")
print("=" * 30)

health = 3
rock_art_player = """
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
"""
rock_art_ai = """
        _______
   ____(____   '--- 
  (_____)
  (_____)
  (____)
   (___)__.---
"""

scissors_art_player = """
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
"""
scissors_art_ai = """
        _______
   ____(____   '--- 
  (______
 (__________
       (____)
       (___)__.---
"""

paper_art_player = """
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
"""
paper_art_ai = """
        _______
   ____(____   '--- 
  (______
 (_______
 (_______
       (__________.---
"""

while health > 0:
    write = input("주먹 가위 보 <<< 선택 하여 쓰시오: ")
    if write not in value:
        print("잘못된 값을 입력했습니다.")
        continue
    print("당신의 값은:", write)
    if write == "가위":
        print(scissors_art_player)
    elif write == "주먹":
        print(rock_art_player)
    elif write == "보":
        print(paper_art_player)
    time.sleep(2)
    
    a = r.choice(value)
    print("AI의 값은:", a)
    if a == "가위":
        print(scissors_art_ai)
    elif a == "주먹":
        print(rock_art_ai)
    elif a == "보":
        print(paper_art_ai)

    if write == a:
        print("무승부가 나셨습니다.")
        print("""
         _   _ ______          _____ 
        | | | || ___ \\    _   |  _  |
        | |_| || |_/ /  _| |_ | |/' |
        |  _  ||  __/  |_   _||  /| |
        | | | || |       |_|  \\ |_/ /
        \\_| |_/\\_|             \\___/ 
        """)
        print("당신의 현재 생명력은:", health)
    elif (write == "가위" and a == "보") or (write == "주먹" and a == "가위") or (write == "보" and a == "주먹"):
        print("당신은 이겼습니다.")
        health += 1
        print("""
         _   _ ______          __  
        | | | || ___ \\    _   /  | 
        | |_| || |_/ /  _| |_ `| | 
        |  _  ||  __/  |_   _| | | 
        | | | || |       |_|  _| |_
        \\_| |_/\\_|            \\___/
        """)
        print("당신의 현재 생명력은:", health)
    else:
        print("당신은 졌습니다.")
        health -= 1
        print("""
         _   _ ______           __  
        | | | || ___ \\         /  | 
        | |_| || |_/ /  ______ `| | 
        |  _  ||  __/  |______| | | 
        | | | || |             _| |_
        \\_| |_/\\_|             \\___
        """)
        print("당신의 현재 생명력은:", health)
        

print("게임 오버! 당신의 최종 생명력은:", health)
