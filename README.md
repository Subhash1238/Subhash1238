import time

def countdown(t):
    while t:
        mins, secs = divmod(t, 60)
        timer = '{:02d}:{:02d}'.format(mins, secs)
        print(f"\r⏳ Countdown: {timer}", end="")
        time.sleep(1)
        t -= 1
    print("\n\n🎉 Time's up! 🎉")

def birthday_wish():
    print("\n✨✨✨✨✨✨✨✨✨✨✨✨✨✨✨✨✨")
    print("✨                         ✨")
    print("✨   🎂🎉  Happy Birthday  🎉🎂   ✨")
    print("✨           Suraj!          ✨")
    print("✨                         ✨")
    print("✨✨✨✨✨✨✨✨✨✨✨✨✨✨✨✨✨\n")

    message = """
    🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈
    🎈                        🎈
    🎈   May your day be filled with   🎈
    🎈   joy, love, and laughter.    🎈
    🎈    Keep shining bright,      🎈
    🎈   just like you always do!    🎈
    🎈                        🎈
    🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈🎈
    """
    print(message)

def surprise_wish():
    print("Get ready for a special birthday wish!")
    countdown(5)
    birthday_wish()

surprise_wish()
