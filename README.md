# treasure-island-game
#Game about finding a treasure island

print('''
 ____________________________________________________________________
 / \-----     ---------  -----------     -------------- ------    ----\
 \_/__________________________________________________________________/
 |~ ~~ ~~~ ~ ~ ~~~ ~ _____.----------._ ~~~  ~~~~ ~~   ~~  ~~~~~ ~~~~|
 |  _   ~~ ~~ __,---'_       "         `. ~~~ _,--.  ~~~~ __,---.  ~~|
 | | \___ ~~ /      ( )   "          "   `-.,' (') \~~ ~ (  / _\ \~~ |
 |  \    \__/_   __(( _)_      (    "   "     (_\_) \___~ `-.___,'  ~|
 |~~ \     (  )_(__)_|( ))  "   ))          "   |    "  \ ~~ ~~~ _ ~~|
 |  ~ \__ (( _( (  ))  ) _)    ((     \\//    " |   "    \_____,' | ~|
 |~~ ~   \  ( ))(_)(_)_)|  "    ))    //\\ " __,---._  "  "   "  /~~~|
 |    ~~~ |(_ _)| | |   |   "  (   "      ,-'~~~ ~~~ `-.   ___  /~ ~ |
 | ~~     |  |  |   |   _,--- ,--. _  "  (~~  ~~~~  ~~~ ) /___\ \~~ ~|
 |  ~ ~~ /   |      _,----._,'`--'\.`-._  `._~~_~__~_,-'  |H__|  \ ~~|
 |~~    / "     _,-' / `\ ,' / _'  \`.---.._          __        " \~ |
 | ~~~ / /   .-' , / ' _,'_  -  _ '- _`._ `.`-._    _/- `--.   " " \~|
 |  ~ / / _-- `---,~.-' __   --  _,---.  `-._   _,-'- / ` \ \_   " |~|
 | ~ | | -- _    /~/  `-_- _  _,' '  \ \_`-._,-'  / --   \  - \_   / |
 |~~ | \ -      /~~| "     ,-'_ /-  `_ ._`._`-...._____...._,--'  /~~|
 | ~~\  \_ /   /~~/    ___  `---  ---  - - ' ,--.     ___        |~ ~|
 |~   \      ,'~~|  " (o o)   "         " " |~~~ \_,-' ~ `.     ,'~~ |
 | ~~ ~|__,-'~~~~~\    \"/      "  "   "    /~ ~~   O ~ ~~`-.__/~ ~~~|
 |~~~ ~~~  ~~~~~~~~`.______________________/ ~~~    |   ~~~ ~~ ~ ~~~~|
 |____~jrei~__~_______~~_~____~~_____~~___~_~~___~\_|_/ ~_____~___~__|
 / \----- ----- ------------  ------- ----- -------  --------  -------\
 \_/__________________________________________________________________/
''')
print("Welcome to Treasure Island.")
print("Your mission is to find the treasure without dying.") 


#Write your code below this line 
go = input("Choose left or right to start the game: \n").lower()
#Start of game
if go == "left":
  #continue game
  swim_wait = input("You find a small lake. Do you want swim across or wait (for a boat)? \n").lower()
  if swim_wait == "wait":
    #continue game
    door = input("You arrive in front of a building; which door do you want to enter? Choose Blue or Red. \n").lower()
    if door == "blue":
      #continue game
      cup = input("You find three cups  with liquid in it. You have to drink one of them to get vision powers. Which one drink? Choose: 1 , 2 or 3 \n")
      if cup == "3":
        #Continue game
        treasure = input("You have seen the treasure. Open and pick the treasure. Enter open: \n").lower()
        if treasure == "open":
          print("Congratulations you WON")
        else:
          print("You waited too long. The treasure exploded. Game over!!!")
      elif cup == "1":
        print("You drank acid and died. Game over!!!")
      else:
        print("You drank poison and died. Game over!!!")
    else:
      print("You are killed by pirates. Game over!!!")
  else:
    print("You are eaten by crocodiles. Game over!!!")
else:
  print("You ran into fire... Game over!!!")
